---
title: Compartilhar públicos
description: Saiba como compartilhar públicos com seus colaboradores para campanhas publicitárias.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0fdf0598-89c9-452d-a2e3-ce868df0b9d2
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 6%

---

# Compartilhar públicos

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Compartilhamento]** só estará disponível se o caso de uso **Compartilhamento e ativação de público** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

Como anunciante, saiba como compartilhar públicos com seus editores para que eles possam executar campanhas. Se sua colaboração tiver habilitado o caso de uso **Descobrir públicos-alvo**, comece executando relatórios de sobreposição na [guia Descobrir](/help/guide/collaborate/discover.md) para identificar os melhores públicos-alvo para compartilhamento.

## Compartilhar novos públicos

Para começar a compartilhar públicos, navegue até a guia **[!UICONTROL Compartilhar]** no espaço de trabalho do projeto. Somente **organizações de anunciantes** podem compartilhar públicos para campanhas. Nesta guia, é possível revisar e gerenciar públicos-alvo compartilhados.

Selecione a opção **Mais símbolo (+)** ou **[!UICONTROL Compartilhar público-alvo]** se nenhum público-alvo anterior tiver sido compartilhado, para iniciar o processo de compartilhamento do público-alvo.

![Modo de exibição padrão sem públicos-alvo compartilhados.](/help/assets/collaborate/share/share-new-audiences.png)

Um novo painel é exibido, onde você pode selecionar os públicos que deseja compartilhar com seu colaborador.

![Compartilhar novo fluxo de trabalho de públicos-alvo.](/help/assets/collaborate/share/share-audiences-workflow.png)

### Selecionar públicos-alvo para compartilhar

Na janela de seleção de público, procure por públicos-alvo específicos para compartilhar inserindo o nome do público-alvo na barra de pesquisa. Selecione **[!UICONTROL Procurar públicos-alvo]** e use as opções de classificação disponíveis para encontrar os públicos-alvo exatos de que você precisa.

![Procurar exibição de públicos com públicos selecionados.](/help/assets/collaborate/share/browse-audiences-view.png)

### Editar chaves de correspondência e definir opções de direcionamento

Depois de selecionar os públicos-alvo desejados para compartilhamento, você pode selecionar outras opções de configuração para a atividade de compartilhamento.

![Editar chaves de correspondência e destino ou suprimir seletor realçado](/help/assets/collaborate/share/match-keys-and-targeting.png)

Selecione **[!UICONTROL Editar chaves de correspondência]** para indicar quais chaves de correspondência devem ser usadas para as identidades no público-alvo. Essas opções são herdadas das configurações que foram selecionadas quando a conexão entre colaboradores foi inicialmente configurada. Você pode remover as chaves de correspondência que foram selecionadas nesse momento se elas não se aplicarem a essa campanha específica, mas não é possível adicionar novas chaves de correspondência nesse momento.

![Editar chaves de correspondência.](/help/assets/collaborate/share/update-match-keys.png)

Para cada público, selecione se deseja que os membros desse público sejam direcionados ou suprimidos na campanha. Os perfis suprimidos não farão especificamente parte do público-alvo ativado pelo editor.

### Definir frequência e intervalo de atualização do público-alvo

Por fim, defina a frequência e o intervalo de datas desejados para a atualização do público-alvo. Os modos atualmente permitidos para atualização de público são **[!UICONTROL Uma vez]** e **[!UICONTROL Diariamente]**.

Ao selecionar **[!UICONTROL Uma vez]**, a associação de público-alvo não é atualizada durante toda a duração de uma campanha. Ao selecionar **[!UICONTROL Diariamente]**, a associação de público é atualizada uma vez por dia durante toda a duração de uma campanha.

![Opções de frequência realçadas.](/help/assets/collaborate/share/audience-refresh-frequency.png)

Quando estiver satisfeito com suas seleções, selecione **[!UICONTROL Compartilhar]** para concluir o fluxo de trabalho.

>[!SUCCESS]
>
>Você pode ver uma nova atividade de compartilhamento de público na guia **[!UICONTROL Compartilhamento]**. Se desejar, você pode voltar e editar qualquer seleção feita.

## Exibir públicos compartilhados no momento

Na guia **[!UICONTROL Compartilhamento]**, é possível exibir os públicos-alvo que estão sendo compartilhados entre os colaboradores, agrupados em atividades de compartilhamento de público-alvo.

![Visão geral da guia de compartilhamento.](/help/assets/collaborate/share/share-tab-overview.png)

<!--

The banner at the top of the page shows figures across all audience sharing activities. 

![The hero banner in the sharing tab.](/help/assets/collaborate/share/share-hero-banner.png)


|Metric | Description |
|---------|----------|
| **[!UICONTROL Shared audiences]** | Indicates the number of audiences shared between collaborators in this project, across all audience sharing modules. |
| **[!UICONTROL Estimated addressable reach]** | Indicates the approximate number of profiles that you can reach across all the audiences that are currently shared in the project. [TODO: ADD INFORMATION ABOUT HOW THIS IS CALCULATED] |
| **[!UICONTROL Target identities]** | The number of identities across all audiences shared in this project for which you selected to target the profiles. |
| **[!UICONTROL Suppress identities]** | The number of identities across all audiences shared in this project for which you selected to suppress the profiles and thereby not target them in campaigns. |

-->

Em cada atividade de compartilhamento de público, você pode obter informações sobre cada público compartilhado.

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Contagem de identidades]** | Indica o número de perfis em todas as identidades vinculadas a esse público, de acordo com a última avaliação de contagem de identidades. Esses números são atualizados a cada 24 horas. |
| **[!UICONTROL Identidades sobrepostas]** | Indica o número de identidades sobrepostas entre os membros deste público e a população total de perfis no inventário do colaborador. |
| **[!UICONTROL Detalhamento de chave de correspondência]** | Mostra a contagem de identidades para cada identidade usada no público-alvo. Por exemplo, uma contagem total de identidade de 500 mil usuários pode consistir em 400 mil usuários que ignoraram a identidade de email com hash e 100 mil usuários ignoraram uma identidade de ID móvel. Observe que no exemplo descrito aqui, a mesma pessoa pode estar presente no público-alvo duas vezes com suas identidades de email e de ID de dispositivo móvel. |
| **[!UICONTROL Objetivo]** | **[!UICONTROL Suprimir]** ou **[!UICONTROL Destino]**. Indica se os membros de um público-alvo devem ser alvos ou excluídos de campanhas. |

A página também fornece controles para você **[!UICONTROL Pausar o compartilhamento]** e **[!UICONTROL Editar públicos-alvo]**.

## Editar públicos-alvo {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="Direcionar ou suprimir caso de uso"
>abstract="<p>Selecione **Direcionar** se deseja exibir anúncios da campanha aos perfis no público-alvo.</p> <p>Selecione **Suprimir** se deseja excluir os perfis no público-alvo das mensagens da campanha.</p>"

Selecione **[!UICONTROL Editar públicos-alvo]** para alterar quais públicos-alvo são compartilhados em um módulo de compartilhamento de público-alvo, bem como para alterar várias configurações relacionadas ao modo como os públicos-alvo estão sendo compartilhados.

![Exibição do modal de edição de públicos-alvo](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## Próximas etapas

Depois que o editor receber os públicos-alvo compartilhados, ele [os ativará](/help/guide/collaborate/activate.md) em campanhas de publicidade digital.
