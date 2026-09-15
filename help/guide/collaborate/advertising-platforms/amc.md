---
title: Amazon Marketing Cloud
description: Saiba mais sobre como colaborar com o Amazon Marketing Cloud no Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 1a1b8fec-384b-465f-832d-0772c518fdf1
TQID: https://experienceleague.adobe.com/jNTQWEaUuuvgqKboJWsUH4XoKStP49nB0GLUSze0eXw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
    internal-label: Use cases
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: b29c92fa411198ec4e9a0a493c91ee302a327697
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 19%
---
# Amazon Marketing Cloud

{{limited-availability-release-note}}

Depois de formar uma conexão com [!DNL Amazon Marketing Cloud] ([!DNL AMC]), os anunciantes podem [criar um projeto](../manage-projects.md#create-project) para colaborar com [!DNL AMC]. Há suporte para dois casos de uso em um projeto [!DNL AMC]: **Descoberta de público-alvo** usando a seção **[!UICONTROL Descoberta]** e **Medição** usando a guia **[!UICONTROL Medida]**.

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
>abstract="Representa o número de “IDs resolvidas” do público-alvo enviados que também foram expostas a um anúncio por meio do Amazon Ads."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="% de sobreposição"
>abstract="A proporção de “IDs resolvidas” que foram expostas a um anúncio por meio do Amazon Ads."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Detalhamento por produto de anúncio da Amazon"
>abstract="Detalhamento de “Sobreposição de IDs expostas a anúncios” alcançado pelo Produto patrocinado por meio do Amazon Ads e/ou pelo Amazon Ads DSP."

Na seção **[!UICONTROL Discover]**, você pode comparar o público-alvo da AMC a todos os consumidores atingidos pelos seus anúncios do Amazon. Você também pode visualizar os segmentos de direcionamento do Amazon com os quais seu público-alvo tem as sobreposições mais altas, considerando apenas as impressões do DSP (esses segmentos só podem ser direcionados no DSP).

>[!IMPORTANT]
>
>Os dados de público-alvo são processados de públicos-alvo carregados na sua conta do [!DNL Amazon Ads]. Para saber como usar o recurso Destinos do Experience Platform para enviar os públicos-alvo para a conta do [!DNL Amazon Ads], leia o guia [Conexão de anúncios do Amazon](https://experienceleague.adobe.com/pt-br/docs/experience-platform/destinations/catalog/advertising/amazon-ads).

![A seção Descobrir em um projeto com o Amazon Marketing Cloud.](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### Comparar públicos-alvo {#compare-audiences}

A seção **[!UICONTROL Comparar públicos-alvo]** fornece informações sobre como o público-alvo do [!DNL AMC] se sobrepõe aos consumidores atingidos pelos seus anúncios do Amazon. Na seção **[!UICONTROL Comparar públicos-alvo]**, você pode exibir as seguintes métricas:

| Métrica | Descrição |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL IDs Resolvidas] | O número de IDs que [!DNL Amazon's Identity Resolution] conseguiu resolver usando seus dados de público-alvo. |
| [!UICONTROL Sobreposição de IDs expostas ao anúncio] | O número de [!UICONTROL IDs resolvidas] do público-alvo carregado que também foram expostas a um anúncio via [!DNL Amazon Ads]. |
| [!UICONTROL Sobreposição %] | A proporção de [!UICONTROL IDs resolvidas] que foram expostas a um anúncio via [!DNL Amazon Ads]. |
| [!UICONTROL Detalhamento por produto de anúncio da Amazon] | Detalhamento de [!UICONTROL IDs sobrepostas e expostas] atingidas por [!UICONTROL Produto patrocinado] e/ou [!UICONTROL DSP]. Cada uma é representada como uma porcentagem individual do número total de IDs de anúncios expostos. Como uma ID pode pertencer a [!UICONTROL Produtos Patrocinados] e [!UICONTROL DSP], as porcentagens não podem somar 100%. |


### Públicos-alvo relevantes {#relevant-audiences}

A seção **[!UICONTROL Públicos-alvo relevantes]** fornece informações sobre segmentos de direcionamento [!DNL Amazon], ou públicos-alvo, com os quais seu público-alvo tem as sobreposições mais altas, considerando apenas as impressões do DSP (esses segmentos só podem ser direcionados no DSP). Você pode alternar entre todos os públicos relevantes e, em cada seção, ver as seguintes métricas:

| Métrica | Descrição |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL IDs Resolvidas] | O número de IDs que [!DNL Amazon's Identity Resolution] conseguiu resolver usando seus dados de público-alvo. |
| [!UICONTROL Sobreposição de IDs expostas ao anúncio] | Representa o número de [!UICONTROL IDs resolvidas] do público-alvo carregado que também foram expostas a um anúncio via [!DNL Amazon Ads]. Isso só considera impressões do DSP. |
| [!UICONTROL Sobreposição %] | A proporção de [!UICONTROL IDs resolvidas] que foram expostas a um anúncio via [!DNL Amazon Ads]. |
| [!UICONTROL Categorias] | A categoria ou categorias às quais o público-alvo pertence. Um público-alvo pode pertencer a várias categorias. |

### Descobrir sobreposições com [!DNL Amazon Marketing Cloud] {#discover-overlaps}

A seção **[!UICONTROL Descobrir sobreposições com o Amazon Marketing Cloud]** fornece informações sobre como seus públicos se sobrepõem aos segmentos ou públicos-alvo de direcionamento do [!DNL Amazon]. Você pode exibir as seguintes métricas:

| Métrica | Descrição |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL IDs Resolvidas] | O número de IDs que [!DNL Amazon's Identity Resolution] conseguiu resolver usando seus dados de público-alvo. |
| [!UICONTROL Sobreposição de IDs expostas ao anúncio] | Representa o número de [!UICONTROL IDs resolvidas] do público-alvo carregado que também foram expostas a um anúncio via [!DNL Amazon Ads]. Isso só considera impressões do DSP. |
| [!UICONTROL Sobreposição %] | A proporção de [!UICONTROL IDs resolvidas] que foram expostas a um anúncio via [!DNL Amazon Ads]. |

## Medição {#measure}

A guia **[!UICONTROL Medida]** está disponível quando a instância [!DNL AMC] contém IDs de campanha. Ao criar um projeto, o Real-Time CDP Collaboration executa consultas em segundo plano com base nos dados do [!DNL AMC] para preencher a seção [!UICONTROL Descobrir] e as listas de eventos de campanha e conversão usadas para configurar relatórios de medição.

Para obter instruções passo a passo sobre como criar e interpretar [!DNL AMC] relatórios de medição, leia o [guia Criar relatórios de medição da AMC](./amc-measure.md).
