---
title: Configurar [!DNL Snowflake] para Origem de Público-Alvo
description: Saiba como configurar e conectar o  [!DNL Snowflake Secure Data Share]  como uma fonte de dados de autoatendimento para assimilar dados de público-alvo no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 517a28afc83b0e1b4a9e64fa53eb90e0ad5541e9
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 1%

---

# Configurar [!DNL Snowflake] para fornecimento de público

Saiba como configurar e conectar seu [!DNL Snowflake Secure Data Share] na interface do usuário do Adobe Real-Time CDP Collaboration aos dados de público-alvo de origem para ativação e análise de sobreposição.

## Visão geral {#overview}

[!DNL Snowflake] é uma das opções com suporte para fornecer dados de público-alvo primário no Collaboration. Outros métodos disponíveis incluem o fornecimento de públicos do [Experience Platform](./onboard-audiences.md), a conexão de um [[!DNL AWS S3] bucket](./configure-aws-s3-audience-sourcing.md) ou o upload de um [arquivo CSV](./upload-csv-audience-sourcing.md).

Siga as etapas abaixo para conectar seu [!DNL Snowflake Secure Data Share] e originar seus dados de público-alvo no Collaboration. Depois que a configuração for concluída, você poderá revisar, ativar e gerenciar os públicos-alvo originados para os projetos de colaboração.

## Pré-requisitos {#prerequisites}

Antes de configurar a conexão do [!DNL Snowflake], verifique se você atende aos seguintes pré-requisitos:

* Você criou um [!DNL Snowflake Share] e configurou as permissões necessárias em sua conta [!DNL Snowflake] para conceder à Adobe acesso a seu [!DNL Snowflake Secure Data Share].
* Você tem os seguintes [!DNL Snowflake Share] valores prontos:

   * **Nome do compartilhamento**
   * **Identificador da conta**
   * **Esquema**
   * **Exibir**

* Os dados de público-alvo em seu [!DNL Snowflake Secure Data Share] devem atender aos requisitos de formato descritos no guia de [Especificação de Origem de Público-Alvo (v1.2)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf).
* Todas as chaves de correspondência no arquivo de público-alvo [!DNL Snowflake] também devem ser habilitadas para a conta do Collaboration. Saiba como [habilitar chaves de correspondência](./onboard-account.md#set-up-match-keys) ou [adicionar novas chaves de correspondência](./onboard-account.md#edit-match-keys) à sua conta.

## Configurar sua conexão com o [!DNL Snowflake] {#configure-snowflake-connection}

Na guia **[!UICONTROL Meus públicos-alvo]** do espaço de trabalho **[!UICONTROL Configuração]**, selecione o ícone adicionar (![Ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Público]**.

Se este for seu primeiro público-alvo, você também poderá selecionar a opção **[!UICONTROL Adicionar público-alvo]**.

![A guia Meus públicos-alvo no espaço de trabalho de Instalação com o ícone Adicionar e a opção Adicionar público-alvo é exibida.](../../assets/setup/snowflake-audience-sourcing/add-audience.png)

O fluxo de trabalho Adicionar público-alvo é exibido. Selecione **[!UICONTROL Adicionar nova conexão de dados]** e **[!UICONTROL Avançar]**.

![O espaço de trabalho Adicionar públicos-alvo com a opção Adicionar uma nova conexão de dados foi realçado.](../../assets/setup/snowflake-audience-sourcing/add-data-connection.png){zoomable="yes"}

### Selecione [!DNL Snowflake] como conexão de dados {#select-snowflake}

Em seguida, selecione **[!UICONTROL Snowflake]** como conexão de dados, seguido de **[!UICONTROL Próximo]**.

![A tela de seleção de conexão de dados com [!DNL Snowflake] está disponível como uma opção selecionável.](../../assets/setup/snowflake-audience-sourcing/select-snowflake-data-connection.png)

### Revisar arquivo de público {#review-audience-file}

Uma caixa de diálogo é exibida, explicando os requisitos do arquivo de público-alvo [!DNL Snowflake Share] e [!DNL Snowflake] antes de você começar a fornecer. Verifique se o [!DNL Snowflake Share] foi criado com o nome de compartilhamento, identificador de conta, esquema e exibição corretos. Para confirmar se os dados do público-alvo estão formatados e estruturados corretamente para uso no Collaboration, revise o guia **[[!UICONTROL Especificação da origem do público-alvo]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)**.

Depois de concluído, selecione **[!UICONTROL Iniciar integração]**.

![Prepare seu [!DNL Snowflake Share] para a caixa de diálogo de integração com um link para as Especificações de Fornecimento de Público-Alvo.](../../assets/setup/snowflake-audience-sourcing/prepare-snowflake-share-onboarding-dialog.png)

### Autenticar conexão [!DNL Snowflake Share] {#authenticate-snowflake-share-connection}

Nesta etapa, você precisa fornecer as credenciais do [!DNL Snowflake Share] necessárias para conectar o [!DNL Snowflake Share] ao Collaboration:

| Campo | Descrição | Exemplo |
|--------------------|-------------|------------------------------|
| Nome do compartilhamento | O nome de seu [!DNL Snowflake Share]. | `ADOBE_DATA_SHARE` |
| Identificador da conta | O identificador exclusivo da sua conta da Snowflake. | `CUSTOMER_ORG.CUSTOMER_SNOWFLAKE_ACCOUNT` |
| Esquema | O esquema em seu [!DNL Snowflake Share] que contém seus dados de público-alvo. | `CUSTOMER_SCHEMA` |
| Exibir | O conjunto de dados real que o Collaboration extrai de dados de público-alvo. | `SECURE_VIEW_FOR_ADOBE` |

{style="table-layout:auto"}

Depois de inserir todas as credenciais necessárias, selecione **[!UICONTROL Avançar]**.

![O formulário de conexão [!DNL Snowflake Share] com os campos Nome do compartilhamento, Identificador da conta, Esquema e Exibição foi preenchido, e o botão Avançar foi realçado.](../../assets/setup/snowflake-audience-sourcing/snowflake-authentication-credentials-form.png)

Uma caixa de diálogo de confirmação é exibida na parte inferior da próxima página, confirmando que o [!DNL Snowflake Share] foi conectado com êxito ao Collaboration.

![Uma caixa de diálogo de confirmação confirma que a conexão [!DNL Snowflake Share] foi estabelecida com êxito.](../../assets/setup/snowflake-audience-sourcing/snowflake-share-connection-established.png)

### Fornecer nome e descrição {#provide-name-description}

No modo de exibição **[!UICONTROL Fornecer detalhes]**, insira um nome descritivo e uma descrição opcional para sua conexão de dados [!DNL Snowflake]. Quando terminar, selecione **[!UICONTROL Próximo]**.

![A tela Fornecer detalhes exibe o nome e a descrição da conexão de dados, com o botão Avançar realçado.](../../assets/setup/snowflake-audience-sourcing/provide-name-description.png)

### Mapear campos {#map-fields}

A tela **[!UICONTROL Mapping]** é somente leitura neste momento. Não é possível adicionar, excluir ou aplicar transformações. O Collaboration mapeia automaticamente os campos de identidade de origem dos seus dados do [!DNL Snowflake Share] para campos de destino com base na **[Especificação da origem do público-alvo (v1.2)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)**.

Confirme visualmente os campos mapeados e selecione **[!UICONTROL Avançar]** para continuar. Você também pode visualizar dados de amostra do seu [!DNL Snowflake Share] com a opção **[!UICONTROL Visualizar dados de origem]**.

![A tela Mapear campos exibe os campos de origem e destino mapeados automaticamente, com as opções Visualizar dados de origem e Avançar realçadas.](../../assets/setup/snowflake-audience-sourcing/map-fields-screen.png)

Quando você opta por visualizar, a caixa de diálogo **[!UICONTROL [!DNL Snowflake Share]visualização de dados]** é exibida com dados de exemplo exibidos em formato de tabela. Revise isso e selecione **[!UICONTROL Fechar]**.

A caixa de diálogo de visualização de dados do ![[!DNL Snowflake Share] mostra os dados de exemplo do [!DNL Snowflake Share] e a opção Fechar realçada.](../../assets/setup/snowflake-audience-sourcing/preview-source-data.png)

<!-- NOTE: Manual mapping will be available in the future. -->
<!-- In the **[!UICONTROL Map fields]** screen, you can use the **[!UICONTROL Source field]** and **[!UICONTROL Target field]** dropdowns to update the auto-mapped fields, or include additional fields with the **[!UICONTROL Add field]** option. Once finished, select **[!UICONTROL Next]**. -->

<!-- ![The Map fields screen showing the mapped fields with the Next option highlighted.](../../assets/setup/snowflake-audience-sourcing/map-fields.png) -->

### Agendar intervalo de datas e frequência de atualização {#refresh-frequency-date-range}

Em seguida, no modo de exibição **[!UICONTROL Agendar]**, use o menu suspenso para selecionar a frequência de atualização entre um e seis dias. Em seguida, use o ícone de calendário para especificar datas de início e término para o público-alvo de origem.

>[!IMPORTANT]
>
>Para gerenciar seus créditos do Collaboration com eficiência, defina a frequência de atualização para corresponder ou não exceder a frequência de atualização de seus dados [!DNL Snowflake] subjacentes. O intervalo mínimo de atualização suportado é uma vez a cada seis dias.

![A tela Agendar realça a frequência de atualização, as configurações de intervalo de datas e a opção Avançar.](../../assets/setup/snowflake-audience-sourcing/refresh-frequency-date-range.png)

### Revisar e concluir a conexão {#review-and-complete}

Por fim, revise suas configurações na tela de resumo. Essa exibição contém um resumo das seguintes seções:

* **[!UICONTROL Conexão de dados]**: exibe o nome do compartilhamento, o identificador da conta, o esquema e a exibição de seu [!DNL Snowflake Share].
* **[!UICONTROL Detalhes]**: exibe o nome e a descrição opcional da sua conexão de dados para ajudar a identificá-la mais tarde.
* **[!UICONTROL Mapeamento]**: mostra como os campos de origem do seu arquivo de público-alvo são mapeados para campos de destino usados no Collaboration.
* **[!UICONTROL Agendar]**: mostra a frequência com que a conexão atualiza os dados do público-alvo e o intervalo de datas ativo para fornecimento.

Selecione o ícone de lápis (![Ícone Editar](/help/assets/icons/edit.png)) se precisar editar uma seção. Selecione **[!UICONTROL Concluir]** para confirmar todas as seções.

![A tela Revisão exibe um resumo das configurações de conexão de dados, detalhes, mapeamento e agendamento, com a opção Concluído realçada.](../../assets/setup/snowflake-audience-sourcing/review-settings.png)

Uma caixa de diálogo de confirmação confirma que a conexão de dados foi criada com sucesso e a origem do público-alvo está em andamento.

## Revisar públicos-alvo originados {#review-sourced-audiences}

Após a conclusão da instalação, a Collaboration começa a fornecer públicos-alvo do seu [!DNL Snowflake Share]. Se o fornecimento do público-alvo estiver em andamento, um banner será exibido na parte superior da exibição.

![A guia Meus públicos-alvo mostra o banner Fonte de público-alvo em andamento.](../../assets/setup/snowflake-audience-sourcing/audience-sourcing-in-progress.png)

>[!TIP]
>
>O tempo de fornecimento do público-alvo varia de acordo com o tamanho dos dados do [!DNL Snowflake] e a frequência de atualização configurada. Conjuntos de dados maiores ou agendamentos de atualização menos frequentes podem levar mais tempo para serem exibidos no espaço de trabalho **[!UICONTROL Meus públicos]**.

Quando o fornecimento for concluído, seus públicos-alvo estarão disponíveis na guia **[!UICONTROL Meus públicos-alvo]** com os mesmos recursos e informações que os públicos-alvo provenientes da Experience Platform.

![A guia Meus públicos-alvo mostra uma lista de públicos-alvo originados na exibição em tabelas.](../../assets/setup/snowflake-audience-sourcing/snowflake-audience-list.png)

Quando estiver na exibição de grade ou tabela, selecione um item de linha ou **[!UICONTROL Exibir público-alvo]** para ter uma visão geral de um público-alvo específico. Ele exibe o status do público-alvo, a origem e o nome da conexão de dados, juntamente com painéis detalhados para **[!UICONTROL Identidades]**, **[!UICONTROL Categorias]**, **[!UICONTROL Acesso à conexão]** e **[!UICONTROL Visibilidade de metadados]**. Consulte [como exibir um público-alvo individual](./onboard-audiences.md#view-individual-audiences) para obter detalhes.

Use esta exibição para confirmar as configurações de público-alvo e as configurações de visibilidade antes de usar o público-alvo em projetos de colaboração.

## Exibir sua conexão de dados do [!DNL Snowflake] {#view-snowflake-connection}

Sua conexão [!DNL Snowflake] recém-adicionada está imediatamente disponível na guia **[!UICONTROL Minhas conexões de dados]**. A origem do público é exibida como [!UICONTROL [!DNL Snowflake]].

Sua conexão de dados do [!DNL Snowflake] inclui a mesma funcionalidade e os mesmos detalhes de outras conexões de dados de público-alvo. Saiba mais sobre [como exibir e gerenciar conexões de dados](../setup/manage-data-connection.md).

![A guia Minhas conexões de dados mostra a conexão de dados [!DNL Snowflake] com as informações de status de fornecimento.](../../assets/setup/snowflake-audience-sourcing/data-connection-tab-snowflake.png)

## Próximas etapas {#next-steps}

Agora você configurou e conectou com êxito o [!DNL Snowflake] como fonte de dados no Collaboration. Após a conclusão do fornecimento, você pode [criar projetos de colaboração](../collaborate/manage-projects.md), [ativar públicos-alvo](../collaborate/activate.md), [revisar sobreposições e insights](../collaborate/measure.md) e [gerenciar as configurações e a visibilidade do público-alvo](./onboard-audiences.md).

Para obter informações sobre outros métodos de fornecimento de público, consulte as seguintes documentações:

* [Configurar [!DNL Amazon S3] para fornecimento de público](./configure-aws-s3-audience-sourcing.md)
* [Públicos-alvo da Source no Experience Platform](./onboard-audiences.md)
* [Fazer upload de arquivo CSV para fornecimento de público](./upload-csv-audience-sourcing.md)
