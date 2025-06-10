---
title: Ativar públicos-alvo
description: Saiba como ativar públicos no Adobe Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: 691161cdc1f9338a470373988fbc0dee9a5be6db
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# Ativar públicos-alvo

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Ativar]** só estará disponível se o caso de uso **Ativação de público-alvo** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

A ativação de público permite ativar públicos em campanhas. O processo de atividade é uma colaboração entre anunciantes e editores. Depois de [descobrir os melhores públicos-alvo para sua campanha](./discover.md), os públicos-alvo podem ativar os públicos-alvo direcionados. Os públicos ativados são enviados para o destino pré-configurado do editor, como o Adobe Experience Platform, para uso em campanhas. Para obter mais informações sobre como configurar o destino, consulte o guia [visão geral dos destinos](../destinations/overview.md).

>[!IMPORTANT]
>
>Atualmente, quando os anunciantes ativam os públicos-alvo, eles são ativados automaticamente para o destino do publicador configurado para sua organização. O publicador **deve** configurar um destino *antes* de o anunciante ativar um público-alvo. Se nenhum destino estiver configurado, o público-alvo será enviado para o editor, mas não poderá ser ativado em nenhuma campanha.

## Ativar novos públicos

Para começar a ativar públicos, navegue até a guia **[!UICONTROL Ativar]** no espaço de trabalho do projeto.

Selecione o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)) ou a opção **[!UICONTROL Ativar público-alvo]** se nenhum público-alvo anterior tiver sido enviado para ativação.

![O espaço de trabalho Ativar em um projeto sem públicos adicionados.](/help/assets/collaborate/activate/activate-new-audiences.png)

O fluxo de trabalho ativar públicos-alvo é aberto, onde você pode selecionar o público-alvo que deseja enviar para o colaborador. Use a lista suspensa para selecionar um público ou pesquise por um público específico. Para ver mais informações sobre os públicos-alvo antes de fazer sua seleção, selecione **[!UICONTROL Procurar públicos-alvo]**

![O fluxo de trabalho de ativação de Público-alvo com as opções suspensa e Procurar públicos-alvo foi realçado.](/help/assets/collaborate/activate/audience-activation.png)

Em **[!UICONTROL Procurar públicos-alvo]**, você pode ver a **[!UICONTROL Contagem de identidades]**, **[!UICONTROL Identidades sobrepostas]** e **[!UICONTROL Sobreposição %]** para cada público-alvo.

![A caixa de diálogo Procurar públicos-alvo mostrando os públicos-alvo disponíveis.](/help/assets/collaborate/activate/browse-audiences.png)

Selecione o público que você deseja ativar nas campanhas e selecione **[!UICONTROL Salvar]**. O público agora é exibido e você pode ver a **[!UICONTROL Contagem de identidades]**, **[!UICONTROL Identidades sobrepostas]** e **[!UICONTROL Sobreposição %]** para o público selecionado.

![O fluxo de trabalho de ativação de público-alvo com o público-alvo selecionado foi exibido.](/help/assets/collaborate/activate/audience-selected.png)

### Editar chaves de correspondência

Em seguida, você pode editar as chaves de correspondência do público selecionando **[!UICONTROL Editar chaves de correspondência]** no público selecionado. Essas opções são herdadas de suas seleções de chave de correspondência quando a conexão entre colaboradores foi configurada inicialmente. Você pode remover as chaves de correspondência que foram selecionadas se elas não se aplicarem a uma campanha específica, mas não pode adicionar novas chaves de correspondência.

![O fluxo de trabalho de ativação de público-alvo com a opção Editar chaves de correspondência foi realçado.](/help/assets/collaborate/activate/edit-match-keys.png)

A caixa de diálogo **[!UICONTROL Editar chaves de correspondência]** é aberta, onde você pode desativar as chaves de correspondência que não deseja usar. Selecione **[!UICONTROL Salvar]** para salvar suas alterações.

>[!NOTE]
>
>Pelo menos uma chave de correspondência deve ser selecionada. Na versão atual, as únicas chaves de correspondência disponíveis são **[!UICONTROL email com hash]**, portanto, você não pode remover essa chave de correspondência.

![A caixa de diálogo Editar chaves de correspondência no fluxo de trabalho de ativação do Público-alvo.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Definir frequência e intervalo de atualização do público-alvo

Por fim, defina a frequência e o intervalo de datas desejados para o público-alvo ser atualizado. Na versão atual, a única opção de frequência com suporte é **[!UICONTROL Uma Vez]**. A frequência **[!UICONTROL Once]** significa que os públicos-alvo são ativados uma única vez e não são atualizados. A opção **[!UICONTROL Data]** é preenchida automaticamente com a data atual.

![O fluxo de trabalho de ativação de público-alvo com a seção Frequência realçada.](/help/assets/collaborate/activate/audience-frequency.png)

Quando satisfeito com suas seleções, selecione **[!UICONTROL Ativar]** para concluir o fluxo de trabalho. O público-alvo agora está ativado e você pode visualizá-lo na guia **[!UICONTROL Ativar]**. Ele também estará disponível para o colaborador na guia **[!UICONTROL Ativar]**, onde ele poderá usá-lo em campanhas.

Você pode editar o ícone de edição do nome do público-alvo (![Ícone de lápis.](/help/assets/icons/edit.png)) ou desative o público selecionando **[!UICONTROL Desativar]**.

![A guia Ativar com o público-alvo ativado foi exibida e as opções Editar e Desativar foram realçadas.](/help/assets/collaborate/activate/edit-activate-audience.png)

## Exibir públicos ativados

Na guia **[!UICONTROL Ativar]**, tanto editores quanto anunciantes podem exibir os públicos-alvo ativados no momento. Atualmente, os públicos-alvo são enviados automaticamente para o destino configurado do editor depois que o anunciante os ativa.

![Visão geral da guia Ativar, mostrando um público ativado.](/help/assets/collaborate/activate/activate-overview.png)

Em cada público ativado, você pode ver as seguintes métricas:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Identidades ativadas]** | Indica o número de identidades ativadas no público. |
| **[!UICONTROL Identidades sobrepostas]** | Indica o número de identidades sobrepostas entre esse público-alvo e a população total de perfis no inventário do colaborador. |
| **[!UICONTROL Detalhamento de chave de correspondência]** | Mostra a contagem de identidades para cada identidade usada no público-alvo. Por exemplo, uma contagem total de identidade de 500 mil usuários pode consistir em 400 mil usuários que ignoraram a identidade de email com hash e 100 mil usuários ignoraram uma identidade de ID móvel. Observe que no exemplo descrito aqui, a mesma pessoa pode estar presente no público-alvo duas vezes com suas identidades de email e de ID de dispositivo móvel. |

## Próximas etapas {#next-steps}

Após ativar os dados e executar as campanhas, trabalhe com a equipe de capacitação e engenharia do Adobe para carregar os dados de medição e exibir os [relatórios de medição](/help/guide/collaborate/measure.md) correspondentes.
