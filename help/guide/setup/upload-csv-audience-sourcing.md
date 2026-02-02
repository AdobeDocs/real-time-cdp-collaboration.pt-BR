---
title: Fazer upload de arquivo CSV para origem de público-alvo
description: Saiba como fazer upload do arquivo CSV como uma fonte de dados de autoatendimento para assimilar dados de público-alvo no Real-Time CDP Collaboration.
source-git-commit: 96d3f87cedcfde73ce01c2b53c0b2ce4365fd277
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# Fazer upload de arquivo CSV para fornecimento de público

Este guia fornece etapas para fazer upload de um arquivo CSV na interface do usuário do Adobe Real-Time CDP Collaboration a fim de obter os dados do público-alvo para uso em projetos de colaboração.

## Visão geral {#overview}

O upload de arquivos CSV é um método para fornecer dados de público-alvo primários para projetos de colaboração. Esta é uma alternativa para [conectar seu bucket do AWS S3](./configure-aws-s3-audience-sourcing.md) ou [fornecer públicos-alvo do Experience Platform](./onboard-audiences.md).

Siga este fluxo de trabalho para fazer upload de um arquivo CSV contendo os dados do público-alvo para fornecer e gerenciar públicos-alvo primários no Collaboration. É possível mapear campos de identidade para ativação e análise de sobreposição. Depois que o arquivo é carregado e processado, o público-alvo de origem fica disponível no espaço de trabalho **[!UICONTROL Meus públicos-alvo]**, onde você pode revisar, ativar e gerenciar seus projetos de colaboração.

>[!IMPORTANT]
>
>* Os públicos-alvo originados por meio do upload de CSV estão disponíveis por **7 dias**. Após esse período, o público-alvo expira e deve ser recarregado para uso em seus projetos de colaboração.
>
>* Agora, é possível carregar um arquivo CSV por sessão. Para adicionar outros públicos-alvo, conclua o fluxo de trabalho de upload novamente para cada arquivo que deseja originar.

## Pré-requisitos {#prerequisites}

Antes de carregar arquivos CSV para fornecimento de público, verifique se você tem:

* Integração de conta concluída no Real-Time CDP Collaboration. Consulte [Integrar sua conta](./onboard-account.md) para obter instruções passo a passo.
* As permissões necessárias para adicionar públicos-alvo na organização.
* Um arquivo CSV que contém os dados do público-alvo com campos de identidade como email ou telefone.

## Fazer upload de um arquivo CSV {#upload-csv-file}

Na guia **[!UICONTROL Meus públicos-alvo]** do espaço de trabalho **[!UICONTROL Configuração]**, selecione o ícone adicionar (![ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Público-alvo]**.

Se este for seu primeiro público-alvo, você também poderá selecionar a opção **[!UICONTROL Adicionar]**.

![A guia Meus públicos-alvo no espaço de trabalho de Instalação com o ícone Adicionar e a opção Adicionar público-alvo é exibida.](../../assets/setup/add-manage-audiences/add-audiences.png)

O fluxo de trabalho Adicionar público-alvo é exibido. Selecione **[!UICONTROL Adicionar nova conexão de dados]** e **[!UICONTROL Avançar]**.

![O espaço de trabalho Adicionar públicos-alvo com a opção Adicionar uma nova conexão de dados foi realçado.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### Selecione Arquivo CSV como a conexão de dados {#select-csv-file}

Selecione **[!UICONTROL Arquivo CSV]** como uma conexão de dados, seguido por **[!UICONTROL Próximo]**.

![A tela de seleção de conexão de dados com o Arquivo CSV está disponível como uma opção selecionável.](../../assets/setup/csv-audience-sourcing/select-csv-data-connection.png)

### Selecionar arquivo {#select-file}

Escolha **[!UICONTROL Selecionar do computador]** para carregar um arquivo CSV do sistema local. Como alternativa, você pode arrastar e soltar o arquivo CSV que deseja carregar no painel [!UICONTROL Arrastar e soltar um arquivo CSV].

>[!IMPORTANT]
>
>Somente arquivos CSV são suportados. O tamanho máximo do arquivo é **2 GB**.

![Selecione um arquivo CSV contendo dados de público-alvo do seu sistema local.](../../assets/setup/csv-audience-sourcing/select-file.png)

Depois de carregada, a interface mostra um resumo que inclui o número de colunas, uma contagem de linhas estimada, a estrutura do arquivo e uma pré-visualização das primeiras 10 linhas de dados.

Revise o resumo e selecione **[!UICONTROL Próximo]**.

![Visualize os dados de público-alvo de exemplo a partir do seu arquivo CSV.](../../assets/setup/csv-audience-sourcing/preview-sample-data.png)

#### Substituir arquivo {#replace-file}

Se precisar carregar um arquivo CSV diferente, escolha **[!UICONTROL Substituir arquivo]** e selecione seu novo arquivo. A interface é atualizada para exibir um resumo atualizado dos novos dados.

Depois de revisar o resumo revisado, selecione **[!UICONTROL Próximo]**.

![Selecione a opção Substituir arquivo para carregar outro arquivo CSV.](../../assets/setup/csv-audience-sourcing/replace-file.png)

### Confirmar confirmação de consentimento {#confirm-consent}

Antes de continuar, você deve reconhecer que as opções de recusa de consentimento foram removidas dos dados do público-alvo. O Collaboration exige dados limpos do público-alvo sem usuários que recusaram o compartilhamento de dados.

Marque a caixa de confirmação seguida de **[!UICONTROL OK]** para confirmar. A caixa de diálogo é fechada e você prossegue para a tela Mapear campos.

![A caixa de diálogo de confirmação de recusa de consentimento requer confirmação antes de continuar.](../../assets/setup/csv-audience-sourcing/consent-optout-acknowledgment.png)

### Mapear campos de identidade de origem {#map-fields}

O mapeamento de campo determina como o Collaboration usa os dados do público-alvo para ativação e análise de sobreposição. Na tela **[!UICONTROL Mapear campos]**, use os menus suspensos para mapear cada campo de identidade de origem do seu arquivo CSV para o campo de destino apropriado no Collaboration.

Se você precisar de detalhes adicionais sobre um campo de destino, incluindo o tipo de dados ou a descrição, selecione **[!UICONTROL Detalhes dos campos de destino]** para obter mais informações.

![A lista suspensa para mapear um campo de identidade de origem a partir dos dados de público-alvo em formato CSV para o campo de destino no Collaboration.](../../assets/setup/csv-audience-sourcing/map-fields.png)

Em seguida, revise os campos mapeados e selecione **[!UICONTROL Avançar]**.

![A tela de mapeamento de campos mostrando os campos de identidade de origem e destino mapeados.](../../assets/setup/csv-audience-sourcing/confirm-mapped-fields.png)

### Revisar e concluir o upload {#review-and-complete}

A tela **[!UICONTROL Avaliação]** é exibida com um resumo das configurações de público-alvo do seu arquivo CSV. Revise as informações nas seguintes seções:

* **[!UICONTROL Informações do Arquivo]**: Exibe o nome do arquivo, o número de colunas e a contagem estimada de linhas.
* **[!UICONTROL Mapeamento]**: lista como os campos de origem do seu arquivo de público-alvo carregado (por exemplo, `email`) são mapeados para campos de destino usados no Collaboration (por exemplo, Email com hash).

Selecione o ícone de lápis se precisar editar uma seção. Selecione **[!UICONTROL Concluir]** para confirmar todas as seções.

![Revise o resumo das configurações de carregamento, incluindo informações de arquivo CSV e detalhes de mapeamento de campo.](../../assets/setup/csv-audience-sourcing/review-upload-summary.png)

Uma barra de progresso é exibida abaixo das seções de resumo para indicar o progresso do upload. Depois que o upload for concluído, uma caixa de diálogo de confirmação confirmará que o público-alvo de CSV foi criado e a origem do público-alvo está em andamento.

![Após o carregamento do arquivo, é exibida uma caixa de diálogo de confirmação informando que o público-alvo CSV foi criado e que a origem do público-alvo está em andamento.](../../assets/setup/csv-audience-sourcing/upload-success-sourcing-in-progress.png)

## Revisar públicos-alvo originados {#review-sourced-audiences}

Depois de fazer upload do arquivo CSV, o Collaboration começa a fornecer públicos-alvo do arquivo. Esse processo pode levar vários minutos. Quando o fornecimento for concluído, seus públicos-alvo estarão disponíveis na guia **[!UICONTROL Meus públicos-alvo]** com os mesmos recursos e informações que os públicos-alvo provenientes da Experience Platform.

![A guia Públicos-alvo mostrando uma lista de públicos-alvo originados na exibição de grade.](../../assets/setup/csv-audience-sourcing/csv-audiences-list.png)

Quando estiver na exibição de grade ou tabela, selecione um item de linha ou **[!UICONTROL Exibir público-alvo]** para ter uma visão geral de um público-alvo específico. Ele exibe o status, a origem e o nome da conexão de dados do público-alvo, juntamente com painéis detalhados para:

**[!UICONTROL Identidades]**: exibe a contagem e o detalhamento totais de identidades assim que os dados são disponibilizados.
**[!UICONTROL Categorias]**: exibe as marcas usadas para organizar ou filtrar o público.
**[!UICONTROL Acesso à conexão]**: exibe se o público é privado, público ou compartilhado com colaboradores específicos.
**[!UICONTROL Visibilidade de metadados]**: mostra quais informações de público-alvo (como contagem de identidades, porcentagem de sobreposição e índice) estão visíveis para os colaboradores.

Use esta exibição para confirmar as configurações de público-alvo e as configurações de visibilidade antes de usar o público-alvo em projetos de colaboração. Para obter mais informações, consulte [como visualizar um público-alvo individual](./onboard-audiences.md#view-individual-audiences).

## Próximas etapas {#next-steps}

Agora você carregou com êxito seu arquivo CSV no Collaboration. Após a conclusão da seleção de fornecedor, você pode:

* Crie projetos de colaboração com os públicos-alvo de origem. Consulte [Descobrir públicos-alvo](../../guide/collaborate/discover.md).
* Ative públicos para destinos conectados. Consulte [Ativar públicos-alvo](../../guide/collaborate/activate.md).
* Analise a sobreposição de público e os insights. Consulte [Medir o desempenho da campanha](../../guide/collaborate/measure.md).
* Gerencie as configurações e a visibilidade do seu público-alvo. Consulte [Source e gerenciar públicos](./onboard-audiences.md).

Para obter informações sobre outros métodos de fornecimento de público, consulte [Configurar o AWS S3 para fornecimento de público](./configure-aws-s3-audience-sourcing.md) ou [Públicos-alvo da Source na Experience Platform](./onboard-audiences.md).
