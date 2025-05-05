---
title: Rastrear sua atividade de consumo de crédito
description: Saiba como rastrear a atividade de consumo de crédito da sua organização no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: 3aec9806d2ea920d656bb0981f22ba31fd8ae3ee
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Rastrear sua atividade de consumo de crédito

{{limited-availability-release-note}}

Use a guia **[!UICONTROL Minha Atividade]** para monitorar e acompanhar o consumo de crédito estimado da sua organização em todas as atividades de colaboração. Esse recurso fornece insights detalhados sobre como os créditos estão sendo usados em diferentes conexões e atividades, ajudando você a gerenciar seus recursos de maneira eficaz.

>[!IMPORTANT]
>
>A tabela de consumo de crédito é arredondada e agregada por dia para monitoramento. Os números no painel **[!UICONTROL Minha atividade]** representam um consumo de crédito *estimado*. O consumo de crédito *real* usado para cobrança é rastreado em sistemas internos e está disponível mediante solicitação. Entre em contato com o representante da Adobe para obter essas informações.

Para acessar sua atividade de consumo de crédito estimado, navegue até **[!UICONTROL Configuração]** na navegação principal e selecione a guia **[!UICONTROL Minha atividade]**.

![Painel Minha Atividade mostrando detalhes do consumo de crédito](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>A exibição **[!UICONTROL Minha atividade]** não inclui informações sobre ações do usuário em diferentes partes da interface do usuário da Real-Time Collaboration CDP. Use a funcionalidade [logs de auditoria](/help/guide/setup/audit-logs.md) para obter essas informações.

## Entender o painel de atividades {#understand-dashboard}

O painel de instrumentos de atividade exibe uma lista abrangente de todas as operações de consumo de crédito na organização. Cada linha representa uma atividade distinta e fornece informações importantes sobre o uso do crédito:

>[!NOTE]
>
>As atividades de **[!UICONTROL Gerenciamento de Público-Alvo]** não estão associadas a outro colaborador, portanto, as colunas **[!UICONTROL ID de Conexão]** e **[!UICONTROL Nome de Conexão]** para esses tipos de atividades indicam um valor **[!UICONTROL N/A]**.

| Coluna | Descrição |
|------------|--------------|
| **[!UICONTROL Data]** | A data em que a atividade ocorreu, exibida no formato MM/DD/AAAA. |
| **[!UICONTROL ID da Conexão]** | Um identificador exclusivo para cada conexão associada a uma atividade de consumo de crédito, representada como uma sequência alfanumérica. |
| **[!UICONTROL Nome da conexão]** | O nome do colaborador associado à conexão e à atividade que consome crédito. |
| **[!UICONTROL Atividade]** | O tipo de atividade realizada, como **Ativação - Compartilhamento**, **Ativação - Saída** ou **Gerenciamento de público-alvo**. |
| **[!UICONTROL Entradas processadas]** | O número total de entradas (por exemplo, IDs ou linhas) processadas para a atividade. |
| **[!UICONTROL Total de créditos usados]** | O número total de créditos consumidos pela atividade. |
| **[!UICONTROL Meu compartilhamento de crédito]** | A parte da organização nos créditos usada para a atividade. |

{style="table-layout:auto"}

## Tipos de atividades {#types-of-activities}

A coluna **[!UICONTROL Atividade]** mostra diferentes tipos de operações que consomem crédito.

* **[!UICONTROL Gerenciamento de público-alvo]**: os créditos são consumidos quando os públicos-alvo são importados para a Real-Time CDP Collaboration. Os créditos são consumidos como uma função do número de IDs (em milhões) indexadas no Real-Time CDP Collaboration em todos os públicos-alvo e da frequência dessa indexação (diariamente, a cada três dias ou semanalmente) durante o período de faturamento. Leia mais sobre [importação e gerenciamento de públicos](/help/guide/setup/onboard-audiences.md).
* **[!UICONTROL Ativação - Compartilhamento]** - Os créditos são consumidos como uma função do número de IDs ativadas da Real-Time CDP Collaboration durante todo o período de cobrança. Leia mais sobre [compartilhamento](/help/guide/collaborate/share.md) e [ativação de públicos](/help/guide/collaborate/activate.md) no Real-Time CDP Collaboration.
* **[!UICONTROL Ativação - Saída]** - Os créditos são consumidos como uma função do número de IDs ativadas da Real-Time CDP Collaboration durante todo o período de cobrança. Leia mais sobre [compartilhamento](/help/guide/collaborate/share.md) e [ativação de públicos](/help/guide/collaborate/activate.md) no Real-Time CDP Collaboration.
* **[!UICONTROL Sobreposições de público-alvo]** - Os créditos são consumidos ao analisar sobreposições de público-alvo usando rascunhos de dados. Os rascunhos de dados são resumos simplificados de dados de público-alvo que ajudam a determinar a semelhança entre dois públicos-alvo e, ao mesmo tempo, mantêm a privacidade dos dados. Leia mais sobre [sobreposições de público-alvo na guia de descoberta](/help/guide/collaborate/discover.md).
* **[!UICONTROL Medição de público-alvo]** - Execute atividades no Real-Time CDP Collaboration para gerar relatórios e insights de desempenho da campanha. Os créditos são consumidos com base no número de linhas nos relatórios de campanha em todas as campanhas e na frequência dos relatórios (diariamente, a cada três dias ou semanalmente).


<!--

**[!UICONTROL Audience Overlaps]** – Credits are consumed as a function of the number of matched IDs across 2 or more shared audiences throughout the billing period. Read more about [audience overlaps in the discover tab](/help/guide/collaborate/discover.md).

Collaboration Measurement – Credits are consumed as a function of the number of rows existing in campaign reports across all campaigns, and the frequency of that reporting (daily, every three days, or weekly).

-->


## Gerencie seu consumo de crédito {#manage-credit-consumption}

Para gerenciar efetivamente o consumo de crédito:

1. **Entenda** o consumo de crédito associado a cada atividade. Verifique a [descrição do produto Real-Time CDP Collaboration](https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} para obter uma tabela de créditos de colaboração usados por atividade.
2. **Monitorar regularmente**: verifique seu painel de atividades com frequência para entender os padrões de uso.
3. **Rastrear por conexão**: use o nome da conexão para identificar quais parcerias estão consumindo mais créditos.

<!--

## Pagination and navigation

The activity list is paginated to improve performance and readability. Use the navigation controls at the bottom of the table to move between pages and adjust how many records you can view at once.

-->
