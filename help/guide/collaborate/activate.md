---
title: Ativar públicos-alvo
description: Saiba como ativar públicos no Adobe Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: a7215d453021be578a32ce1af4d659845c3b8493
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 2%

---

# Ativar públicos-alvo

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Ativar]** só estará disponível se o caso de uso **Ativação de público-alvo** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

A ativação de público permite ativar públicos para uso em campanhas. A ativação pode ser feita por qualquer um dos colaboradores, dependendo das configurações de ativação de público-alvo [definidas na conexão](/help/guide/connect/establishing-connections.md#configure-connection-settings). Depois que você [descobrir os melhores públicos-alvo da sua campanha](./discover.md), ative os públicos-alvo para disponibilizá-los para uso. Quando você ativa um público-alvo, ele é enviado para o destino pré-configurado do colaborador, como o Adobe Experience Platform, onde fica disponível para uso em campanhas. Para obter mais informações sobre como configurar destinos, consulte o guia [visão geral dos destinos](../destinations/overview.md).

## Ativar novos públicos {#activate-new-audiences}

Para começar a ativar públicos, navegue até a guia **[!UICONTROL Ativar]** no espaço de trabalho do projeto.

>[!IMPORTANT]
>
>**Antes** de ativar um público-alvo, seu colaborador **deve** configurar um destino. Quando você ativa um público-alvo, ele é enviado automaticamente para o destino configurado do colaborador. Se nenhum destino estiver configurado, não será possível ativar os públicos-alvo.
>
>![O espaço de trabalho Ativar quando o colaborador não tiver um destino configurado.](/help/assets/collaborate/activate/no-destination-configured.png)

Selecione o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)) ou a opção **[!UICONTROL Ativar público-alvo]** se nenhum público-alvo anterior tiver sido enviado para ativação.

![O espaço de trabalho Ativar em um projeto sem públicos adicionados.](/help/assets/collaborate/activate/activate-new-audiences.png)

O fluxo de trabalho ativar públicos-alvo é aberto, onde você pode selecionar o público-alvo que deseja enviar para o colaborador. Use a lista suspensa para selecionar um público ou pesquise por um público específico. Para ver mais informações sobre os públicos-alvo antes de fazer sua seleção, selecione **[!UICONTROL Procurar públicos-alvo]**

![O fluxo de trabalho de ativação de Público-alvo com as opções suspensa e Procurar públicos-alvo foi realçado.](/help/assets/collaborate/activate/audience-activation.png)

Em **[!UICONTROL Procurar públicos-alvo]**, você pode ver a **[!UICONTROL Contagem de identidades]**, **[!UICONTROL Identidades sobrepostas]** e **[!UICONTROL Sobreposição %]** para cada público-alvo.

![A caixa de diálogo Procurar públicos-alvo mostrando os públicos-alvo disponíveis.](/help/assets/collaborate/activate/browse-audiences.png)

Selecione o público que você deseja ativar nas campanhas e selecione **[!UICONTROL Salvar]**. O público agora é exibido e você pode ver a **[!UICONTROL Contagem de identidades]**, **[!UICONTROL Identidades sobrepostas]** e **[!UICONTROL Sobreposição %]** para o público selecionado.

![O fluxo de trabalho de ativação de público-alvo com o público-alvo selecionado foi exibido.](/help/assets/collaborate/activate/audience-selected.png)

### Editar chaves de correspondência {#edit-match-keys}

Em seguida, você pode editar as chaves de correspondência do público selecionando **[!UICONTROL Editar chaves de correspondência]** no público selecionado. Essas opções são herdadas de suas seleções de chave de correspondência quando a conexão entre colaboradores foi configurada inicialmente. Você pode remover as chaves de correspondência que foram selecionadas se elas não se aplicarem a uma campanha específica, mas não pode adicionar novas chaves de correspondência.

![O fluxo de trabalho de ativação de público-alvo com a opção Editar chaves de correspondência foi realçado.](/help/assets/collaborate/activate/edit-match-keys.png)

A caixa de diálogo **[!UICONTROL Editar chaves de correspondência]** é aberta, onde você pode desativar as chaves de correspondência que não deseja usar. Selecione **[!UICONTROL Salvar]** para salvar suas alterações.

>[!NOTE]
>
>Pelo menos uma chave de correspondência deve ser selecionada. Na versão atual, as únicas chaves de correspondência disponíveis são **[!UICONTROL email com hash]**, portanto, você não pode remover essa chave de correspondência.

![A caixa de diálogo Editar chaves de correspondência no fluxo de trabalho de ativação do Público-alvo.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Definir a frequência de atualização do público {#set-audience-refresh-frequency}

Por fim, defina a frequência e o intervalo de datas desejados para o público-alvo ser atualizado. Na versão atual, a única opção de frequência com suporte é **[!UICONTROL Uma Vez]**. A frequência **[!UICONTROL Once]** significa que os públicos-alvo são ativados uma única vez e não são atualizados. A opção **[!UICONTROL Data]** é preenchida automaticamente com a data atual.

![O fluxo de trabalho de ativação de público-alvo com a seção Frequência realçada.](/help/assets/collaborate/activate/audience-frequency.png)

Quando satisfeito com suas seleções, selecione **[!UICONTROL Ativar]** para concluir o fluxo de trabalho.

## Ativar painel {#activate-dashboard}

Na guia **[!UICONTROL Ativar]**, é possível exibir todos os públicos-alvo enviados ao colaborador, bem como todos os públicos-alvo que o colaborador ativou para o destino.

![O painel Ativar mostrando as seções Públicos enviados e Públicos ativados.](/help/assets/collaborate/activate/activate-dashboard.png)

## Exibir públicos-alvo enviados {#view-sent-audiences}

Na seção **[!UICONTROL Públicos-alvo enviados para o]** collaborator, todos os públicos-alvo enviados serão listados. Atualmente, os públicos-alvo são enviados automaticamente para o destino configurado do colaborador depois que você os envia. Na exibição do seu colaborador, esses públicos são exibidos na seção **[!UICONTROL Públicos ativados]**.

Em cada público-alvo enviado, você pode ver as seguintes métricas:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Nome]** | O nome do público. |
| **[!UICONTROL Status]** | O status do público-alvo enviado. |
| **[!UICONTROL Contagem de identidades]** | O número de identidades no público-alvo. |
| **[!UICONTROL Identidades sobrepostas]** | O número de identidades sobrepostas entre esse público-alvo e a população total de perfis no inventário do colaborador. |
| **[!UICONTROL Criado]** | A data em que o público-alvo foi enviado inicialmente. |
| **[!UICONTROL Último envio]** | A data em que o público-alvo foi enviado pela última vez para o colaborador. |
| **[!UICONTROL Chaves correspondentes]** | Indica a chave de correspondência usada para o público-alvo. |

## Exibir públicos ativados {#view-activated-audiences}

Na seção **[!UICONTROL Públicos ativados]**, você pode ver todos os públicos que foram ativados para o seu destino.

Em cada público ativado, você pode ver as seguintes métricas:

| Métrica | Descrição |
|---------|----------|
| **[!UICONTROL Nome]** | O nome do público. |
| **[!UICONTROL Status]** | O status do público-alvo ativado. |
| **[!UICONTROL Contagem de identidades]** | O número de identidades que foram ativadas, com base nas identidades sobrepostas quando seu colaborador enviou o público. |
| **[!UICONTROL Criado]** | A data em que o público-alvo foi ativado. |
| **[!UICONTROL Última atualização]** | A data em que o público-alvo foi atualizado pela última vez, com base no agendamento de atualização escolhido durante a ativação. |
| **[!UICONTROL Destino]** | O destino onde o público-alvo foi ativado. |
| **[!UICONTROL Chaves correspondentes]** | Indica a chave de correspondência usada para o público-alvo. |

## Excluir públicos-alvo enviados {#delete-sent-audiences}

Você pode excluir os públicos-alvo enviados que não deseja mais ativar. Ao excluir um público-alvo enviado, ele é removido da seção **[!UICONTROL Públicos-alvo enviados para]** e não será mais ativado para o destino do seu colaborador.

Para excluir um público-alvo enviado, selecione o ícone **[!UICONTROL Excluir]** (![Ícone Excluir.](/help/assets/icons/delete.png)) ao lado do público-alvo na seção **[!UICONTROL Públicos-alvo enviados para]**.

![A opção Excluir na seção Públicos enviados.](/help/assets/collaborate/activate/delete-sent-audiences.png)

Uma caixa de diálogo de confirmação é aberta, solicitando que você confirme a exclusão. Selecione **[!UICONTROL Excluir]** para confirmar.

![A caixa de diálogo de confirmação Excluir.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## Próximas etapas {#next-steps}

Após ativar os públicos-alvo e executar campanhas, trabalhe com a equipe de capacitação e engenharia do Adobe para carregar dados de medição e exibir os [relatórios de medição](/help/guide/collaborate/measure.md) correspondentes.
