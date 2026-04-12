---
title: Descubra sobreposições e compare públicos
description: Descubra sobreposições entre o seu e o público-alvo de seus colaboradores. Saiba como descobrir os melhores públicos-alvo para usar em suas campanhas.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: 2cd03a98228e1e379396360942227ddbcab8f6ca
workflow-type: tm+mt
source-wordcount: '2120'
ht-degree: 17%

---

# Descubra sobreposições e compare públicos

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Descoberta]** só estará disponível se o caso de uso **Descoberta de público-alvo** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

Depois de [criar um projeto](/help/guide/collaborate/manage-projects.md), você pode comparar seus públicos com os de seus colaboradores. Isso ajuda a identificar públicos relevantes para campanhas e decidir quais enviar aos colaboradores para ativação.

>[!IMPORTANT]
>
>Quaisquer [rascunhos de dados](/help/guide/glossary.md#sketches) que não forem atualizados ou atualizados serão excluídos após 7 dias. Quando isso acontece, os números exibidos nos vários relatórios de sobreposição nesta página vão para zero e o compartilhamento de público-alvo fica indisponível para esses públicos expirados. Os rascunhos de dados são atualizados automaticamente para públicos-alvo com um [cronograma de atualização ativo](/help/guide/setup/onboard-audiences.md#schedule).

As chaves de correspondência usadas para descobrir e comparar públicos estão configuradas [durante o processo de conexão](/help/guide/connect/establishing-connections.md#connection-settings). As teclas de correspondência são usadas para calcular a sobreposição entre os públicos, e podem ser ativadas e desativadas. Para editar as chaves de correspondência, selecione a opção **[!UICONTROL Editar chaves de correspondência]**.

![O espaço de trabalho da guia Descobrir, mostrando os insights do Público-alvo.](/help/assets/collaborate/discover/discover-overview.png)

A caixa de diálogo **[!UICONTROL Editar chaves de correspondência]** é aberta, onde você pode desativar as chaves de correspondência que não deseja usar. Selecione **[!UICONTROL Salvar]** para salvar suas alterações.

![A caixa de diálogo Editar chaves de correspondência no espaço de trabalho Descobrir.](/help/assets/collaborate/discover/edit-match-keys.png)

## Pré-requisitos {#prerequisites}

Para começar a usar a guia **[!UICONTROL Descobrir]** no seu projeto, você deve ter:

* [Públicos-alvo &#x200B;](/help/guide/setup/onboard-audiences.md) originados na sua conta
* [Conectado](/help/guide/connect/establishing-connections.md) com um colaborador com o caso de uso **Descoberta de público-alvo** habilitado
* [Criou um projeto](/help/guide/collaborate/manage-projects.md) entre você e um colaborador

Depois que esses pré-requisitos forem atendidos, você poderá começar a explorar e comparar sobreposições entre você e os públicos do seu colaborador.

>[!NOTE]
>
>Este espaço de trabalho **[!UICONTROL Descobrir]** não é relevante para colaborações com plataformas de publicidade. Currently, Amazon Marketing Cloud is the only available advertising platform in Real-Time CDP Collaboration. For more information about the [!DNL AMC] **[!UICONTROL Discover]** workspace, read the [Amazon Marketing Cloud](/help/guide/collaborate/advertising-platforms/amc.md) guide.

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

Use the compare audiences section to get rich information about the overlap between your and your collaborator&#39;s audiences. To change the audience selection, use the dropdown selector at the top of the **[!UICONTROL Compare audiences]** section. You can select one or all of your audiences and one or all of your collaborator&#39;s audiences to compare against each other.

![The Discover workspace with the audience selector highlighted in the Compare audiences section.](/help/assets/collaborate/discover/compare-audiences-selector.png)

In the compare audiences section, you can see the following metrics, which are based on the match keys that you and your collaborator agreed on for the project:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Identity count]** (yours) | The number of unique IDs within your selected audience(s). |
| **[!UICONTROL Identity count]** (your collaborator) | The number of unique IDs within your collaborator&#39;s audience(s). |
| **[!UICONTROL Overlapping identities]** | The number of unique IDs that are present in both your and your collaborator&#39;s audiences. |
| **[!UICONTROL Overlap %]** | A porcentagem de sobreposição de perfis entre o público-alvo alvo selecionado do seu colaborador e o seu. |
| **[!UICONTROL Audience index]** | A score that indicates how strongly one audience relates to another based on underlying audience counts &amp; overlaps. To learn more about what the scores mean, read the [audience index score](#audience-index-score) section. Audience index scores are not available when comparing against your collaborator&#39;s baseline (all audiences). |
| **[!UICONTROL Identities breakdown by match key]** | The breakdown of identites matched for each match key chosen in the project, based on the select audiences for each collaborator. |

{style="table-layout:auto"}

>[!NOTE]
>
>The overlap percentage figure and audience index score may not be always available for all audiences. The visibility of the overlap percentage and audience index score depends on the setting that your collaborator chose for an audience in the [metadata visibility section](/help/guide/setup/onboard-audiences.md#metadata-visibility).

If your collaborator has not enabled either the audience index or the overlap percentage, the audience will not have any comparison data available.

## Públicos-alvo relevantes {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="Públicos-alvo relevantes"
>abstract="Com base nas porcentagens de sobreposição, esses públicos-alvo podem ser adequados para a campanha. <br><br> A <b>contagem de identidades</b> é o tamanho do público-alvo do colaborador. <br><br> As <b>identidades sobrepostas</b> representam a sobreposição entre o público-alvo recomendado e todos os seus públicos-alvo. <br><br> A <b>% de sobreposição</b> representa o número de identidades sobrepostas dividido pelo tamanho de <i>todos</i> os seus públicos-alvo."

The **[!UICONTROL Relevant audiences]** section in the **[!UICONTROL Discover]** tab provides a curated list of the top five audiences based on the overlap percentage between the your collaborator&#39;s audience, and all your audiences. This feature helps you quickly identify the audiences with the highest overlap, enabling you to target your campaigns more effectively. Alterne entre os públicos-alvo relevantes usando os seletores de página na parte superior direita da seção.

![A seção Descobrir espaço de trabalho com os Públicos relevantes foi realçada.](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>A visibilidade dos públicos do colaborador depende da configuração escolhida por ele para um público na [seção de acesso à conexão](/help/guide/setup/onboard-audiences.md#connection-access) e na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility). Se o colaborador tiver definido todos os públicos-alvo como privados, esta seção não exibirá públicos-alvo.

A seção **[!UICONTROL Públicos relevantes]** exibe as seguintes informações para cada público recomendado:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Contagem de identidades]** | O número de IDs exclusivas dentro do público-alvo. |
| **[!UICONTROL Identidades sobrepostas]** | O número de IDs exclusivas que se sobrepõem entre o público-alvo recomendado e todos os públicos-alvo. |
| **[!UICONTROL Sobreposição %]** | A porcentagem de identidades sobrepostas entre o público-alvo recomendado e todos os públicos-alvo. |
| **[!UICONTROL Índice de público-alvo]** | Uma pontuação que indica com que intensidade um público-alvo está relacionado a outro com base em contagem de público-alvo e sobreposições subjacentes. Para saber mais sobre o significado das pontuações, leia a seção [pontuação do índice de público-alvo](#audience-index-score). |
| **[!UICONTROL Categorias de público-alvo]** | As categorias que seu colaborador atribuiu ao público-alvo. |
| **[!UICONTROL Chaves correspondentes]** | As chaves de correspondência que seu colaborador selecionou para o público-alvo. |

{style="table-layout:auto"}

Se a pontuação do índice de público-alvo estiver habilitada para qualquer público-alvo do colaborador, os públicos relevantes serão baseados na pontuação do índice de público-alvo, e qualquer público-alvo no qual o índice de público-alvo não foi habilitado não será incluído. Os públicos-alvo relevantes com base na pontuação do índice de público-alvo são classificados para que a pontuação de índice mais alta seja exibida primeiro. Se o índice de público-alvo não estiver habilitado para qualquer público-alvo do colaborador, os públicos-alvo relevantes serão baseados na porcentagem de sobreposição.

## Descubra sobreposições {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="Descubra sobreposições com públicos-alvo individuais"
>abstract="Obtenha insights sobre as sobreposições entre os seus públicos-alvo e os públicos-alvo do colaborador."

Descubra sobreposições para obter insights sobre como os públicos-alvo se comparam com os públicos-alvo do colaborador. Por padrão, esta seção compara todos os públicos-alvo com cada um dos públicos-alvo do colaborador. Use o controle de paginação na parte inferior da seção para navegar pelos públicos disponíveis.

![O espaço de trabalho do Discover com a seção Descobrir sobreposições foi realçado.](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>A visibilidade dos públicos do colaborador depende da configuração escolhida por ele para um público na [seção de acesso à conexão](/help/guide/setup/onboard-audiences.md#connection-access) e na [seção de visibilidade de metadados](/help/guide/setup/onboard-audiences.md#metadata-visibility). Se o colaborador tiver definido todos os públicos-alvo como privados, esta seção não exibirá públicos-alvo.

Se o colaborador não tiver ativado o índice de público-alvo ou a porcentagem de sobreposição, o público-alvo não será exibido.

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
| **[!UICONTROL Índice de público-alvo]** | Uma pontuação que indica com que intensidade um público-alvo está relacionado a outro com base em contagem de público-alvo e sobreposições subjacentes. Para saber mais sobre o significado das pontuações, leia a seção [pontuação do índice de público-alvo](#audience-index-score). |
| **[!UICONTROL Categorias de público-alvo]** | As categorias que seu colaborador atribuiu ao público-alvo. |
| **[!UICONTROL Chaves correspondentes]** | As chaves de correspondência que seu colaborador selecionou para o público-alvo. |

{style="table-layout:auto"}

## Pontuação do índice de público-alvo {#audience-index-score}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_audience_index_score"
>title="Pontuação do índice de público-alvo"
>abstract="As pontuações do índice de público-alvo são uma métrica aprimorada que mostra o nível de relação entre um público-alvo e outro com base nas contagens e sobreposições subjacentes do público-alvo. A pontuação do índice bruta é traduzida em faixas de relevância, que categorizam as pontuações do índice de público-alvo de muito baixas até muito altas. Isso permite avaliar rapidamente a força da relação entre o seu público-alvo e o público-alvo do colaborador."

As pontuações do índice de público-alvo são uma métrica aprimorada que mostra o nível de relação entre um público-alvo e outro com base nas contagens e sobreposições subjacentes do público-alvo. Isso ajuda a contextualizar os insights do público-alvo e identificar públicos-alvo de alto potencial para prospecção e direcionamento de campanha.

A pontuação do índice é calculada usando a seguinte fórmula:

![A fórmula para calcular a pontuação do índice.](/help/assets/collaborate/discover/index-score-formula.png)

Imagine a car manufacturer wants to run an advertising campaign with a large CTV publisher for a new SUV model. The car manufacturer has data on who currently owns a similar model and wants to use that to find additional prospects to convert them to customers. The car manufacturer looks at the CTV publisher&#39;s audiences to find a relevant audience that closely matches the current SUV owners.

![The car advertiser versus the CTV publisher audiences.](/help/assets/collaborate/discover/audience-index-score-example.png)

Index score calculations are made and can be used to determine the likely success of the campaign:

| CTV Publisher Audience | Fórmula | Index Score (i) | Interpretação |
|------------------------|-------------|----------------|----------------|
| Baseline (all audiences) | ((1.3M / 1.3M) / (50M / 50M)) * 100 | 100 | This serves as the baseline against which your collaborator&#39;s other audiences are compared to. |
| Binge Watchers | ((500k / 1.3M) / (20M / 50M)) * 100 | 96 | By targeting this audience, you are 4% less likely to reach SUV owners compared to the baseline. |
| Comedy Lovers | ((200k / 1.3M) / (6M / 50M)) * 100 | 128 | By targeting this audience, you are 28% more likely to reach SUV owners compared to the baseline. |
| Males 25-34 | ((700k / 1.3M) / (12M / 50M)) * 100 | 224 | By targeting this audience, you are 124% more likely to reach SUV owners compared to the baseline. |
| Tech Enthusiasts | ((500k / 1.3M) / (8M / 50M)) * 100 | 240 | By targeting this audience, you are 140% more likely to reach SUV owners compared to the baseline. |

{style="table-layout:auto"}

To better understand how the index scores will impact your campaign, relevance bands are provided alongside the scores.

### Relevance bands {#audience-index-relevance-bands}

To enable easy comparison across different audiences and campaigns, Collaboration translates the index scores into relevance bands (very low to very high). Isso permite avaliar rapidamente a força da relação entre o seu público-alvo e o público-alvo do colaborador.

| Pontuação do índice (i) | Faixa de Relevância | Descrição |
|---------------|----------|-----------|
| i &lt; 60 | Muito baixo | A sobreposição é muito menos prevalente no público-alvo em comparação ao seu público-alvo, indicando um relacionamento muito fraco. Os clientes que usam esse público-alvo têm muito menos probabilidade de alcançar seu público-alvo. |
| 60 &lt; i &lt; 80 | Baixo | A sobreposição é um pouco menos prevalente no público-alvo em comparação ao seu público-alvo, sugerindo um relacionamento fraco. Os clientes que usam esse público-alvo têm menos probabilidade de alcançar o público-alvo. |
| 80 &lt; i &lt; 120 | Médio | A sobreposição é tão prevalente no público-alvo quanto no seu público-alvo, indicando uma relação típica. Os clientes que usam esse público-alvo têm uma probabilidade média de alcançar seu público-alvo. |
| 120 &lt; i &lt; 140 | Alto | A sobreposição é mais prevalente no público-alvo em comparação ao seu público-alvo, mostrando uma relação forte. Os clientes que usam esse público-alvo têm mais probabilidade de alcançar o público-alvo. |
| i > 140 | Muito alto | A sobreposição é muito mais prevalente no público-alvo em comparação ao seu público-alvo, refletindo uma relação muito forte. Os clientes que usam esse público-alvo têm muito mais probabilidade de alcançar o público-alvo. |

{style="table-layout:auto"}

Na seção descobrir sobreposições, a pontuação do índice de público-alvo exibirá a faixa de relevância ao lado da pontuação. A pontuação será codificada por cores para indicar a faixa de relevância, facilitando a identificação da força do relacionamento num relance. As faixas de relevância muito baixa e baixa são exibidas em laranja, as faixas de relevância média em preto e as faixas de relevância alta e muito alta em verde.

## Próximas etapas

Depois de explorar e descobrir os públicos-alvo desejados, é hora de [ativar](/help/guide/collaborate/activate.md) os públicos-alvo que devem ser usados nas campanhas.
