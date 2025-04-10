---
title: Conectar-se a anunciantes ou editores
description: Depois de descobrir possíveis colaboradores, saiba como estabelecer conexões e começar a colaborar em projetos.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: 81cedb2a06d930734b1f97304de82d450c06bf79
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 1%

---

# Conectar-se a anunciantes ou editores

{{limited-availability-release-note}}

Estabelecer uma conexão entre duas partes de uma colaboração (geralmente um anunciante e um editor) é o pré-requisito no Real-Time CDP Collaboration para empresas que trabalham juntas em campanhas. Tanto editores quanto anunciantes podem configurar conexões. O participante que iniciar a conexão será o *proprietário da conexão*.

## Fluxo de trabalho de alto nível

Em um alto nível, para estabelecer uma conexão entre um anunciante e um editor, o fluxo de trabalho se parece com o abaixo:

1. O anunciante [procura editores e descobre](/help/guide/connect/discover-publishers.md) um com o qual gostaria de trabalhar
2. O anunciante envia um convite de conexão.
3. A editor aceita o convite.
4. O anunciante envia configurações de conexão, incluindo chaves de correspondência e outras. Essas configurações de conexão representam os termos no produto do colaboração.
5. A editor aceita as configurações de conexão. Se desejado, o editor pode rejeitar as configurações iniciais de conexão e solicitação que a anunciante envie configurações de conexão revisadas.

![Diagrama de alto nível do processo de conexão editor com anunciante níveis.](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png)

Quando os itens acima forem concluídos, os colaboradores poderão prosseguir para [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para [executar relatórios de sobreposição](/help/guide/collaborate/discover.md) e iniciar campanhas publicitárias.

>[!IMPORTANT]
>
>Depois que a conexão entre dois colaboradores for estabelecida, as configurações de conexão não poderão mais ser revisadas.

## Enviar convite {#send-invite}

Para configurar uma conexão, selecione **[!UICONTROL Conectar]** ao navegar no editor inventário na tela do editor Discover.

![Conecte-se seletor](/help/assets/connect/establish-connection/connect-selection.png)

Neste ponto, o convite está fora e você pode visualizar as configurações de conexão, mas não pode editá-las. Você pode exibir o convite pendente na guia **[!UICONTROL Minhas conexões]**. O status da conexão é **[!UICONTROL Convite enviado]**.

![Convite pendente enviado ao editor exibido no modo de exibição Minhas conexões.](/help/assets/connect/establish-connection/pending-invite-sent.png)

Depois que o colaborador aceitar o convite, você poderá definir as configurações de conexão e enviá-las ao colaborador para revisar e aceitar.

## Configurações de conexão {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="Casos de uso"
>abstract="Os casos de uso são preenchidos previamente com todas as opções. Você pode editar os casos de uso antes de enviar as configurações de conexão."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="Coincidir chaves"
>abstract="As chaves de correspondência são pré-preenchidas com aquelas que você selecionou no nível organizacional. Você pode desativar qualquer chave de correspondência que não quiser usar nesta conexão."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="Divisão de crédito"
>abstract="Esta seção determina quem está pagando pelas atividades correspondentes na Colaboração CDP em tempo real. Atualmente, somente o público-alvo caso de uso de compartilhamento está configurável."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Compartilhamento de público"
>abstract="O compartilhamento de público-alvo é o atividade que uma parte toma ao solicitar que seus dados correspondentes sejam ativados por seus parceiro de colaboração."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="Contrato legal"
>abstract="Verifique se existe um contrato de compartilhamento de dados entre as duas partes."

Depois que o convite for enviado, você poderá visualizar as configurações de conexão. O convite deve ser aceito antes que você possa concluir a configuração da conexão.

![As configurações de conexão visualização no estado pré-visualização.](/help/assets/connect/establish-connection/preview-connection-settings.png)

Depois que a conexão for aceita pelo seu colaborador, agora você pode start configurar as configurações de conexão para a conexão. As configurações de conexão definem os termos do seu colaboração, como os casos de uso que você realizará em conjunto, as teclas de correspondência que você usará em projetos e muito mais.

Para configurar e compartilhar configurações de conexão com seu colaborador, navegue até **[!UICONTROL Minhas conexões]**. Para qualquer conexão com o status **[!UICONTROL pendente]**, é possível selecionar **[!UICONTROL Configurar conexão]** para definir as configurações de conexão.

![A exibição Minhas conexões com uma conexão Pendente e sua opção Configurar conexão foi realçada.](/help/assets/connect/establish-connection/pending-connection.png)

É possível editar e definir os campos abaixo:

![Configurar exibição de conexão](/help/assets/connect/establish-connection/connection-view.png)

+++Casos de uso

Os casos de uso são preenchidos previamente com todos os casos de uso disponíveis. Você pode escolher quais casos de uso sua conexão usará ao selecionar **[!UICONTROL Editar]** e desativar todos os casos de uso que não desejar. Os casos de uso selecionados afetarão quais modos de exibição e opções estão [disponíveis em seus projetos](../collaborate/manage-projects.md#project-use-cases).

![Casos de uso](/help/assets/connect/establish-connection/view-use-cases.png)

+++

+++Chaves de correspondência

As chaves de correspondência são preenchidas previamente com as que você [selecionou em seu nível organizacional](/help/guide/setup/onboard-organization.md#set-up-match-keys). É possível desativar as teclas de correspondência que não deseja usar nessa conexão, mas não é possível adicionar teclas de correspondência que não foram selecionadas ao configurar a organização.

![Chaves de correspondência](/help/assets/connect/establish-connection/match-keys.png)

+++

+++Divisão de crédito

Use a seção divisão de crédito para determinar qual das duas partes colaboradoras cobrirá os custos das atividades.

![Divisão de crédito](/help/assets/connect/establish-connection/edit-billing-ownership.png)

+++

+++Contratos

Antes de prosseguir com essa conexão, você deve reconhecer que existe um acordo de compartilhamento de dados entre as duas partes.

![Acordos legais.](/help/assets/connect/establish-connection/legal-agreement.png)

+++

Depois de fazer sua seleção, selecione **[!UICONTROL Enviar]** para enviar as configurações sugeridas ao seu colaborador para revisão.

Se você estiver recebendo configurações de conexão propostas do seu colaborador, é possível **[!UICONTROL Aceitar]** ou **[!UICONTROL Rejeitar]** essas configurações. Antes de aceitar as configurações de conexão, você precisa reconhecer e confirmar que um contrato legal está em vigor entre você e o colaborador. Se você estiver rejeitando configurações de conexão, entre em contato com seu colaborador fora do produto e discuta como ele deve revisar as configurações de conexão para que você as aceite.

## Excluir conexões {#delete-connections}

Você pode excluir qualquer conexão com colaboradores com os quais não deseja continuar trabalhando. Para excluir conexões existentes:

1. Navegue até **[!UICONTROL Conectar]** > **[!UICONTROL Minhas conexões]**.
2. Selecione **[!UICONTROL Exibir conexão]** no cartão de conexão para acessar a conexão que deseja excluir.
3. Selecione o ícone de exclusão ![ícone de exclusão](/help/assets/common/delete.svg) para abrir a caixa de diálogo de confirmação de exclusão da conexão.
   ![Ícone de exclusão de conexão realçado.](/help/assets/connect/establish-connection/delete-icon-highlighted.png)
4. Confirme a exclusão selecionando **[!UICONTROL Excluir]**.
   ![Diálogo para confirmar a exclusão de uma conexão. ](/help/assets/connect/establish-connection/delete-connection-dialog.png)

>[!WARNING]
>
>Quando a conexão for excluída, você não estará mais conectado com o colaborador e todos os projetos existentes que fazem parte da colaboração serão permanentemente excluídos e irrecuperáveis.

## Próximas etapas

Depois de estabelecer uma conexão com seu colaborador, você e seu colaborador agora [podem criar projetos](/help/guide/collaborate/manage-projects.md#create-project).
