---
title: Fluxo de trabalho completo
description: Entenda o fluxo de trabalho completo do uso do Real-Time CDP Collaboration com base no seu padrão de colaboração.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 901b17c7493e76b17e780b6f7b05a69fa22303d2
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# Fluxo de trabalho completo

{{limited-availability-release-note}}

No Adobe Real-Time CDP Collaboration, o fluxo de trabalho completo varia de acordo com o padrão de colaboração escolhido. O fluxo de trabalho descreve as etapas envolvidas na configuração e execução de um projeto de colaboração, desde a criação de contas e a seleção de públicos até a criação de conexões e de projetos. A compreensão desse fluxo de trabalho é essencial para aproveitar efetivamente os recursos da plataforma para atingir suas metas de marketing.

## Introdução

Antes de começar, verifique se você tem uma sólida compreensão destes conceitos-chave:

- **Padrões do Collaboration**: esses padrões definem como os colaboradores trabalham juntos. Há cinco padrões distintos:
   - [anunciante-editor](./collaboration-patterns.md#advertiser-to-publisher)
   - [marca-a-marca](./collaboration-patterns.md#brand-to-brand)
   - [anunciante-parceiro de dados](./collaboration-patterns.md#advertiser-to-data-partner)
   - [agência para editor](./collaboration-patterns.md#agency-to-publisher)
   - [plataforma de anunciante para agência](./collaboration-patterns.md#advertiser-to-agency-platform)
- **Funções da conta**: as funções da conta determinam seus recursos na plataforma. Elas devem se alinhar aos objetivos, à marca e às metas de sua organização. Há quatro funções de conta: [anunciante](./roles.md#advertiser), [publicador](./roles.md#publisher), [agência](./roles.md#agency) e [parceiro de dados](./roles.md#data-partner).
- **Casos de uso**: os casos de uso definem como você pode aproveitar o Collaboration para atingir seus objetivos de marketing. Há três casos de uso de colaboração: [Descobrir](./use-cases.md#discover), [Ativar](./use-cases.md#activate) e [Medida](./use-cases.md#measure).

Este guia usará três colaboradores simulados para ilustrar o fluxo de trabalho completo:

- **[!UICONTROL Luma]**: uma marca de vestuário esportivo. Eles são um anunciante que deseja alcançar públicos-alvo específicos por meio de campanhas de marketing direcionadas.
- **[!UICONTROL Tubo de TV]**: um provedor de streaming digital. Eles são um editor que fornece dados de público-alvo para uso por anunciantes.
- **[!UICONTROL Fit Apparel]**: outra marca de vestuário esportivo. Eles são um segundo anunciante que deseja colaborar para compartilhar dados e insights do público-alvo para esforços aprimorados de marketing.
- **[!UICONTROL Agency99]**: uma agência de mídia. Eles gerenciam várias contas de clientes em seu espaço de trabalho e se conectam com editores e anunciantes.
- **[!UICONTROL DataM8]**: um provedor de dados de terceiros. Eles fornecem dados de público-alvo para uso por anunciantes.
- **[!UICONTROL Holdco]**: uma plataforma de serviços de marketing e publicidade de uma empresa holding agência que é usada por equipes internas da agência para gerenciar campanhas de clientes.

## Fluxo de trabalho do anunciante para o editor {#advertiser-to-publisher-workflow}

A [!UICONTROL Luma], uma empresa de varejo atlético, deseja formar uma conexão com o [!UICONTROL TV Tube], um provedor de streaming digital, para alcançar públicos-alvo específicos através de campanhas de marketing direcionadas.

Para começar, a [!UICONTROL Luma] precisa [criar uma conta](../setup/onboard-account.md) com a função de anunciante, enquanto o [!UICONTROL Tubo de TV] cria uma conta com a função de publicador.

Depois de estabelecer suas contas, a [!UICONTROL Luma] e o [!UICONTROL Tubo de TV] devem [criar uma conexão de dados e fornecer públicos-alvo](../setup/onboard-audiences.md). Somente o [!UICONTROL Tubo de TV] ativará os públicos das campanhas de marketing. Portanto, eles precisam [configurar um destino](../setup/manage-destinations.md).

Depois que ambos os colaboradores tiverem suas contas configuradas, eles estarão prontos para [formar uma conexão](../connect/establishing-connections.md) dentro da plataforma. [!UICONTROL O Luma] usa o recurso [descobrir colaboradores](../connect/discover-collaborators.md) para localizar o [!UICONTROL Tubo de TV] e iniciar uma solicitação de conexão. Depois que o [!UICONTROL Tubo de TV] aceitar a solicitação de conexão, o [!UICONTROL Luma] definirá as configurações de conexão para definir como eles irão colaborar. [!UICONTROL TV Tube] aceita a solicitação de conexão para estabelecer um vínculo seguro entre as duas marcas.

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
