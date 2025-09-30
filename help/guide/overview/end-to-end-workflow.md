---
title: Fluxo de trabalho completo
description: Entenda o fluxo de trabalho completo do uso do Real-Time CDP Collaboration com base no seu padrão de colaboração.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 36f43d9d34ce7851a1c7093e0891f9c87e56387c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Fluxo de trabalho completo

{{limited-availability-release-note}}

No Adobe Real-Time CDP Collaboration, o fluxo de trabalho completo varia de acordo com o padrão de colaboração escolhido. O fluxo de trabalho descreve as etapas envolvidas na configuração e execução de um projeto de colaboração, desde a criação de contas e a seleção de públicos até a criação de conexões e de projetos. A compreensão desse fluxo de trabalho é essencial para aproveitar efetivamente os recursos da plataforma para atingir suas metas de marketing.

## Introdução

Antes de começar, verifique se você tem uma sólida compreensão destes conceitos-chave:

- **Padrões do Collaboration**: esses padrões definem como os colaboradores trabalham juntos. Há dois padrões distintos: [anunciante-editor](./collaboration-patterns.md#advertiser-to-publisher) e [marca-para-marca](./collaboration-patterns.md#brand-to-brand).
- **Funções da conta**: as funções da conta determinam seus recursos na plataforma. Elas devem se alinhar aos objetivos, à marca e às metas de sua organização. Há duas funções de conta: [anunciante](./roles.md#advertiser) e [publicador](./roles.md#publisher).
- **Casos de uso**: os casos de uso definem como você pode aproveitar o Collaboration para atingir seus objetivos de marketing. Há três casos de uso de colaboração: [Descobrir](./use-cases.md#discover), [Ativar](./use-cases.md#activate) e [Medida](./use-cases.md#measure).

Este guia usará três colaboradores simulados para ilustrar o fluxo de trabalho completo:

- **[!UICONTROL Luma]**: uma marca de vestuário esportivo. Eles são um anunciante que deseja alcançar públicos-alvo específicos por meio de campanhas de marketing direcionadas.
- **[!UICONTROL Tubo de TV]**: um provedor de streaming digital. Eles são um editor que fornece dados de público-alvo para uso por anunciantes.
- **[!UICONTROL Fit Apparel]**: outra marca de vestuário esportivo. Eles são um segundo anunciante que deseja colaborar para compartilhar dados e insights do público-alvo para esforços aprimorados de marketing.

## Fluxo de trabalho do anunciante para o editor {#advertiser-to-publisher-workflow}

A [!UICONTROL Luma], uma empresa de varejo atlético, deseja formar uma conexão com o [!UICONTROL TV Tube], um provedor de streaming digital, para alcançar públicos-alvo específicos através de campanhas de marketing direcionadas.

Para começar, a [!UICONTROL Luma] precisa [criar uma conta](../setup/onboard-account.md) com a função de anunciante, enquanto o [!UICONTROL Tubo de TV] cria uma conta com a função de publicador.

Depois de estabelecer suas contas, a [!UICONTROL Luma] e o [!UICONTROL Tubo de TV] devem [criar uma conexão de dados e fornecer públicos-alvo](../setup/onboard-audiences.md). Somente o [!UICONTROL Tubo de TV] ativará os públicos das campanhas de marketing. Portanto, eles precisam [configurar um destino](../setup/manage-destinations.md).

Depois que ambos os colaboradores tiverem suas contas configuradas, eles estarão prontos para [formar uma conexão](../connect/establishing-connections.md) dentro da plataforma. [!UICONTROL O Luma] usa o recurso [descobrir colaboradores](../connect/discover-collaborators.md) para localizar o [!UICONTROL Tubo de TV] e iniciar uma solicitação de conexão. Depois que o [!UICONTROL Tubo de TV] aceitar a solicitação de conexão, o [!UICONTROL Luma] definirá as configurações de conexão para definir como será a colaboração. [!UICONTROL TV Tube] aceita a solicitação de conexão para estabelecer um vínculo seguro entre as duas marcas.

Depois que a conexão for estabelecida, o [!UICONTROL Luma] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com o [!UICONTROL Tubo de TV]. Durante a configuração do projeto, eles escolhem os casos de uso de colaboração que melhor se ajustam aos seus objetivos: [Descobrir](../collaborate/discover.md), [Ativar](../collaborate/activate.md) e [Medida](../collaborate/measure.md).

[!UICONTROL O Luma] aproveita o caso de uso [Discover](../collaborate/discover.md) para obter insights sobre os dados de público-alvo do [!UICONTROL Tubo de TV]. Depois que a [!UICONTROL Luma] identificar os segmentos de público-alvo, ela [ativará](../collaborate/activate.md) esses públicos-alvo.

Depois de ativar os públicos-alvo, o [!UICONTROL TV Tube] executa campanhas de marketing direcionadas e carrega dados para [Medir](../collaborate/measure.md) os resultados para avaliar a eficácia da campanha.

## Fluxo de trabalho de marca para marca {#brand-to-brand-workflow}

A [!UICONTROL Fit Apparel], uma marca de vestuário esportivo, deseja colaborar com a [!UICONTROL Luma], outra marca de vestuário esportivo, para compartilhar dados e insights do público-alvo e aprimorar os esforços de marketing.

Depois de estabelecer suas contas, a [!UICONTROL Fit Apparel] e a [!UICONTROL Luma] precisam [criar uma conexão de dados e públicos-alvo de origem](../setup/onboard-audiences.md). O [!UICONTROL Fit Apparel] e a [!UICONTROL Luma] ativarão públicos para campanhas de marketing, portanto, ambos precisam [configurar um destino](../setup/manage-destinations.md).

Depois de fornecer seus públicos-alvo, o [!UICONTROL Fit Apparel] e o [!UICONTROL Luma] [formam uma conexão](../connect/establishing-connections.md) dentro da plataforma para compartilhar dados de público-alvo com segurança. Para isso, eles devem usar o recurso [convidar para conexão privada](../connect/establishing-connections.md#private-connection-invite). [!UICONTROL A Luma] compartilha seu código de conexão com [!UICONTROL Fit Apparel], que o usa para iniciar uma solicitação de conexão. Depois que a [!UICONTROL Luma] aceitar a solicitação de conexão, o [!UICONTROL Fit Apparel] definirá as configurações de conexão para definir como elas irão colaborar. Na configuração, o [!UICONTROL Fit Apparel] especifica que ambos os colaboradores podem ativar públicos para campanhas de marketing. Para concluir a conexão, a [!UICONTROL Luma] aceita a solicitação para estabelecer um vínculo seguro entre as duas marcas.

Depois que a conexão é estabelecida, o [!UICONTROL Fit Apparel] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com a [!UICONTROL Luma]. Durante a configuração do projeto, eles escolhem os casos de uso de colaboração que melhor se ajustam aos seus objetivos: [Descobrir](../collaborate/discover.md), [Ativar](../collaborate/activate.md) e [Medida](../collaborate/measure.md).

A [!UICONTROL Fit Apparel] e a [!UICONTROL Luma] podem usar o caso de uso [Discover](../collaborate/discover.md) para obter insights sobre os dados de público-alvo um do outro. Depois de identificar segmentos de público valiosos, eles [ativam](../collaborate/activate.md) os públicos escolhidos para campanhas de marketing.

Finalmente, após executar suas campanhas, ambas as marcas carregam dados para [Medir](../collaborate/measure.md) os resultados e avaliam a eficácia de sua colaboração.
