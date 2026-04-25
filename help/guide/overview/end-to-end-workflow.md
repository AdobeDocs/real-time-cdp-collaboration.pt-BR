---
title: Fluxo de trabalho completo
description: Understand the end-to-end workflow of using Real-Time CDP Collaboration based on your collaboration pattern.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
TQID: https://experienceleague.adobe.com/9edtg5tMbnB3BrdLrDkcHQ-AjBNOqMFGojAja3NCwCs
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1738
ht-degree: 0%

---

# Fluxo de trabalho completo

{{limited-availability-release-note}}

In Adobe Real-Time CDP Collaboration, the end-to-end workflow varies based on the collaboration pattern you choose. The workflow outlines the steps involved in setting up and executing a collaboration project, from creating accounts and sourcing audiences to forming connections and creating projects. Understanding this workflow is essential for effectively leveraging the platform&#39;s capabilities to achieve your marketing goals.

## Introdução

Before you begin, ensure you have a solid understanding of these key concepts:

- **Collaboration patterns**: These patterns define how collaborators work together. There are five distinct patterns:
   - [advertiser-to-publisher](./collaboration-patterns.md#advertiser-to-publisher)
   - [brand-to-brand](./collaboration-patterns.md#brand-to-brand)
   - [advertiser-to-data partner](./collaboration-patterns.md#advertiser-to-data-partner)
   - [agency-to-publisher](./collaboration-patterns.md#agency-to-publisher)
   - [advertiser-to-agency platform](./collaboration-patterns.md#advertiser-to-agency-platform)
- **Account roles**: Account roles determine your capabilities within the platform. They should align with your organization&#39;s objectives, brand, and goals. There are four account roles: [advertiser](./roles.md#advertiser), [publisher](./roles.md#publisher), [agency](./roles.md#agency) and [data partner](./roles.md#data-partner).
- **Use cases**: Uses cases define the ways you can leverage Collaboration to achieve your marketing objectives. There are three collaboration use cases: [Discover](./use-cases.md#discover), [Activate](./use-cases.md#activate), and [Measure](./use-cases.md#measure).

This guide will use three mock collaborators to illustrate the end-to-end workflow:

- **[!UICONTROL Luma]**: An athletic apparel brand. They are an advertiser that wants to reach specific audiences through targeted marketing campaigns.
- **[!UICONTROL TV Tube]**: A digital streaming provider. They are a publisher that provides audience data for use by advertisers.
- **[!UICONTROL Fit Apparel]**: outra marca de vestuário esportivo. They are a second advertiser that wants to collaborate to share audience data and insights for enhanced marketing efforts.
- **[!UICONTROL Agency99]**: A media agency. They manage multiple client accounts within their workspace, and connect with publishers and advertisers.
- **[!UICONTROL DataM8]**: a third-party data provider. They provide audience data for use by advertisers.
- **[!UICONTROL Holdco]**: an agency holding company marketing and advertising services platform that&#39;s used by internal agency teams to manage client campaigns.

## Advertiser-to-publisher workflow {#advertiser-to-publisher-workflow}

[!UICONTROL Luma], an athletic retail company, wants to form a connection with [!UICONTROL TV Tube], a digital streaming provider, to reach specific audiences through targeted marketing campaigns.

To begin, [!UICONTROL Luma] needs to [create an account](../setup/onboard-account.md) with the advertiser role, while [!UICONTROL TV Tube] creates an account with the publisher role.

After establishing their accounts, both [!UICONTROL Luma] and [!UICONTROL TV Tube] must [create a data connection and source audiences](../setup/onboard-audiences.md). Only [!UICONTROL TV Tube] will activate audiences for marketing campaigns, so they need to [configure a destination](../setup/manage-destinations.md).

Once both collaborators have their accounts set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) within the platform. [!UICONTROL Luma] uses the [discover collaborators](../connect/discover-collaborators.md) feature to find [!UICONTROL TV Tube] and initiate a connection request. After [!UICONTROL TV Tube] accepts the connection request, [!UICONTROL Luma] configures the connection settings to define how they will collaborate. [!UICONTROL TV Tube] accepts the connection request to establish a secure link between the two brands.

After the connection is established, [!UICONTROL Luma] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!UICONTROL TV Tube]. During the project setup, they choose the collaboration use cases that best fit their objectives: [Discover](../collaborate/discover.md), [Activate](../collaborate/activate.md), and [Measure](../collaborate/measure.md).

[!UICONTROL Luma] leverages the [Discover](../collaborate/discover.md) use case to gain insights into [!UICONTROL TV Tube]&#39;s audience data. Once [!UICONTROL Luma] has identified the target audience segments, they [Activate](../collaborate/activate.md) these audiences.

After activating the audiences, [!UICONTROL TV Tube] runs targeted marketing campaigns and uploads data to [Measure](../collaborate/measure.md) the results to evaluate the effectiveness of their campaign.

## Brand-to-brand workflow {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel], an athletic apparel brand, wants to collaborate with [!UICONTROL Luma], another athletic apparel brand, to share audience data and insights for enhanced marketing efforts.

After establishing their accounts, both [!UICONTROL Fit Apparel] and [!UICONTROL Luma] need to [create a data connection and source audiences](../setup/onboard-audiences.md). Both [!UICONTROL Fit Apparel] and [!UICONTROL Luma] will activate audiences for marketing campaigns, so they both need to [configure a destination](../setup/manage-destinations.md).

Depois de fornecer seus públicos-alvo, o [!UICONTROL Fit Apparel] e o [!UICONTROL Luma] [formam uma conexão](../connect/establishing-connections.md) dentro da plataforma para compartilhar dados de público-alvo com segurança. Para isso, eles devem usar o recurso [convidar para conexão privada](../connect/establishing-connections.md#private-connection-invite). [!UICONTROL A Luma] compartilha seu código de conexão com [!UICONTROL Fit Apparel], que o usa para iniciar uma solicitação de conexão. Depois que a [!UICONTROL Luma] aceitar a solicitação de conexão, o [!UICONTROL Fit Apparel] definirá as configurações de conexão para definir como elas irão colaborar. Na configuração, o [!UICONTROL Fit Apparel] especifica que ambos os colaboradores podem ativar públicos para campanhas de marketing. Para concluir a conexão, a [!UICONTROL Luma] aceita a solicitação para estabelecer um vínculo seguro entre as duas marcas.

Depois que a conexão é estabelecida, o [!UICONTROL Fit Apparel] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com a [!UICONTROL Luma]. Durante a configuração do projeto, eles escolhem os casos de uso de colaboração que melhor se ajustam aos seus objetivos: [Descobrir](../collaborate/discover.md), [Ativar](../collaborate/activate.md) e [Medida](../collaborate/measure.md).

A [!UICONTROL Fit Apparel] e a [!UICONTROL Luma] podem usar o caso de uso [Discover](../collaborate/discover.md) para obter insights sobre os dados de público-alvo um do outro. Depois de identificar segmentos de público valiosos, eles [ativam](../collaborate/activate.md) os públicos escolhidos para campanhas de marketing.

Finalmente, após executar suas campanhas, ambas as marcas carregam dados para [Medir](../collaborate/measure.md) os resultados e avaliam a eficácia de sua colaboração.

## Fluxo de trabalho da plataforma do anunciante para o anúncio {#advertiser-to-advertising-platform-workflow}

A [!UICONTROL Luma], uma empresa de varejo esportivo, deseja se conectar com a [!DNL Amazon Marketing Cloud] ([!DNL AMC]) para aprimorar seus recursos de marketing, aproveitando as ferramentas de direcionamento e resolução de identidade do [!DNL AMC]. A Luma já tem uma conta [!DNL Amazon Advertising] ativa e está aprovada para usar [!DNL AMC].

Para começar, a [!UICONTROL Luma] precisa [criar uma conta](../setup/onboard-account.md) com a função de anunciante. Depois de estabelecer a conta, a [!UICONTROL Luma] deve [criar uma conexão de dados e públicos-alvo de origem](../setup/onboard-audiences.md). Como a [!UICONTROL Luma] ativará públicos para campanhas de marketing, é necessário [configurar um destino](../setup/manage-destinations.md).

Depois que a [!UICONTROL Luma] tiver sua conta configurada, ela estará pronta para [formar uma conexão](../connect/establishing-connections.md) com [!DNL AMC] dentro da plataforma. A [!UICONTROL Luma] usa o recurso [descobrir colaboradores](../connect/discover-collaborators.md) para localizar o [!UICONTROL Amazon Marketing Cloud] e [iniciar uma solicitação de conexão](../connect/advertising-platforms/amc.md). Após autenticar e autorizar a conexão por meio da página de entrada [!DNL Amazon], a conexão com [!DNL AMC] é estabelecida.

Depois que a conexão é estabelecida, o [!UICONTROL Luma] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com o [!DNL AMC]. As configurações de conexão, incluindo casos de uso, são pré-configuradas dependendo da plataforma de publicidade. Para [!DNL AMC], o caso de uso disponível é [Descobrir](../collaborate/advertising-platforms/amc.md#discover).

[!UICONTROL O Luma] aproveita o caso de uso [Discover](../collaborate/advertising-platforms/amc.md#discover) para obter insights e dados de público-alvo de [!DNL AMC]. Usando esses insights, a [!UICONTROL Luma] pode otimizar suas estratégias de marketing e melhorar a eficácia da campanha.

## Fluxo de trabalho do anunciante para o parceiro de dados {#advertiser-to-data-partner-workflow}

A [!UICONTROL Luma], uma empresa de varejo atlético, deseja colaborar com a [!UICONTROL DataM8], um provedor de dados de terceiros, para enriquecer os perfis dos clientes e melhorar o direcionamento do público-alvo.

Para começar, a [!UICONTROL Luma] precisa [criar uma conta](../setup/onboard-account.md) com a função de anunciante, enquanto a [!UICONTROL DataM8] cria uma conta com a função de parceiro de dados.

Depois de estabelecer suas contas, a [!UICONTROL Luma] e o [!UICONTROL DataM8] devem [criar uma conexão de dados e públicos-alvo de origem](../setup/onboard-audiences.md). Ambos os colaboradores podem ativar públicos para campanhas de marketing, portanto, cada um deles precisa [configurar um destino](../setup/manage-destinations.md).

Depois que ambos os colaboradores tiverem suas contas configuradas, eles estarão prontos para [formar uma conexão](../connect/establishing-connections.md) dentro da plataforma. A [!UICONTROL Luma] usa o recurso [descobrir colaboradores](../collaborate/discover.md) para localizar o [!UICONTROL DataM8] e iniciar uma solicitação de conexão. Depois que o [!UICONTROL DataM8] aceitar a solicitação de conexão, a [!UICONTROL Luma] definirá as configurações de conexão para definir como eles irão colaborar. [!UICONTROL DataM8] aceita a solicitação de conexão para estabelecer um vínculo seguro entre os dois colaboradores.

Depois que a conexão é estabelecida, o [!UICONTROL Luma] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com o [!UICONTROL DataM8]. Durante a configuração do projeto, eles escolhem os casos de uso de colaboração que melhor se ajustam aos seus objetivos: [Descobrir](../collaborate/discover.md), [Ativar](../collaborate/activate.md) e [Medida](../collaborate/measure.md).

[!UICONTROL O Luma] aproveita o caso de uso [Discover](../collaborate/discover.md) para obter insights sobre os dados de público-alvo do [!UICONTROL DataM8]. Depois que a [!UICONTROL Luma] identificar os segmentos de público-alvo de destino, ela [ativará](../collaborate/activate.md) esses públicos-alvo.

[!UICONTROL DataM8] também pode [ativar](../collaborate/activate.md) seus públicos-alvo para [!UICONTROL Luma]. A [!UICONTROL Luma] usa esses recursos para anexar atributos de terceiros aos seus perfis de clientes e analisar a composição do público-alvo. Com dados enriquecidos disponíveis diretamente em sua CDP, a [!UICONTROL Luma] pode criar públicos mais precisos e ativá-los para destinos de mídia paga sem mover dados para fora do ambiente controlado.

## Fluxo de trabalho de agência para editor {#agency-to-publisher-workflow}

A [!UICONTROL Agency99], uma agência de mídia, deseja colaborar com o [!UICONTROL TV Tube], um provedor de streaming digital, para atingir públicos específicos através de campanhas de marketing direcionadas.

Para começar, [!UICONTROL Agency99] precisa [criar uma conta](../setup/onboard-account.md) com a função de agência, enquanto o [!UICONTROL TV Tube] cria uma conta com a função de editor.

Depois de estabelecer suas contas, o [!UICONTROL Agency99] e o [!UICONTROL TV Tube] devem [criar uma conexão de dados e fornecer públicos-alvo](../setup/onboard-audiences.md). [!UICONTROL Agency99] configurará subcontas de cliente e dados de cliente de origem em seu espaço de trabalho. Somente o [!UICONTROL Tubo de TV] ativará os públicos das campanhas de marketing. Portanto, eles precisam [configurar um destino](../setup/manage-destinations.md).

Depois que ambos os colaboradores tiverem suas contas configuradas, eles estarão prontos para [formar uma conexão](../connect/establishing-connections.md) dentro da plataforma. A [!UICONTROL Agency99] usa o recurso [descobrir colaboradores](../collaborate/discover.md) para localizar o [!UICONTROL Tubo de TV] e iniciar uma solicitação de conexão. A [!UICONTROL Agency99] fará isso para um ou vários clientes que desejam colaborar com o [!UICONTROL TV Tube]. Depois que o [!UICONTROL Tubo de TV] aceitar as solicitações de conexão, a [!UICONTROL Agency99] definirá as configurações de conexão para definir como cada colaboração. [!UICONTROL TV Tube] aceita as solicitações de conexão para estabelecer um vínculo seguro entre as duas marcas.

Depois que a conexão é estabelecida, o [!UICONTROL Agency99] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com o [!UICONTROL Tubo de TV] em cada subconta de cliente. Durante a configuração do projeto, eles escolhem os casos de uso de colaboração que melhor se ajustam aos seus objetivos: [Descobrir](../collaborate/discover.md), [Ativar](../collaborate/activate.md) e [Medida](../collaborate/measure.md).

A [!UICONTROL Agency99] aproveita o caso de uso [Discover](../collaborate/discover.md) para obter insights sobre os dados de público-alvo do [!UICONTROL Tubo de TV]. Depois que a [!UICONTROL Agency99] identificar os segmentos de público-alvo, eles [ativarão](../collaborate/activate.md) esses públicos-alvo.

Depois de ativar os públicos-alvo, o [!UICONTROL TV Tube] executa campanhas de marketing direcionadas e carrega dados para [medir](../collaborate/measure.md) os resultados para avaliar a eficácia da campanha.

## Fluxo de trabalho da plataforma do anunciante para a agência {#advertiser-to-agency-platform-workflow}

A [!UICONTROL Luma], uma empresa de varejo atlético, deseja colaborar com a [!UICONTROL Holdco], uma plataforma de agência, para compartilhar dados e receber insights de mídia paga.

Para começar, a [!UICONTROL Luma] precisa [criar uma conta](../setup/onboard-account.md) com a função de anunciante, enquanto a [!UICONTROL Holdco] cria uma conta com a função de agência. 

Depois de estabelecer suas contas, a [!UICONTROL Luma] e a [!UICONTROL Holdco] devem [criar uma conexão de dados e públicos-alvo de origem](../setup/onboard-audiences.md). Ambos os colaboradores podem ativar públicos para campanhas de marketing, portanto, cada um deles precisa [configurar um destino](../setup/manage-destinations.md). 

Depois que ambos os colaboradores tiverem suas contas configuradas, eles estarão prontos para [formar uma conexão](../connect/establishing-connections.md) dentro da plataforma. A [!UICONTROL Luma] usa o recurso [descobrir colaboradores](../collaborate/discover.md) para localizar a [!UICONTROL Holdco] e iniciar uma solicitação de conexão. Depois que a [!UICONTROL Holdco] aceitar a solicitação de conexão, a [!UICONTROL Luma] definirá as configurações de conexão para definir como elas irão colaborar.

[!UICONTROL Holdco] aceita a solicitação de conexão para estabelecer um vínculo seguro entre os dois colaboradores.

Depois que a conexão é estabelecida, o [!UICONTROL Luma] [cria um projeto](../collaborate/manage-projects.md) para iniciar sua colaboração com a [!UICONTROL Holdco]. Durante a configuração do projeto, eles escolhem os casos de uso de colaboração que melhor se ajustam aos seus objetivos: [Descobrir](../collaborate/discover.md), [Ativar](../collaborate/activate.md) e [Medida](../collaborate/measure.md).

A [!UICONTROL Luma] aproveita o caso de uso [Discover](../collaborate/discover.md) para obter insights sobre os dados de público-alvo da [!UICONTROL Holdco]. Depois que a [!UICONTROL Luma] identificar os segmentos de público-alvo de destino, ela [ativará](../collaborate/activate.md) esses públicos-alvo.

[!UICONTROL A Holdco] também pode [ativar](../collaborate/activate.md) seus públicos-alvo para a [!UICONTROL Luma]. A [!UICONTROL Luma] usa esses recursos para receber insights de mídia paga de campanhas executadas por agências para obter insights, anexos de perfil de CDP e orquestração de mídia própria.
