---
title: Gerenciar conexões
description: Saiba como gerenciar suas conexões no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 50120839-4a20-4ec1-8887-9342bd17c52d
TQID: https://experienceleague.adobe.com/plolWAj37G7hiH7gMYxDwJJDVXAIfMhSQHPRypErbxw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1092
ht-degree: 1%

---

# Gerenciar conexões {#manage-connections}

{{limited-availability-release-note}}

O espaço de trabalho **[!UICONTROL Minhas conexões]** fornece um local centralizado para gerenciar suas conexões. Você pode exibir conexões existentes na seção **[!UICONTROL Conexões existentes]** e ver todas as conexões que exigem uma ação na seção **[!UICONTROL Ação necessária]**.

## Visualizar conexão {#view-connection}

Para exibir suas conexões existentes, navegue até o espaço de trabalho **[!UICONTROL Conectar]**. Como editor, sua conexão existente será exibida. Como anunciante, você deve navegar até **[!UICONTROL Minhas conexões]**.

![A opção Exibir conexão foi realçada para uma conexão no espaço de trabalho Minhas conexões.](/help/assets/connect/manage-connections/view-connection.png){zoomable="yes"}

A área de trabalho de visão geral da conexão é exibida, mostrando detalhes sobre a conexão e seus projetos ativos. Selecione **[!UICONTROL Configurações de conexão]** para exibir as configurações de conexão.

![A opção Configurações de conexão foi realçada no espaço de trabalho de visão geral da conexão.](/help/assets/connect/manage-connections/connection-overview.png){zoomable="yes"}

O espaço de trabalho de configurações de conexão é exibido, exibindo os detalhes da conexão entre você e seu colaborador. Aqui, você pode exibir todas as configurações selecionadas durante o processo de conexão, o status atual da conexão, o proprietário da conexão e as informações de contato do seu colaborador. Para obter informações sobre configurações de conexão específicas, consulte o guia [configurações de conexão](/help/guide/connect/establishing-connections.md#connection-settings).

![O espaço de trabalho de configurações de conexão exibindo detalhes da conexão.](/help/assets/connect/manage-connections/connection-settings.png){zoomable="yes"}

## Excluir conexão {#delete-connection}

Você pode excluir qualquer conexão com colaboradores com os quais não deseja continuar trabalhando. Para excluir uma conexão, navegue até a conexão que deseja excluir e selecione o ícone de exclusão ![ícone de exclusão](/help/assets/common/delete.svg) no espaço de trabalho de conexão.

![O ícone de exclusão foi realçado no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

Uma caixa de diálogo de confirmação é exibida, solicitando que você confirme a exclusão da conexão. Selecione **[!UICONTROL Excluir]** para confirmar a exclusão.

![A caixa de diálogo de confirmação para excluir uma conexão.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Depois que a conexão for excluída, todos os projetos existentes na colaboração serão permanentemente excluídos e irrecuperáveis. A solicitação de conexão permanecerá em um estado pendente na seção **[!UICONTROL Ação necessária]** em **[!UICONTROL Minhas conexões]**, mas a conexão e suas configurações não estarão mais ativas. Você precisará restabelecer a conexão se quiser se conectar com o colaborador novamente.

## Editar conexão {#edit-connection}

Como proprietário de uma conexão de colaboração, você poderá editar as configurações de conexão com seu colaborador depois que a conexão for estabelecida. É possível:

* Adicionar casos de uso
* Adicionar chaves de correspondência. A remoção da chave de correspondência será suportada no futuro.
* Atualizar permissões de ativação de público
* Atualizar configurações de divisão de crédito

>[!IMPORTANT]
>
>Depois que um caso de uso ou chave de correspondência é adicionado a uma conexão, ele não pode ser removido.

>[!TIP]
>
>O **proprietário** é o colaborador que inicia a conexão enviando o convite para o **destinatário**. Para obter mais informações, consulte a [documentação sobre estabelecimento de conexões com colaboradores](./establishing-connections.md).

Para editar configurações de conexão, navegue até o espaço de trabalho de configurações de conexão. Selecione o ícone de três pontos (![ícone de três pontos.](/help/assets/icons/more.png)) para exibir as ações disponíveis, selecione **[!UICONTROL Editar]**.

![O espaço de trabalho de configurações de conexão com a opção Editar realçada.](/help/assets/connect/manage-connections/edit-connection.png){zoomable="yes"}

Uma caixa de diálogo é exibida, solicitando que você edite e envie as alterações de configuração para revisão do colaborador. Selecione **[!UICONTROL Editar]**.

![A caixa de diálogo Editar configurações de conexão com a opção Editar foi realçada.](/help/assets/connect/manage-connections/edit-connection-settings-dialog.png){zoomable="yes"}

### Editar ativação de público {#edit-audience-activation}

As configurações de ativação de público-alvo determinam qual colaborador na conexão pode ativar públicos-alvo para destinos. Para alterar essas configurações, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Ativação de público-alvo]**.

![A tela Editar configurações de conexão mostrando a seção de ativação de público-alvo e a opção Editar.](/help/assets/connect/manage-connections/edit-audience-activation.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL Ativação de público-alvo]**, use o menu suspenso para atualizar as permissões de ativação de público-alvo. Você pode escolher um único colaborador ou permitir que ambos os colaboradores ativem públicos.

![O menu suspenso de realce da caixa de diálogo de ativação de público-alvo foi expandido para atualizar as permissões de ativação de público-alvo.](/help/assets/connect/manage-connections/audience-activation-dropdown-menu.png){zoomable="yes"}

Depois de concluído, selecione **[!UICONTROL Salvar]**.

![A caixa de diálogo de ativação de público-alvo mostrando as novas permissões de ativação de público-alvo e a opção Salvar.](/help/assets/connect/manage-connections/audience-activation-dialog.png){zoomable="yes"}

### Adicionar casos de uso {#add-use-cases}

No Collaboration, casos de uso como Detectar, Ativar e Medir determinam quais seções e recursos do projeto você pode usar com seu colaborador. Você pode adicionar outros casos de uso a uma conexão existente para projetos futuros. Para obter mais informações, consulte [casos de uso de colaboração](../overview/use-cases.md).

Para adicionar novos casos de uso, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Casos de uso]**.

![A tela de configurações da conexão de edição destacando a seção de Casos de uso e a opção Editar.](/help/assets/connect/manage-connections/edit-use-cases.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL Casos de uso]**, alterne para novos casos de uso que deseja adicionar, seguido por **[!UICONTROL Salvar]**.

![A caixa de diálogo Casos de uso exibindo a opção Salvar foi realçada.](/help/assets/connect/manage-connections/use-cases-dialog.png){zoomable="yes"}

>[!NOTE]
>
>Ao [adicionar novos casos de uso](#add-use-cases), como &quot;Ativação de público-alvo&quot; ou &quot;Medição&quot;, a tela de edição de configurações de conexão é atualizada para incluir as seções **[!UICONTROL Ativação de público-alvo]** e **[!UICONTROL Divisão de crédito]**. Você deve definir as configurações apropriadas para esses novos casos de uso. Para obter mais detalhes, consulte os guias [ativação de público](../connect/establishing-connections.md#audience-activation) e [divisão de crédito](../connect/establishing-connections.md#credit-split).
>
>![A tela Editar configurações de conexão exibindo as seções Ativação de público-alvo e Divisão de crédito após a adição de novos casos de uso.](/help/assets/connect/manage-connections/setup-audience-activation-credit-split.png){zoomable="yes"}

### Adicionar chaves de correspondência {#add-match-keys}

Somente as chaves de correspondência configuradas em sua conta e também selecionadas pelo colaborador estão disponíveis para a conexão. Depois que você [adicionar novas chaves de correspondência à sua conta](../setup/onboard-account.md#edit-match-keys) e seu colaborador também selecionar as mesmas chaves, você poderá habilitá-las em suas conexões existentes.

Na tela editar configurações da conexão, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Chaves de correspondência]**.

![A tela de edição de configurações de conexão destacando a seção Corresponder chaves e a opção Editar.](/help/assets/connect/manage-connections/edit-connection-match-keys.png){zoomable="yes"}

Uma caixa de diálogo **[!UICONTROL Chaves de correspondência]** é exibida, mostrando as chaves de correspondência existentes configuradas para a conexão. Selecione as chaves de correspondência que deseja adicionar, seguidas por **[!UICONTROL Salvar]**.

![A caixa de diálogo Chaves de correspondência exibindo as novas chaves de correspondência selecionadas e a opção Salvar.](/help/assets/connect/manage-connections/connection-match-keys-dialog.png){zoomable="yes"}

### Editar divisão de crédito {#edit-credit-split}

As configurações de divisão de crédito especificam qual colaborador é responsável pelos custos associados a cada caso de uso na conexão. Para atualizar essas configurações, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Divisão de crédito]**.

![A tela de configurações da conexão de edição destacando a seção Divisão de crédito e a opção Editar.](/help/assets/connect/manage-connections/edit-credit-split.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL Divisão de crédito]**, selecione as configurações preferenciais para [!UICONTROL Correspondência de Ativação] e [!UICONTROL Medição]. Em seguida, selecione **[!UICONTROL Salvar]** para confirmar.

![The Credit split dialog showing the credit split settings and the Save option.](/help/assets/connect/manage-connections/credit-split-dialog.png){zoomable="yes"}

### Review and submit changes {#review-and-submit-changes}

When you complete editing the connection settings, review and select **[!UICONTROL Submit changes]**. The connection settings updates will be sent to your collaborator for review.

![The edit connection settings screen displaying the updates and the Submit changes option.](/help/assets/connect/manage-connections/review-and-submit-changes.png){zoomable="yes"}

#### Save connection settings changes as draft

You can save the connection settings changes as a draft and return to finish updating the connection settings at any time.

To save the changes as a draft, select **[!UICONTROL Cancel]** next to **[!UICONTROL Submit changes]**. Then, in the **[!UICONTROL Unsubmitted changes]** dialog, select **[!UICONTROL Continue later]** to confirm.

![The edit connection settings screen.](/help/assets/connect/manage-connections/unsubmitted-changes-dialog.png){zoomable="yes"}

Your changes are now saved as a draft. In the connection settings workspace, you can see a notification indicating that there are unsubmitted changes. To make further updates, select **[!UICONTROL Continue editing]**.

![A notification in the connection settings workspace showing there are unsubmitted changes pending review and submission.](/help/assets/connect/manage-connections/continue-editing-connection.png){zoomable="yes"}
