---
title: Gerenciar conexões de dados
description: Saiba como gerenciar conexões de dados, incluindo chaves de correspondência, agendamento, casos de uso e filtragem de público-alvo no Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 3%

---

# Gerenciar conexões de dados

{{limited-availability-release-note}}

## Visão geral

Use conexões de dados no Real-Time CDP Collaboration para importar públicos de várias fontes. Saiba como gerenciar chaves de correspondência e agendar importações de dados para suas conexões de dados existentes. Além disso, você poderá filtrar públicos-alvo por atributos diferentes para obter insights mais granulares.

Antes de gerenciar suas conexões de dados aqui, você deve inicialmente configurá-las durante o [fluxo de trabalho de integração de público-alvo](./onboard-audiences.md). Isso garantirá que as fontes de dados corretas sejam conectadas para uso no Real-Time CDP Collaboration.

## Exibir conexões de dados

>[!IMPORTANT]
>
>No momento, a exclusão de uma conexão de dados não é suportada na interface do usuário do Real-Time CDP Collaboration. Para excluir uma conexão de dados, entre em contato com o representante da Adobe ou [crie um tíquete de suporte ao cliente](https://experienceleague.adobe.com/home?lang=en&amp;support-tab=open-ticket#support){target="_blank"}{target=&quot;_blank&quot;}.

Para exibir as conexões de dados existentes, navegue até **[!UICONTROL Configuração]** > **[!UICONTROL Meus públicos-alvo]** e selecione **[!UICONTROL Gerenciar conexões de dados]**.

![Espaço de trabalho de Instalação com Gerenciar conexões de dados realçado.](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

Isso exibe todas as conexões de dados configuradas no momento, com informações sobre o número de públicos-alvo em cada uma delas, a fonte da conexão de dados e muito mais. Selecione **[!UICONTROL Exibir conexão de dados]** para exibir informações sobre as chaves de correspondência, o agendamento e os públicos-alvo que fazem parte dessa conexão de dados.

![Gerenciar espaço de trabalho de conexões de dados com uma conexão Exibir conexões de dados realçadas. ](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

### Coincidir chaves {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Coincidir chaves"
>abstract="As chaves de correspondência determinam como os dados de diferentes fontes serão correspondidos. Escolha as chaves de correspondência mais relevantes para seus casos de uso e diretrizes de privacidade."

As chaves de correspondência são identificadores usados para reconciliar membros entre públicos-alvo de diferentes fontes de dados. As chaves de correspondência disponíveis incluem:

- **Email com hash**

Não é possível editar as chaves de correspondência usadas nesta conexão de dados.

![Um espaço de trabalho de conexões de dados com a seção Corresponder chaves realçada.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

### Agendando {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Agendando"
>abstract="Essa exibição mostra as opções de agendamento selecionadas inicialmente para sua conexão de dados."

Não é possível editar as opções de agendamento selecionadas inicialmente para a conexão de dados. Para obter mais informações sobre opções de agendamento, exiba a [seção de agendamento](/help/guide/setup/onboard-audiences.md#schedule) no documento de fluxo de trabalho de importação de público-alvo.

![Um espaço de trabalho de conexões de dados com a seção Agendamento realçada.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

## Gerenciar públicos {#manage-audiences}

Ao exibir a lista de públicos-alvo da conexão de dados, você pode optar por exibi-los, editar suas categorias ou removê-los da conexão de dados.

![Um espaço de trabalho de conexões de dados com os públicos-alvo realçados.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

## Próximas etapas

Depois de gerenciar suas conexões de dados, você pode [descobrir sobreposições](/help/guide/collaborate/discover.md) entre os públicos-alvo e os públicos que o seu colaborador tornou visíveis.
