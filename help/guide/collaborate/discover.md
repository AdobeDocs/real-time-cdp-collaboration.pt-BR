---
title: Descubra sobreposições e compare públicos
description: Descubra sobreposições entre o seu e o público-alvo de seus colaboradores. Saiba como descobrir os melhores públicos-alvo para usar em suas campanhas.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 20%

---

# Descubra sobreposições e compare públicos

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Descoberta]** só estará disponível se o caso de uso **Descoberta de público-alvo** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

Depois de [criar um projeto](/help/guide/collaborate/manage-projects.md), você pode comparar seus públicos com os de seus colaboradores. Isso ajuda a identificar públicos relevantes para campanhas e decidir quais enviar aos editores para ativação.

>[!IMPORTANT]
>
>Quaisquer [rascunhos de dados](/help/guide/glossary.md#sketches) que não forem atualizados ou atualizados serão excluídos após 7 dias. Quando isso acontece, os números exibidos nos vários relatórios de sobreposição nesta página vão para zero e o compartilhamento de público-alvo fica indisponível para esses públicos expirados. Os rascunhos de dados são atualizados automaticamente para públicos-alvo com um [cronograma de atualização ativo](/help/guide/setup/onboard-audiences.md#schedule).

As chaves de correspondência usadas para descobrir e comparar públicos estão configuradas [durante o processo de conexão](/help/guide/connect/establishing-connections.md#connection-settings). As teclas de correspondência são usadas para calcular a sobreposição entre os públicos, e podem ser ativadas e desativadas. Para editar as chaves de correspondência, selecione a opção **[!UICONTROL Editar chaves de correspondência]**.

![O espaço de trabalho da guia Descobrir, mostrando os insights do Público-alvo.](/help/assets/collaborate/discover/discover-overview.png)

A caixa de diálogo **[!UICONTROL Editar chaves de correspondência]** é aberta, onde você pode desativar as chaves de correspondência que não deseja usar. Selecione **[!UICONTROL Salvar]** para salvar suas alterações.

![A caixa de diálogo Editar chaves de correspondência no espaço de trabalho Descobrir.](/help/assets/collaborate/discover/edit-match-keys.png)

## Pré-requisitos {#prerequisites}

Para começar a usar a guia **[!UICONTROL Descobrir]** no seu projeto, você deve ter:

* [Públicos-alvo ](/help/guide/setup/onboard-audiences.md) originados na sua conta
* [Conectado](/help/guide/connect/establishing-connections.md) com um colaborador com o caso de uso **Descoberta de público-alvo** habilitado
* [Criou um projeto](/help/guide/collaborate/manage-projects.md) entre você e um colaborador

Depois que esses pré-requisitos forem atendidos, você poderá começar a explorar e comparar sobreposições entre você e os públicos do seu colaborador.

## Comparar públicos-alvo {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="Comparar públicos-alvo"
>abstract="Descubra sobreposições entre os seus públicos-alvo e os do seu colaborador. É possível ajustar as configurações no seletor suspenso para descobrir sobreposições entre um ou mais dos seus públicos-alvo em relação a um ou mais dos públicos-alvo do seu colaborador."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="Sua contagem de identidades"
>abstract="O número de IDs exclusivas no público-alvo selecionado, com base nas chaves de correspondência do projeto definidas por você e o(a) colaborador(a)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="Contagem de identidades do colaborador"
>abstract="O número de IDs exclusivas no público-alvo do(a) colaborador(a), com base nas chaves de correspondência do projeto que vocês definiram."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="Contagem de identidades sobrepostas"
>abstract="O número de IDs exclusivas que estão presentes no seu público-alvo e no do colaborador, com base nas chaves de correspondência do projeto com as quais você e o colaborador concordaram."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="Porcentagem de identidades sobrepostas"
>abstract="A porcentagem de sobreposição de identidades entre o público-alvo selecionado do colaborador e o seu."

Use a seção comparar públicos para obter informações detalhadas sobre a sobreposição entre os públicos do e do colaborador. Para alterar a seleção de público, use o seletor suspenso na parte superior da seção **[!UICONTROL Comparar públicos]**. Você pode selecionar um ou todos os públicos-alvo e um ou todos os públicos-alvo do colaborador para comparar.

![O espaço de trabalho Descobrir com o seletor de público-alvo realçado na seção Comparar públicos-alvo.](/help/assets/collaborate/discover/compare-audiences-selector.png)

Na seção comparar públicos, você pode ver as seguintes métricas, que se baseiam nas chaves de correspondência acordadas entre você e seu colaborador para o projeto:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Contagem de identidades]** (sua) | O número de IDs exclusivas dentro do(s) público(s) selecionado(s). |
| **[!UICONTROL Contagem de identidades]** (seu colaborador) | O número de IDs exclusivas no(s) público(s) do colaborador. |
| **[!UICONTROL Identidades sobrepostas]** | O número de IDs exclusivas presentes nos públicos do e do colaborador. |
| **[!UICONTROL Sobreposição %]** | A porcentagem de sobreposição de perfis entre o público alvo selecionado do seu colaborador e o seu. |
| **[!UICONTROL Detalhamento de identidades por chave de correspondência]** | O detalhamento de identidades para cada chave de correspondência escolhida no projeto, com base nos públicos selecionados para cada colaborador. |

{style="table-layout:auto"}

>[!NOTE]
>
>O índice de porcentagem de sobreposição nem sempre está disponível para todos os públicos-alvo. A visibilidade do indicador de porcentagem de sobreposição depende da configuração escolhida pelo seu colaborador para um público na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility).

## Públicos-alvo relevantes {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="Públicos-alvo relevantes"
>abstract="Com base nas porcentagens de sobreposição, esses públicos-alvo podem ser adequados para a campanha. <br><br>A <b>contagem de identidades</b> é o tamanho do público-alvo do colaborador. <br><br> As <b>identidades sobrepostas</b> representam a sobreposição entre o público-alvo recomendado e todos os seus públicos-alvo. <br><br> A <b>% de sobreposição</b> representa o número de identidades sobrepostas dividido pelo tamanho de <i>todos</i> os seus públicos-alvo."

A seção **[!UICONTROL Públicos-alvo relevantes]** da guia **[!UICONTROL Descobrir]** fornece uma lista com curadoria dos cinco principais públicos-alvo com base na porcentagem de sobreposição entre o público-alvo do seu colaborador e todos os seus públicos-alvo. Esse recurso ajuda você a identificar rapidamente os públicos-alvo com a maior sobreposição, permitindo direcionar suas campanhas com mais eficiência. Alterne entre os públicos-alvo relevantes usando os seletores de página na parte superior direita da seção.

![A seção Descobrir espaço de trabalho com os Públicos relevantes foi realçada.](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>A visibilidade dos públicos do colaborador depende da configuração escolhida por ele para um público na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility). Se o colaborador tiver definido todos os públicos-alvo como privados, esta seção não exibirá públicos-alvo.

A seção **[!UICONTROL Públicos relevantes]** exibe as seguintes informações para cada público recomendado:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Contagem de identidades]** | O nome das IDs exclusivas no público-alvo. |
| **[!UICONTROL Identidades sobrepostas]** | O número de IDs exclusivas que se sobrepõem entre o público-alvo recomendado e todos os públicos-alvo. |
| **[!UICONTROL Sobreposição %]** | A porcentagem de identidades sobrepostas entre o público-alvo recomendado e todos os públicos-alvo. |
| **[!UICONTROL Categorias de público-alvo]** | As categorias que seu colaborador atribuiu ao público-alvo. |
| **[!UICONTROL Chaves correspondentes]** | As chaves de correspondência que seu colaborador selecionou para o público-alvo. |

{style="table-layout:auto"}

## Descubra sobreposições {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="Descubra sobreposições com públicos-alvo individuais"
>abstract="Obtenha insights sobre as sobreposições entre os seus públicos-alvo e os públicos-alvo do colaborador."

Descubra sobreposições para obter insights sobre como os públicos-alvo se comparam com os públicos-alvo do colaborador. Por padrão, esta seção compara todos os públicos-alvo com cada um dos públicos-alvo do colaborador. Use o controle de paginação na parte inferior da seção para navegar pelos públicos disponíveis.

![O espaço de trabalho do Discover com a seção Descobrir sobreposições foi realçado.](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>A visibilidade dos públicos do colaborador depende da configuração escolhida por ele para um público na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility). Se o colaborador tiver definido todos os públicos-alvo como privados, esta seção não exibirá públicos-alvo.

Para alterar a seleção de público, selecione **[!UICONTROL Alterar público]**.

![O espaço de trabalho do Discover com a opção Alterar público-alvo foi realçado.](/help/assets/collaborate/discover/change-audience.png)

A caixa de diálogo **[!UICONTROL Alterar público-alvo]** é aberta, onde você pode selecionar um público-alvo específico para comparar com os públicos do seu colaborador. Selecione os públicos desejados ou desmarque suas seleções para selecionar todos os públicos e selecione **[!UICONTROL Salvar]**.

![A caixa de diálogo Alterar público-alvo no espaço de trabalho Descobrir.](/help/assets/collaborate/discover/change-audience-selection.png)

Depois de selecionar os públicos desejados, a seção **[!UICONTROL Descobrir sobreposições]** exibe as seguintes informações para cada público:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Contagem de identidades]** | O número de IDs exclusivas dentro do público-alvo. |
| **[!UICONTROL Identidades sobrepostas]** | O número de IDs exclusivas que se sobrepõem entre o público-alvo recomendado e todos os públicos-alvo. |
| **[!UICONTROL Sobreposição %]** | A porcentagem de identidades sobrepostas entre o público-alvo recomendado e todos os públicos-alvo. |
| **[!UICONTROL Categorias de público-alvo]** | As categorias que seu colaborador atribuiu ao público-alvo. |
| **[!UICONTROL Chaves correspondentes]** | As chaves de correspondência que seu colaborador selecionou para o público-alvo. |

{style="table-layout:auto"}

## Próximas etapas

Depois de explorar e descobrir os públicos-alvo desejados, é hora de [ativar](/help/guide/collaborate/activate.md) os públicos-alvo que devem ser usados nas campanhas.
