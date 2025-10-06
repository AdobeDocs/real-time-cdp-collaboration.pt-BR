---
title: Amazon Marketing Cloud
description: Saiba mais sobre como colaborar com o Amazon Marketing Cloud no Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 57b847c25edbf88f4708bda74be41fe6141472a7
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 20%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

Depois de formar uma conexão com [!DNL Amazon Marketing Cloud] ([!DNL AMC]), os anunciantes podem [criar um projeto](../manage-projects.md#create-project) para colaborar com [!DNL AMC] para aproveitar seus recursos avançados de análise. Depois de criar um projeto, você pode usar a seção **[!UICONTROL Descobrir]** para comparar os insights do público-alvo e descobrir públicos relevantes para suas campanhas.

>[!IMPORTANT]
>
>Os únicos casos de uso com suporte no [!DNL AMC] são **Descoberta de público-alvo** e **Medição**. Atualmente, somente a seção **[!UICONTROL Descobrir]** está disponível no seu projeto com [!DNL AMC].

## Descobrir {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="Comparar públicos-alvo"
>abstract="Compare o público-alvo com todos os consumidores alcançados pelo seu Amazon Ads."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="Públicos-alvo relevantes"
>abstract="Segmentos de direcionamento da Amazon com os quais o público-alvo possui as maiores sobreposições, considerando apenas as impressões da DSP (esses segmentos só podem ser direcionados na DSP)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="IDs resolvidas"
>abstract="O número de IDs que a Resolução de identidade da Amazon conseguiu resolver com os dados de público-alvo."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="Sobreposição de IDs expostas a anúncios"
>abstract="Representa o número de &quot;IDs resolvidas&quot; do público-alvo enviado que também foram expostas a um anúncio por meio do Amazon Ads."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="% de sobreposição"
>abstract="A proporção de &quot;IDs resolvidas&quot; que foram expostas a um anúncio por meio do Amazon Ads."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Detalhamento por produto de anúncio da Amazon"
>abstract="Detalhamento de &quot;Sobreposição de IDs expostas a anúncios&quot; alcançado pelo produto patrocinado através do Amazon Ads e/ou pela Amazon Ads DSP."

Na seção **[!UICONTROL Discover]**, você pode comparar o público-alvo da AMC a todos os consumidores atingidos pelos seus anúncios do Amazon. Você também pode visualizar os segmentos de direcionamento do Amazon com os quais seu público-alvo tem as sobreposições mais altas, considerando apenas as impressões do DSP (esses segmentos só podem ser direcionados no DSP).

>[!IMPORTANT]
>
>Os dados de público-alvo são processados de públicos-alvo carregados na sua conta do [!DNL Amazon Ads]. Para saber como usar o recurso Destinos do Experience Platform para enviar os públicos-alvo para a conta do [!DNL Amazon Ads], leia o guia [Conexão de anúncios do Amazon](https://experienceleague.adobe.com/pt-br/docs/experience-platform/destinations/catalog/advertising/amazon-ads).

![A seção Descobrir em um projeto com o Amazon Marketing Cloud.](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### Comparar públicos-alvo {#compare-audiences}

A seção **[!UICONTROL Comparar públicos-alvo]** fornece informações sobre como o público-alvo do [!DNL AMC] se sobrepõe aos consumidores atingidos pelos seus anúncios do Amazon. Na seção **[!UICONTROL Comparar públicos-alvo]**, você pode exibir as seguintes métricas:

| Métrica | Descrição |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL IDs Resolvidas] | O número de IDs que [!DNL Amazon’s Identity Resolution] conseguiu resolver usando seus dados de público-alvo. |
| [!UICONTROL Sobreposição de IDs expostas ao anúncio] | O número de [!UICONTROL IDs resolvidas] do público-alvo carregado que também foram expostas a um anúncio via [!DNL Amazon Ads]. |
| [!UICONTROL Sobreposição %] | A proporção de [!UICONTROL IDs resolvidas] que foram expostas a um anúncio via [!DNL Amazon Ads]. |
| [!UICONTROL Detalhamento por produto de anúncio da Amazon] | Detalhamento de [!UICONTROL IDs sobrepostas e expostas] atingidas por [!UICONTROL Produto patrocinado] e/ou [!UICONTROL DSP]. Cada uma é representada como uma porcentagem individual do número total de IDs de anúncios expostos. Como uma ID pode pertencer a [!UICONTROL Produtos Patrocinados] e [!UICONTROL DSP], as porcentagens não podem somar 100%. |


### Públicos-alvo relevantes {#relevant-audiences}

A seção **[!UICONTROL Públicos-alvo relevantes]** fornece informações sobre segmentos de direcionamento [!DNL Amazon], ou públicos-alvo, com os quais seu público-alvo tem as sobreposições mais altas, considerando apenas as impressões do DSP (esses segmentos só podem ser direcionados no DSP). Você pode alternar entre todos os públicos relevantes e, em cada seção, ver as seguintes métricas:

| Métrica | Descrição |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL IDs Resolvidas] | O número de IDs que [!DNL Amazon’s Identity Resolution] conseguiu resolver usando seus dados de público-alvo. |
| [!UICONTROL Sobreposição de IDs expostas ao anúncio] | Representa o número de [!UICONTROL IDs resolvidas] do público-alvo carregado que também foram expostas a um anúncio via [!DNL Amazon Ads]. Isso só considera impressões do DSP. |
| [!UICONTROL Sobreposição %] | A proporção de [!UICONTROL IDs resolvidas] que foram expostas a um anúncio via [!DNL Amazon Ads]. |
| [!UICONTROL Categorias] | A categoria ou categorias às quais o público-alvo pertence. Um público-alvo pode pertencer a várias categorias. |

### Descobrir sobreposições com [!DNL Amazon Marketing Cloud] {#discover-overlaps}

A seção **[!UICONTROL Descobrir sobreposições com o Amazon Marketing Cloud]** fornece informações sobre como seus públicos se sobrepõem aos segmentos ou públicos-alvo de direcionamento do [!DNL Amazon]. Você pode exibir as seguintes métricas:

| Métrica | Descrição |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL IDs Resolvidas] | O número de IDs que [!DNL Amazon’s Identity Resolution] conseguiu resolver usando seus dados de público-alvo. |
| [!UICONTROL Sobreposição de IDs expostas ao anúncio] | Representa o número de [!UICONTROL IDs resolvidas] do público-alvo carregado que também foram expostas a um anúncio via [!DNL Amazon Ads]. Isso só considera impressões do DSP. |
| [!UICONTROL Sobreposição %] | A proporção de [!UICONTROL IDs resolvidas] que foram expostas a um anúncio via [!DNL Amazon Ads]. |