---
title: Rastrear sua atividade de consumo de crédito
description: Saiba como rastrear a atividade de consumo de crédito da sua organização no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: 4fc9b4e814f7392e1dfdb5847b7189d7d6e21702
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 6%

---

# Rastrear sua atividade de consumo de crédito {#track-credit-consumption-activity}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_my_activity"
>title="Saiba mais"
>abstract=""

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**Período Sem Excedente de 90 Dias**: os clientes em regiões qualificadas se beneficiam de um período sem excedente de 90 dias a partir da data de disponibilidade em sua região. Durante esse período, os clientes não incorrem em taxas de excedente por exceder seus direitos de crédito.

>[!ENDSHADEBOX]

>[!IMPORTANT]
>
>A tabela de consumo de crédito é arredondada e agregada por dia para monitoramento. Os números no painel **[!UICONTROL Minha atividade]** representam um consumo de crédito *estimado*. O consumo de crédito *real* usado para cobrança é rastreado em sistemas internos e está disponível mediante solicitação. Entre em contato com o representante da Adobe para obter essas informações.

Para acessar sua atividade de consumo de crédito estimado, navegue até **[!UICONTROL Configuração]** na navegação principal e selecione a guia **[!UICONTROL Minha atividade]**.

![Painel Minha Atividade mostrando detalhes do consumo de crédito](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>A exibição **[!UICONTROL Minha atividade]** não inclui informações sobre ações do usuário em diferentes partes da interface do usuário do Collaboration. Use a funcionalidade [logs de auditoria](/help/guide/setup/audit-logs.md) para obter essas informações.

## Entender o painel de atividades {#understand-dashboard}

O painel de atividade exibe uma lista abrangente de todas as operações de consumo de crédito na conta. Cada linha representa uma atividade distinta e fornece informações importantes sobre o uso do crédito:

>[!NOTE]
>
>As atividades de **[!UICONTROL Gerenciamento de Público-Alvo]** não estão associadas a outro colaborador, portanto, as colunas **[!UICONTROL ID da Conexão]** e **[!UICONTROL Nome da Conexão]** para esses tipos de atividades indicam um valor de **[!UICONTROL -]**.

| Coluna | Descrição |
|------------|--------------|
| **[!UICONTROL Data]** | A data em que a atividade ocorreu, exibida no formato MM/DD/AAAA. |
| **[!UICONTROL ID da Conexão]** | Um identificador exclusivo para cada conexão associada a uma atividade de consumo de crédito, representada como uma sequência alfanumérica. |
| **[!UICONTROL Nome da conexão]** | O nome do colaborador associado à conexão e à atividade que consome crédito. |
| **[!UICONTROL Atividade]** | O tipo de atividade realizada, como **Ativação - Correspondência**, **Ativação - Saída** ou **Gerenciamento de Público-Alvo**. |
| **[!UICONTROL Entradas processadas]** | O número total de entradas (por exemplo, IDs ou linhas) processadas para a atividade. |
| **[!UICONTROL Total de créditos usados]** | O número total de créditos consumidos pela atividade. |
| **[!UICONTROL Meu compartilhamento de crédito]** | A parte da sua conta dos créditos usados para a atividade. |

{style="table-layout:auto"}

## Tipos de atividades {#types-of-activities}

A coluna **[!UICONTROL Atividade]** mostra diferentes tipos de operações que consomem crédito.

* **[!UICONTROL Gerenciamento de público-alvo]**: os créditos são consumidos quando os públicos-alvo são originados na Collaboration. Os créditos são consumidos como uma função do número de IDs (em milhões) indexadas no Collaboration em todos os públicos-alvo e da frequência dessa indexação (diariamente, a cada três dias ou semanalmente). Para saber mais, leia o [guia de fornecimento e gerenciamento de públicos-alvo](/help/guide/setup/onboard-audiences.md).
* **[!UICONTROL Ativação - Correspondente]** - Os créditos são consumidos como uma função do número de IDs correspondentes e preparadas para ativação. Para saber mais, leia o [guia de ativação de públicos-alvo](/help/guide/collaborate/activate.md).
* **[!UICONTROL Ativação - Saída]** - Os créditos são consumidos como uma função do número de IDs enviadas para um destino. Isso é sempre cobrado do colaborador que recebe o público-alvo. Para saber mais, leia o [guia de ativação de públicos-alvo](/help/guide/collaborate/activate.md).
* **[!UICONTROL Medição]** - Execute atividades no Collaboration para gerar relatórios e insights de desempenho da campanha. Os créditos são consumidos com base no número de linhas nos relatórios de campanha em todas as campanhas e na frequência dos relatórios (diariamente, a cada três dias ou semanalmente).

## Gerencie seu consumo de crédito {#manage-credit-consumption}

Para gerenciar efetivamente o consumo de crédito:

1. **Entenda** o consumo de crédito associado a cada atividade. Verifique a [descrição do produto Collaboration](https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} para obter uma tabela de créditos usados por atividade.
2. **Monitorar regularmente**: verifique seu painel de atividades com frequência para entender os padrões de uso.
3. **Rastrear por conexão**: use o nome da conexão para identificar quais conexões estão consumindo mais créditos.
