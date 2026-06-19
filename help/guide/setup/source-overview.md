---
title: Visão geral das fontes
description: Saiba mais sobre conectores de origem no Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
source-git-commit: b30d1b01e929e586404faac34650c7fd479d071b
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 6%

---

# Visão geral das fontes

No Adobe Real-Time CDP Collaboration, uma fonte (ou conexão de dados) é de onde os dados do público-alvo vêm. Você pode se conectar a vários tipos de origem, como aplicativos Adobe, armazenamentos na nuvem ou arquivos do seu sistema local, para [originar e gerenciar públicos](./onboard-audiences.md) para seus projetos Collaboration. Durante o fluxo de trabalho de fornecimento de público, você pode escolher e configurar sua origem preferida com base nas necessidades da organização.

## Conectar uma origem {#connect-a-source}

Para conectar uma origem, você precisa informar o workflow de seleção de fornecedor. Primeiro, navegue até a guia **[!UICONTROL Meus públicos-alvo]** no espaço de trabalho **[!UICONTROL Instalação]**.

Selecione o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Público-alvo]** para iniciar o fluxo de trabalho de origem.

![Meu espaço de trabalho de públicos-alvo com a opção Adicionar e a opção Públicos-alvo realçadas.](/help/assets/setup/add-manage-audiences/add-audiences.png)

Durante o fluxo de trabalho, você será solicitado a adicionar uma nova conexão de dados selecionando uma origem. A fonte escolhida determina como os dados do público-alvo são trazidos para o Collaboration. Consulte a tabela [fontes disponíveis](#available-sources) para obter uma lista de todas as fontes com suporte.

![O espaço de trabalho Adicionar públicos-alvo com a opção Adicionar uma nova conexão de dados foi realçado.](/help/assets/setup/add-manage-audiences/add-data-connection.png)

Depois de selecionar uma origem, o fluxo de trabalho orienta você pelas etapas de configuração específicas da conexão, incluindo autenticação, mapeamento de campo, agendamento e seleção de público-alvo.

### Fontes disponíveis {#available-sources}

As fontes a seguir estão disponíveis no Collaboration. Para exibir o guia de seleção de fornecedor passo a passo para essa origem, selecione o nome da origem na tabela abaixo. Se você estiver interessado em uma fonte que não está disponível no momento, entre em contato com o representante da Adobe.

| Fonte | Descrição | Disponibilidade |
| --- | --- | --- |
| [Adobe Experience Platform](./onboard-audiences.md) | Traga públicos-alvo da instância conectada do Experience Platform e reutilize os segmentos de clientes existentes. | Disponível |
| [Amazon S3](./configure-aws-s3-audience-sourcing.md) | Conecte seus buckets do S3 para obter grandes conjuntos de dados primários a partir de sua infraestrutura de nuvem. | Disponível |
| [[!DNL Snowflake]](./configure-snowflake-audience-sourcing.md) | Conecte seu [!DNL Snowflake Secure Data Share] para trazer conjuntos de dados de público-alvo em larga escala. | Disponível |
| [[!DNL Google Cloud Storage]](./configure-gcs-audience-sourcing.md) | Conecte seus buckets do GCS para trazer os dados de público-alvo armazenados em seu ambiente [!DNL Google Cloud]. | Disponível |
| [Carregamento de arquivo CSV](./upload-csv-audience-sourcing.md) | Carregue um arquivo CSV formatado diretamente do sistema local. | Disponível |
| Adobe Audience Manager | Traga segmentos existentes do Audience Manager para seus projetos do Collaboration. | *Em breve* |
| [[!DNL Azure Blob Storage]](./configure-azure-storage-audience-sourcing.md) | Conecte seus contêineres do [!DNL Azure Blob Storage] aos conjuntos de dados primários de origem do seu ambiente do [!DNL Microsoft Azure]. | Disponível |
| [[!DNL Azure Data Lake Storage]](./configure-azure-storage-audience-sourcing.md) | Conecte sua conta do [!DNL Azure Data Lake Storage Gen 2] para trazer os dados de público-alvo armazenados em seu data lake do [!DNL Azure]. | Disponível |

{style="table-layout:auto"}

## Próximas etapas

Depois de conectar uma origem e trazer seus públicos-alvo, você pode exibir detalhes, atualizar configurações ou excluir fontes existentes. Para obter mais informações, consulte o guia [Gerenciar conexões de dados](./manage-data-connection.md).
