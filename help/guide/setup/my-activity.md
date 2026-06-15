---
title: Rastrear sua atividade de consumo de crédito
description: Saiba como visualizar a Carteira de crédito da sua organização e rastrear a atividade de consumo de crédito no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
TQID: https://experienceleague.adobe.com/hDvkKFUCBYvsX8wntcYFrL6qZTxOo5CZOWAbxNwk7mw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 681f4af47a58a2ce66b25b09d793d0b5b127df39
workflow-type: tm+mt
source-wordcount: 726
ht-degree: 2%

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

Para acessar sua Carteira de Crédito e a atividade de consumo de crédito, navegue até **[!UICONTROL Configuração]** na navegação principal e selecione a guia **[!UICONTROL Minha atividade]**.

![A guia Minha atividade mostrando a Carteira de Crédito com créditos provisionados, créditos consumidos, créditos disponíveis e a tabela de atividade de consumo de crédito.](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>A exibição **[!UICONTROL Minha atividade]** não inclui ações do usuário de outras áreas da interface do Real-Time CDP Collaboration. Use a funcionalidade [logs de auditoria](/help/guide/setup/audit-logs.md) para obter essas informações.

## Entender a exibição Minha atividade {#understand-dashboard}

Use a exibição **[!UICONTROL Minha atividade]** para monitorar seu uso de crédito e revisar as atividades que consomem créditos. A view inclui a Carteira de Crédito e uma tabela de atividades.

A Carteira de Crédito mostra os créditos provisionados, os créditos consumidos e os créditos disponíveis.

| Métrica | Descrição |
|---------|-------------|
| **[!UICONTROL Créditos provisionados]** | O número de créditos provisionados para sua conta. |
| **[!UICONTROL Créditos consumidos]** | O número de créditos consumidos pela sua conta a partir da atualização diária mais recente. |
| **[!UICONTROL Créditos disponíveis]** | O número de créditos disponíveis para sua conta, calculado a partir dos créditos provisionados menos os créditos consumidos. |

{style="table-layout:auto"}

A tabela de atividades lista os registros de consumo de crédito diário por data, tipo de atividade, entradas processadas e créditos usados:

>[!NOTE]
>
>As atividades de **[!UICONTROL Gerenciamento de Público-Alvo]** não estão associadas a outro colaborador, portanto, as colunas **[!UICONTROL ID de Conexão]** e **[!UICONTROL Nome de Conexão]** desses tipos de atividades mostram um valor de **[!UICONTROL -]**.

| Coluna | Descrição |
|------------|--------------|
| **[!UICONTROL Data]** | A data em que a atividade ocorreu, exibida no formato MM/DD/AAAA. |
| **[!UICONTROL ID da Conexão]** | Um identificador exclusivo para cada conexão associada a uma atividade de consumo de crédito, representada como uma sequência alfanumérica. |
| **[!UICONTROL Nome da conexão]** | O nome do colaborador associado à conexão e à atividade que consome crédito. |
| **[!UICONTROL Atividade]** | O tipo de atividade realizada, como **[!UICONTROL Ativação - Acesso de Público (Uma Vez)]**, **[!UICONTROL Ativação - Acesso de Público (Recorrente)]**, **[!UICONTROL Ativação - Saída de Público (Uma Vez)]**, **[!UICONTROL Ativação - Saída de Público (Recorrente)]** ou **[!UICONTROL Gerenciamento de Público]**. |
| **[!UICONTROL Entradas processadas]** | O número total de entradas (por exemplo, IDs ou linhas) processadas para a atividade. |
| **[!UICONTROL Total de créditos usados]** | O total de créditos consumidos pela atividade. |
| **[!UICONTROL Meu compartilhamento de crédito]** | A parte da sua conta dos créditos usados para a atividade. |

{style="table-layout:auto"}

## Tipos de atividades {#types-of-activities}

A coluna **[!UICONTROL Atividade]** mostra diferentes tipos de operações que consomem crédito.

* **[!UICONTROL Gerenciamento de público-alvo]**: os créditos são consumidos quando os públicos-alvo são originados na Collaboration. Os créditos são consumidos como uma função do número de IDs indexadas no Collaboration em todos os públicos-alvo e da frequência dessa indexação, como diária, a cada três dias ou semanalmente. Para saber mais, leia o [guia de fornecimento e gerenciamento de públicos-alvo](/help/guide/setup/onboard-audiences.md).
* **[!UICONTROL Ativação - Acesso de Público (Uma Vez)]**: os créditos são consumidos quando o acesso de público é processado uma vez por meio do fluxo de trabalho de ativação. Para saber mais, leia o [guia de ativação de públicos-alvo](/help/guide/collaborate/activate.md).
* **[!UICONTROL Ativação - Acesso de Público (Recorrente)]**: os créditos são consumidos quando o acesso de público é processado em um agendamento recorrente por meio do fluxo de trabalho de ativação. Para saber mais, leia o [guia de ativação de públicos-alvo](/help/guide/collaborate/activate.md).
* **[!UICONTROL Ativação - Saída de público-alvo (Uma vez)]**: os créditos são consumidos quando a saída do público-alvo para um destino é processada uma vez por meio do fluxo de trabalho de ativação. Essa atividade é cobrada do colaborador que recebe o público-alvo. Para saber mais, leia o [guia de ativação de públicos-alvo](/help/guide/collaborate/activate.md).
* **[!UICONTROL Ativação - Saída de público-alvo (Recorrente)]**: os créditos são consumidos quando a saída de público-alvo para um destino é processada em uma agenda recorrente por meio do fluxo de trabalho de ativação. Essa atividade é cobrada do colaborador que recebe o público-alvo. Para saber mais, leia o [guia de ativação de públicos-alvo](/help/guide/collaborate/activate.md).
* **[!UICONTROL Medição]**: os créditos são consumidos quando você gera relatórios de desempenho de campanha e insights no Collaboration. Os créditos são consumidos com base no número de linhas nos relatórios da campanha em todas as campanhas e na frequência dos relatórios, como diariamente, a cada três dias ou semanalmente.

## Gerencie seu consumo de crédito {#manage-credit-consumption}

Para gerenciar efetivamente o consumo de crédito:

1. **Entenda** o consumo de crédito associado a cada atividade. Verifique a [descrição do produto Collaboration](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} para obter uma tabela de créditos usados por atividade.
2. **Monitorar o uso regularmente**: Revise seus créditos disponíveis e a tabela de atividades para entender os padrões de uso nas atividades de gerenciamento de público-alvo, acesso a público-alvo, saída de público-alvo e medição.
3. **Rastrear por conexão**: use o nome da conexão para identificar quais conexões estão consumindo mais créditos.
