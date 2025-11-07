---
title: Configurar [!DNL Amazon S3] para Origem de Público-Alvo
description: Saiba como configurar e conectar seu armazenamento do  [!DNL Amazon S3] como uma fonte de dados de autoatendimento para assimilar dados de público-alvo no Real-Time CDP Collaboration.
source-git-commit: 05fd7ec466ba2b20264490bbbfadc9bb6d361bc8
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# Configurar [!DNL Amazon S3] para fornecimento de público

Saiba como configurar e conectar seu armazenamento do [!DNL Amazon S3] na interface do usuário do Adobe Real-Time CDP Collaboration aos dados de público-alvo de origem para ativação e análise de sobreposição.

>[!IMPORTANT]
>
>Antes de seguir este guia, é necessário concluir as etapas para autorizar a função IAM da Adobe na conta da AWS.\
>Consulte o guia **[Configurar permissões do AWS para fornecimento de público-alvo](./configure-aws-permissions-audience-sourcing.md)** para obter instruções de configuração passo a passo.

## Visão geral {#overview}

Use este fluxo de trabalho para originar e gerenciar públicos próprios diretamente de [!DNL Amazon S3]. Após a configuração, o Collaboration automaticamente origina públicos-alvo do seu bucket do S3 e os disponibiliza para insights e ativação.

Os públicos-alvo originados por meio do S3 seguem as mesmas regras de governança e manipulação de dados que os originados do Adobe Experience Platform.

## Pré-requisitos {#prerequisites}

Antes de configurar sua conexão de dados S3, verifique o seguinte:

* Você tem acesso a um **[!DNL Amazon S3]bucket** ativo contendo arquivos de público-alvo que estão em conformidade com a **[Especificação de Origem de Público-Alvo (v1.1)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.1.pdf)**.
* Você criou uma **função IAM** no AWS que concede à Adobe permissão para acessar seu bucket usando o método **função assumida** (não chaves de acesso/secretas). Consulte **[Configurar permissões do AWS para fornecimento de público-alvo](./configure-aws-permissions-audience-sourcing.md)** para obter instruções detalhadas. A função IAM deve incluir as seguintes permissões:

   * `ListBucket`
   * `GetBucketLocation`
   * `GetObject`

* Você tem os seguintes valores prontos:

   * **ARN (Nome do Recurso da Amazon) da função do IAM**
   * **Nome do bucket do S3**
   * **Caminho da pasta** (o prefixo do diretório que contém seus arquivos de público-alvo)

>[!NOTE]
>
>Os arquivos de público-alvo devem estar localizados no **caminho da pasta raiz** de seu bucket autorizado do S3. Não há suporte para estruturas de subpastas.

## Configurar sua conexão com o [!DNL Amazon S3] {#configure-aws-s3-connection}

Na guia **[!UICONTROL Meus públicos-alvo]** do espaço de trabalho **[!UICONTROL Configuração]**, selecione o ícone adicionar (![ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Público-alvo]**.

Se este for seu primeiro público-alvo, você também poderá selecionar a opção **[!UICONTROL Adicionar]**.

![A guia Meus públicos-alvo no espaço de trabalho de Instalação com o ícone Adicionar e a opção Adicionar público-alvo é exibida.](../../assets/setup/add-manage-audiences/add-audiences.png)

O fluxo de trabalho Adicionar público-alvo é exibido. Selecione **[!UICONTROL Adicionar nova conexão de dados]** e **[!UICONTROL Avançar]**.

![O espaço de trabalho Adicionar públicos-alvo com a opção Adicionar uma nova conexão de dados foi realçado.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### Selecione [!DNL Amazon S3] como conexão de dados {#select-aws-s3}

Selecione **[!UICONTROL Amazon S3]** como conexão de dados, seguido de **[!UICONTROL Próximo]**.

![A tela de seleção de conexão de dados com [!DNL Amazon S3] está disponível como uma opção selecionável.](../../assets/setup/aws-audience-sourcing/select-s3-data-connection.png)

### Revisar requisitos do arquivo de público-alvo {#review-audience-requirements}

Uma caixa de diálogo é exibida explicando como os arquivos de público-alvo devem ser estruturados. Use o link para a **[[!UICONTROL Especificação da Origem do Público-Alvo]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.1.pdf)** para saber como formatar e estruturar os dados do público-alvo do [!DNL Amazon S3] para o Collaboration para lê-los corretamente.

>[!IMPORTANT]
>
>Você deve ter autorizado o Adobe como um usuário [!DNL Amazon S3] para que o Adobe possa recuperar dados do armazenamento [!DNL Amazon S3] para processamento.

Os arquivos de público-alvo devem estar em conformidade com a Especificação de origem de público-alvo. As chaves de correspondência são mapeadas automaticamente com base no formato necessário.

As principais considerações incluem:

* Os arquivos devem estar no formato CSV, usando vírgulas como delimitadores e barras verticais (`|`) para vários valores.
* Se estiver fazendo upload de vários arquivos, verifique se todos os arquivos contêm colunas idênticas.
* Cada registro de público deve incluir um `AUDIENCE_ID` e pelo menos uma chave de correspondência, como `HASHED_EMAIL_SHA_256`, `HASHED_PHONE_SHA_256`, `HASHED_IPV4_SHA_256`, `CRM_ID`, `LOYALTY_ID` ou `ADFIXUS_ID`.
* As atualizações de dados ocorrem a cada 1-6 dias com base em sua seleção durante a configuração de origem no Collaboration.

![A caixa de diálogo Preparar seus Dados para Origem com um link para as Especificações de Origem do Público-Alvo.](../../assets/setup/aws-audience-sourcing/prepare-data-sourcing-dialog.png)

### Autentique sua conexão S3 {#authenticate-s3-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_sources_s3_folderpath"
>title="Formato do caminho da pasta"
>abstract="Insira o caminho da pasta (prefixo) no bucket do [!DNL Amazon S3] onde os arquivos de público-alvo estão armazenados.<br><ul><li>Não inicie caminhos com uma barra (/).</li><li>Inclua uma barra no final do caminho.</li><ul><br>Exemplo válido: `base/path/`<br>Exemplo inválido: `/base/path`"

Em seguida, forneça suas credenciais do [!DNL Amazon S3] para conectar seu bucket do S3 ao Collaboration.

Siga as etapas descritas em **[Configurar permissões do AWS para fornecimento de público-alvo](./configure-aws-permissions-audience-sourcing.md)** para conceder à Adobe acesso aos seus
Armazenamento [!DNL Amazon S3]. Depois de concluído, insira os valores nos seguintes campos da interface do usuário:

* Função do IAM
* Nome do balde do S3
* Caminho da pasta

![O formulário de conexão [!DNL Amazon S3] com campos da função IAM, Nome do Bucket do S3 e Caminho da Pasta.](../../assets/setup/aws-audience-sourcing/s3-authentication-credentials-form.png)

### Confirmar confirmação de consentimento {#confirm-consent}

Você deve reconhecer que as opções de recusa de consentimento foram removidas antes de continuar. Marque a caixa de confirmação seguida de **[!UICONTROL OK]** para confirmar.

![A caixa de diálogo de confirmação de recusa de consentimento requer confirmação antes de continuar.](../../assets/setup/aws-audience-sourcing/consent-optout-acknowledgment.png)

### Validar resultados de autenticação {#validate-authentication}

Após a conexão, o sistema valida suas credenciais e exibe uma das seguintes mensagens:

| Status | Mensagem | Descrição |
|---| ---|---|
| **Sucesso** | **[!UICONTROL Autenticação bem-sucedida]** | Sua conexão com [!DNL Amazon S3] foi estabelecida com êxito. |
| **Falha** | **[!UICONTROL Falha na autenticação]** | Revise suas credenciais e tente novamente. |
| **Acesso negado** | **[!UICONTROL Acesso negado]** | Suas credenciais não têm as permissões necessárias para acessar este bucket do [!DNL Amazon S3]. Verifique as configurações de acesso ou entre em contato com o administrador. |
| **Formato de arquivo inválido** | **[!UICONTROL Formato de arquivo inválido]** | Os dados do público-alvo não correspondem à estrutura esperada. Certifique-se de que seus arquivos estejam em conformidade com as Especificações de origem de público-alvo. |
| **Nenhum arquivo de público encontrado** | **[!UICONTROL Nenhum arquivo de público encontrado]** | Confirme se os arquivos de público-alvo existem no caminho de pasta especificado e se o caminho está acessível. |
| **Erro interno** | **[!UICONTROL Ocorreu um erro interno]** | Tente novamente. Se o problema persistir, entre em contato com o suporte ao cliente. |


### Fornecer detalhes da conexão {#provide-connection-details}

Insira um nome descritivo e uma descrição opcional para sua conexão de dados do S3. Insira seus valores nos seguintes campos da interface do usuário:

* **[!UICONTROL Nome da conexão de dados]** (obrigatório)
* **[!UICONTROL Descrição da conexão de dados]** (opcional)

![Formulário de detalhes da conexão de dados com campos para nome e descrição da conexão.](../../assets/setup/aws-audience-sourcing/s3-connection-name-description.png)

### Revisar campos de identidade mapeados automaticamente {#auto-mapped-fields}

A tela **[!UICONTROL Mapping]** é somente leitura. Não é possível adicionar, excluir ou aplicar transformações. O Collaboration mapeia automaticamente os campos de identidade de origem dos arquivos de público-alvo para os campos de destino com base na Especificação de origem do público-alvo.

Confirme visualmente os campos mapeados e selecione **[!UICONTROL Avançar]** para continuar.

![A tela de mapeamento de campos mostrando campos de identidade de origem e de destino mapeados automaticamente.](../../assets/setup/aws-audience-sourcing/s3-field-mapping-auto-mapped.png)

### Agendar intervalo de datas e frequência de atualização {#schedule-refresh}

A exibição **[!UICONTROL Agenda]** aparece. Use o menu suspenso para selecionar uma frequência de atualização entre um e seis dias e, em seguida, defina o intervalo de datas ativo. Use o ícone de calendário para especificar datas de início e término.

>[!IMPORTANT]
>
>Para gerenciar seus créditos do Collaboration com eficiência, defina a frequência de atualização para corresponder ou exceder a frequência de atualização de seus dados S3 subjacentes. O intervalo mínimo de atualização suportado é uma vez a cada seis dias.

![A tela de configurações de agendamento com opções de frequência de atualização e configuração de intervalo de datas.](../../assets/setup/aws-audience-sourcing/s3-schedule-refresh-frequency.png)

### Revisar e concluir a conexão {#review-and-complete}

Por fim, revise suas configurações na tela de resumo. Essa exibição contém um resumo das seguintes seções:

* **[!UICONTROL Conexão de dados]**: exibe a função IAM, o nome do bucket do S3 e o caminho de pasta que você configurou.
* **[!UICONTROL Detalhes]**: mostra o nome e a descrição opcional da sua conexão de dados para ajudar a identificá-la mais tarde.
* **[!UICONTROL Mapeamento]**: lista como os campos de origem dos arquivos de público-alvo carregados (por exemplo, `HASHED_EMAIL`) são mapeados para campos de destino usados no Collaboration (por exemplo, Email com hash).
* **[!UICONTROL Agendamento]**: resume a frequência com que a conexão atualiza os dados do público-alvo e o intervalo de datas ativo para fornecimento.

Selecione o ícone de lápis se precisar editar uma seção. Selecione **[!UICONTROL Concluir]** para confirmar todas as seções.

![A tela de resumo da revisão exibindo as seções de conexão de dados, detalhes, mapeamento e agendamento.](../../assets/setup/aws-audience-sourcing/s3-connection-review-summary.png)

Uma confirmação da caixa de diálogo é exibida informando que a conexão de dados foi criada com sucesso e que a origem do público-alvo está em andamento.

## Revisar públicos-alvo originados {#review-sourced-audiences}

Após concluir a configuração, o Collaboration começa a fornecer públicos-alvo a partir do seu bucket do S3. Os públicos-alvo provenientes de um bucket do [!DNL Amazon S3] aparecem na guia **[!UICONTROL Meus públicos-alvo]** e têm a mesma funcionalidade e as mesmas informações que os públicos-alvo provenientes da Experience Platform.

Se a origem do público-alvo estiver em andamento, um banner será exibido na parte superior da tela. Públicos-alvo individuais aparecem somente após a conclusão da origem.

![A guia Públicos-alvo mostrando que a origem está em andamento para [!DNL Amazon S3] públicos-alvo.](../../assets/setup/aws-audience-sourcing/s3-audiences-sourcing-in-progress.png)

Depois que os públicos-alvo do S3 forem originados, a lista de públicos-alvo disponíveis será fornecida em uma visualização tabulada ou de cartão.

>[!TIP]
>
>O tempo de fornecimento do público-alvo varia de acordo com o tamanho dos dados do S3 e a frequência de atualização configurada. Conjuntos de dados maiores ou agendamentos de atualização menos frequentes podem levar mais tempo para serem exibidos no espaço de trabalho **[!UICONTROL Meus públicos]**.

![A guia Públicos-alvo exibindo uma lista tabulada de públicos-alvo de origem.](../../assets/setup/aws-audience-sourcing/s3-audiences-list-view.png)

Quando estiver na exibição de grade ou tabela, selecione um item de linha ou **[!UICONTROL Exibir público-alvo]** para ter uma visão geral de um público-alvo específico. Ele exibe o status, a origem e o nome da conexão de dados do público-alvo, juntamente com painéis detalhados para:

**[!UICONTROL Identidades]**: mostra a contagem e o detalhamento totais de identidades assim que os dados são disponibilizados.
**[!UICONTROL Categorias]**: lista todas as marcas usadas para organizar ou filtrar o público.
**[!UICONTROL Acesso à conexão]**: indica se o público é privado, público ou compartilhado com colaboradores específicos.
**[!UICONTROL Visibilidade de metadados]**: define quais informações de público-alvo (como contagem de identidade, porcentagem de sobreposição e índice) estão visíveis para os colaboradores.

Use esta exibição para confirmar as configurações de público-alvo e as configurações de visibilidade antes de usar o público-alvo em projetos de colaboração.

Consulte a [Exibir documentação do painel de públicos-alvo](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#view-audiences-dashboard) para saber mais.

## Exibir sua conexão de dados S3 {#view-s3-connection}

Sua conexão [!DNL Amazon S3] recém-adicionada está imediatamente disponível na guia **[!UICONTROL Minhas conexões de dados]**. A origem do público é exibida como [!UICONTROL Amazon S3].

Sua conexão de dados do S3 inclui a mesma funcionalidade e detalhes de outras conexões de dados de público-alvo, exceto que você não pode adicionar ou editar públicos-alvo diretamente desta exibição.

>[!NOTE]
>
>[!DNL Amazon S3] conexões de dados não são editáveis. Não é possível modificar configurações como a frequência de atualização depois que a conexão é criada. Para atualizar a configuração, você deve excluir a conexão existente e criar uma nova.

![A guia Minhas conexões de dados mostrando a conexão de dados [!DNL Amazon S3] com informações de status de fornecimento.](../../assets/setup/aws-audience-sourcing/s3-data-connections-tab.png)

## Próximas etapas {#next-steps}

Agora você configurou e conectou com êxito o armazenamento do [!DNL Amazon S3] como fonte de dados no Collaboration. Ao concluir esse fluxo de trabalho, você ativou a origem segura de dados de público-alvo primários para ativação e análise de sobreposição.

Após a conclusão da origem, seus públicos-alvo aparecem no espaço de trabalho **[!UICONTROL Meus públicos-alvo]**, prontos para colaboração e ativação. Para obter opções de gerenciamento detalhadas, consulte a [documentação sobre gerenciamento de públicos-alvo](./onboard-audiences.md).
