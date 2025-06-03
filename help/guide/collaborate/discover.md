---
title: Descubra sobreposições e compare públicos
description: Descubra sobreposições entre o seu e o público-alvo de seus colaboradores. Saiba como descobrir os melhores públicos-alvo para usar em suas campanhas.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 24%

---

# Descubra sobreposições e compare públicos

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Descoberta]** só estará disponível se o caso de uso **Descoberta de público-alvo** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

Depois de [criar um projeto](/help/guide/collaborate/manage-projects.md) em um espaço de colaboração entre um anunciante e um editor, você pode comparar seus públicos com os públicos de seu colaborador. Dessa forma, você pode descobrir sobreposições entre públicos e obter insights detalhados por chaves ou identidades de correspondência. Isso ajuda os anunciantes a decidirem quais públicos-alvo compartilhar com editores para ativação.

>[!IMPORTANT]
>
>Quaisquer [rascunhos de dados](/help/guide/glossary.md#sketches) que não forem atualizados ou atualizados serão excluídos após 7 dias. Quando isso acontece, os números exibidos nos vários relatórios de sobreposição nesta página vão para zero e o compartilhamento de público-alvo fica indisponível para esses públicos expirados. Os rascunhos de dados são atualizados automaticamente para públicos-alvo com um [cronograma de atualização ativo](/help/guide/setup/onboard-audiences.md#schedule).

![Descobrir sobreposições](/help/assets/collaborate/discover-overlaps/discover-overlaps.png)

As chaves de correspondência usadas para descobrir e comparar públicos são definidas quando você [se conecta a um publicador](/help/guide/connect/establishing-connections.md#connection-settings). Para alterar as porcentagens de sobreposição indicadas em preparação para campanhas em execução, você pode remover as teclas de correspondência, mas não pode adicionar novas teclas de correspondência neste momento. Para fazer isso, vá para as [configurações de conexão](/help/guide/connect/establishing-connections.md#connection-settings) entre os colaboradores.

![Editar tela de chaves de correspondência](/help/assets/collaborate/discover-overlaps/edit-match-keys.png)

## Pré-requisitos {#prerequisites}

Para utilizar toda a funcionalidade na guia **[!UICONTROL Descobrir]** do fluxo de trabalho **[!UICONTROL Colaborar]**, você já:

* [Públicos importados](/help/guide/setup/onboard-audiences.md)
* [Conectado](/help/guide/connect/establishing-connections.md) com um anunciante ou editor desejado com o caso de uso **Descoberta de público-alvo** habilitado
* [Criou um projeto](/help/guide/collaborate/manage-projects.md) entre você e um colaborador

Depois que os pré-requisitos anotados acima forem atendidos, você poderá começar a explorar e comparar a sobreposição entre os públicos do e do seu colaborador.

## Comparar públicos-alvo {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="Comparar públicos-alvo"
>abstract="Descubra sobreposições entre os seus públicos-alvo e os do seu colaborador. É possível ajustar as configurações no seletor suspenso para descobrir sobreposições entre um ou mais dos seus públicos-alvo em relação a um ou mais dos públicos-alvo do seu colaborador."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="Sua contagem de identidades"
>abstract="O número de perfis com essa identidade selecionada que fazem parte do seu público-alvo selecionado"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="Contagem de identidades do colaborador"
>abstract="O número de perfis com essa identidade selecionada que fazem parte do público-alvo selecionado do colaborador"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="Contagem de identidades sobrepostas"
>abstract="O número de perfis com essa identidade selecionada que estão presentes no seu público-alvo e no do seu colaborador."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="Porcentagem de identidades sobrepostas"
>abstract="A porcentagem de sobreposição de perfis entre o público alvo selecionado do seu colaborador e o seu."

Use o cartão Comparar públicos para obter informações detalhadas sobre a sobreposição entre os públicos do e do colaborador. É possível selecionar uma das seguintes combinações de público-alvo para comparar:

* Um dos públicos-alvo em relação a um dos públicos-alvo do colaborador
* Um dos públicos-alvo em relação a todos os públicos-alvo do colaborador
* Todos os públicos-alvo em relação a um dos públicos-alvo do colaborador
* Todos os públicos-alvo de todos os públicos-alvo do colaborador

As informações exibidas estão relacionadas a:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Contagem de identidades]** (sua) | O número de perfis com uma identidade selecionada que fazem parte do público-alvo selecionado. |
| **[!UICONTROL Contagem de identidades]** (seu colaborador) | O número de perfis com uma identidade selecionada que fazem parte do público selecionado do colaborador. |
| **[!UICONTROL Identidades sobrepostas]** | O número de perfis com uma identidade selecionada presentes no seu público-alvo e no do seu colaborador. |
| **[!UICONTROL Percentual de sobreposição]** | A porcentagem de sobreposição de perfis entre o público alvo selecionado do seu colaborador e o seu. |
| **[!UICONTROL Detalhamento de identidades por chave de correspondência]** | Com base nas chaves de correspondência em que você e seu colaborador concordaram para o projeto, visualize a composição das identidades nos cálculos de sobreposição por chaves de correspondência individuais. |

{style="table-layout:auto"}

>[!TIP]
>
>O índice de porcentagem de sobreposição nem sempre está disponível para todos os públicos-alvo. A visibilidade do indicador de porcentagem de sobreposição depende da configuração escolhida pelo seu colaborador para um público na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility).

## Públicos-alvo relevantes {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="Públicos-alvo relevantes"
>abstract="Com base nas porcentagens de sobreposição, esses públicos-alvo do editor podem ser adequados para a campanha. <br><br> A <b>contagem de identidades</b> é o tamanho do público-alvo do editor. <br><br> As <b>identidades sobrepostas</b> representam a sobreposição entre o público-alvo do editor recomendado e todos os públicos-alvo do anunciante. <br><br> A <b>% de sobreposição</b> representa o número de identidades sobrepostas dividido pelo tamanho de <i>todos</i> os públicos-alvo do anunciante."

A exibição **[!UICONTROL Públicos-alvo relevantes]** no módulo **[!UICONTROL Discover]** fornece uma lista com curadoria dos cinco principais públicos-alvo com base na porcentagem de sobreposição. Esse recurso ajuda a identificar rapidamente os públicos-alvo com a maior sobreposição com os dados atuais, permitindo que você direcione suas campanhas com mais eficiência.

* **[!UICONTROL Contagem de identidades]** é o tamanho do público do publicador.
* **[!UICONTROL Identidades sobrepostas]** representam a sobreposição entre o público-alvo do editor recomendado e todos os públicos-alvo do anunciante.
* **[!UICONTROL Sobreposição %]** representa o número de identidades sobrepostas dividido pelo tamanho de *todos* públicos-alvo de anunciantes.

![Exibição de públicos relevantes](/help/assets/collaborate/discover-overlaps/relevant-audiences-highlighted.png)

## Descubra sobreposições {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="Descubra sobreposições com públicos-alvo individuais"
>abstract="Obtenha insights sobre a população desse público-alvo e suas sobreposições com o universo de identidades do colaborador."

![Descubra sobreposições com diferentes visualizações de públicos-alvo](/help/assets/collaborate/discover-overlaps/discover-overlaps-cards-view.png)

Obtenha informações abrangentes sobre qualquer público do colaborador e visualize informações de sobreposição comparando esses públicos com a contagem completa de população em todos os públicos ou com públicos específicos.

>[!TIP]
>
>Alguns dos números indicados na captura de tela nem sempre estão disponíveis para todos os públicos-alvo. A visibilidade depende da configuração escolhida pelo seu colaborador para um público na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility).

## Próximas etapas

Depois de explorar e descobrir os públicos-alvo desejados, é hora de [compartilhar](/help/guide/collaborate/share.md) os públicos-alvo que devem ser usados nas campanhas com o editor.
