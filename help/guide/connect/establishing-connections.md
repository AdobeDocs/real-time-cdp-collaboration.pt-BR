---
title: Conectar-se a anunciantes ou editores
description: Depois de descobrir possíveis colaboradores, saiba como estabelecer conexões e começar a colaborar em projetos.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 17%

---

# Conectar-se a anunciantes ou editores

{{limited-availability-release-note}}

Estabelecer uma conexão entre duas partes de uma colaboração (geralmente um anunciante e um editor) é o pré-requisito no Real-Time CDP Collaboration para empresas que trabalham juntas em campanhas. Tanto editores quanto anunciantes podem configurar conexões. O participante que iniciar a conexão será o *proprietário da conexão*.

## Fluxo de trabalho de alto nível

Em um alto nível, para estabelecer uma conexão entre um anunciante e um editor, o fluxo de trabalho se parece com o abaixo:

1. O anunciante [procura editores e descobre](/help/guide/connect/discover-publishers.md) um com o qual gostaria de trabalhar
2. O anunciante envia um convite de conexão.
3. O editor aceita o convite.
4. O anunciante envia configurações de conexão, incluindo chaves de correspondência e outras. Essas configurações de conexão representam os termos no produto da colaboração.
5. O editor aceita configurações de conexão. Se desejar, o editor pode rejeitar as configurações de conexão iniciais e solicitar que o anunciante envie configurações de conexão revisadas.

![Diagrama de alto nível do processo de conexão anunciante-publicador.](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png){zoomable="yes"}

Quando os itens acima forem concluídos, os colaboradores poderão prosseguir para [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para [executar relatórios de sobreposição](/help/guide/collaborate/discover.md) e iniciar campanhas publicitárias.

>[!IMPORTANT]
>
>Depois que a conexão entre dois colaboradores for estabelecida, as configurações de conexão não poderão mais ser revisadas.

## Enviar convite {#send-invite}

Para configurar uma conexão, selecione **[!UICONTROL Conectar]** ao navegar pelo inventário de fornecedores na tela de descoberta de editores.

![Seletor de conexão](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

Neste ponto, o convite está fora e você pode visualizar as configurações de conexão, mas não pode editá-las. Você pode exibir o convite pendente na guia **[!UICONTROL Minhas conexões]**. O status da conexão é **[!UICONTROL Convite enviado]**.

![Convite pendente enviado ao editor exibido no modo de exibição Minhas conexões.](/help/assets/connect/establish-connection/pending-invite-sent.png){zoomable="yes"}

Depois que o colaborador aceitar o convite, você poderá definir as configurações de conexão e enviá-las ao colaborador para revisar e aceitar.

## Configurações de conexão {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="Casos de uso"
>abstract="Os casos de uso são preenchidos previamente com todas as opções. É possível editar os casos de uso antes de enviar as configurações de conexão."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="Chaves de correspondência"
>abstract="As chaves de correspondência são preenchidas previamente com aquelas que você selecionou no nível organizacional. É possível desativar qualquer chave de correspondência que não quiser usar nesta conexão."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="Divisão de crédito"
>abstract="Esta seção determina quem está pagando pelas atividades correspondentes na Real-Time CDP Collaboration. Atualmente, somente o caso de uso de compartilhamento de público-alvo é configurável."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Compartilhamento de público-alvo"
>abstract="O Compartilhamento de público-alvo é a atividade que uma parte realiza ao solicitar que os dados correspondentes sejam ativados pelo parceiro de colaboração."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="Medição"
>abstract="Esse caso de uso permite executar atividades na Real-Time CDP Collaboration para gerar relatórios e insights de desempenho da campanha."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="Contrato legal"
>abstract="Verifique se existe um contrato de compartilhamento de dados entre as duas partes."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="Nomes do anunciante"
>abstract="<p>Configuração opcional. Indica o nome e a ID pelos quais o editor conhece o anunciante.</p><p>O nome do anunciante adicionado aqui será preenchido previamente na etapa de criação do projeto.</p><ul><li>Se o editor tiver configurado vários nomes, selecione um deles na lista.</li><li>Se apenas um nome tiver sido configurado, ele será pré-selecionado automaticamente.</li><li>Se nenhum nome tiver sido configurado, o campo será preenchido previamente com o nome da conta do anunciante da Real-Time CDP Collaboration.</li></ul>"
>additional-url="https://experienceleague.adobe.com/pt-br/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="Criar um projeto"

Depois que o convite for enviado, você poderá visualizar as configurações de conexão. O convite deve ser aceito antes que você possa concluir a configuração da conexão.

![A exibição das configurações de conexão no estado de visualização.](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

Depois que a conexão for aceita pelo colaborador, você poderá começar a definir as configurações de conexão para a conexão. As configurações de conexão definem os termos de sua colaboração, como os casos de uso que você realizará juntos, as chaves de correspondência que usará em projetos e muito mais.

Para definir e compartilhar configurações de conexão com seu colaborador, navegue até **[!UICONTROL Minhas conexões]**. Para qualquer conexão com o status **[!UICONTROL Pendente]**, você pode selecionar **[!UICONTROL Configurar conexão]** para definir as configurações de conexão.

![A exibição Minhas conexões com uma conexão Pendente e sua opção Configurar conexão foi realçada.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

É possível editar e definir os campos abaixo:

![Configurar exibição de conexão](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++Casos de uso

Os casos de uso são preenchidos previamente com todos os casos de uso disponíveis. Você pode escolher quais casos de uso sua conexão usará ao selecionar **[!UICONTROL Editar]** e desativar todos os casos de uso que não desejar. Os casos de uso selecionados afetarão quais modos de exibição e opções estão [disponíveis em seus projetos](../collaborate/manage-projects.md#project-use-cases).

![Casos de uso](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++Teclas de correspondência

As chaves de correspondência são preenchidas previamente com aquelas que você [selecionou no seu nível organizacional](/help/guide/setup/onboard-organization.md#set-up-match-keys). Você pode desativar as chaves de correspondência que não deseja usar nesta conexão, mas não pode adicionar chaves de correspondência que não foram selecionadas ao configurar a organização.

![Chaves correspondentes](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++Divisão de crédito

Use a seção divisão de crédito para determinar qual das duas partes colaboradoras cobrirá os custos das atividades. As opções de divisão de crédito são determinadas pelos casos de uso selecionados para a conexão. Embora o caso de uso **[!UICONTROL Medição]** exija que uma parte cubra os custos, o caso de uso **[!UICONTROL Ativação de público-alvo]** oferece uma opção adicional para que cada parte cubra seus próprios custos. Para obter informações sobre o detalhamento de custos, leia o guia [tipos de atividade de crédito](/help/guide/setup/my-activity.md#types-of-activities).

>[!NOTE]
>
>Público-alvo - A saída é sempre coberta pelo colaborador que recebe o público-alvo, portanto, nenhuma seleção é necessária.

![A caixa de diálogo Divisão de crédito com opções no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}
+++

+++Contratos

Antes de prosseguir com essa conexão, você deve reconhecer que existe um acordo de compartilhamento de dados entre as duas partes.

![Contratos legais.](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

+++Nomes do anunciante

Como editor trabalhando nas configurações de conexão, você pode optar por adicionar qualquer nome de anunciante pelo qual ele seja conhecido em seus sistemas. Como editor, você pode adicionar vários nomes de anunciante a uma conexão, por exemplo, em casos em que o anunciante com o qual você trabalha tem presença em várias regiões geográficas. Em uma parte posterior do processo, ao [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para colaborar, você ou seu colaborador poderão selecionar o nome do anunciante a ser associado ao projeto.

![Adicionar modal de nomes de anunciante.](/help/assets/connect/establish-connection/add-advertiser-names-modal.png)

Veja como a seleção de nome do anunciante funciona ao criar um projeto:

1. **Nenhum nome de anunciante definido**: se nenhum nome de anunciante for adicionado, o padrão da Real-Time CDP Collaboration será usar o nome do anunciante como o nome do anunciante.
2. **Um conjunto de nomes de anunciante**: se um único nome de anunciante for adicionado, o Real-Time CDP Collaboration usará automaticamente esse nome como o nome de anunciante do projeto.
3. **Conjunto de vários nomes de anunciante**: se mais de um nome de anunciante for adicionado, você ou seu colaborador poderá selecionar qualquer um dos nomes fornecidos ao criar o projeto.

![Nomes do anunciante.](/help/assets/connect/establish-connection/advertiser-names.png)

+++

Depois de fazer sua seleção, selecione **[!UICONTROL Enviar]** para enviar as configurações sugeridas ao seu colaborador para revisão.

Se você estiver recebendo configurações de conexão propostas do seu colaborador, é possível **[!UICONTROL Aceitar]** ou **[!UICONTROL Rejeitar]** essas configurações. Antes de aceitar as configurações de conexão, você precisa reconhecer e confirmar que um contrato legal está em vigor entre você e o colaborador. Se você estiver rejeitando configurações de conexão, entre em contato com seu colaborador fora do produto e discuta como ele deve revisar as configurações de conexão para que você as aceite.

## Excluir conexões {#delete-connections}

Você pode excluir qualquer conexão com colaboradores com os quais não deseja continuar trabalhando. Para excluir conexões existentes:

1. Navegue até **[!UICONTROL Conectar]** > **[!UICONTROL Minhas conexões]**.
2. Selecione **[!UICONTROL Exibir conexão]** no cartão de conexão para acessar a conexão que deseja excluir.
3. Selecione o ícone de exclusão ![ícone de exclusão](/help/assets/common/delete.svg) para abrir a caixa de diálogo de confirmação de exclusão da conexão.
   ![Ícone de exclusão de conexão realçado.](/help/assets/connect/establish-connection/delete-icon-highlighted.png){zoomable="yes"}
4. Confirme a exclusão selecionando **[!UICONTROL Excluir]**.
   ![Diálogo para confirmar a exclusão de uma conexão. ](/help/assets/connect/establish-connection/delete-connection-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Depois que a conexão for excluída, você não estará mais conectado ao colaborador e todos os projetos existentes que fazem parte da colaboração serão excluídos permanentemente e irrecuperáveis.

## Próximas etapas

Depois de estabelecer uma conexão com seu colaborador, você e ele agora podem [criar projetos](/help/guide/collaborate/manage-projects.md#create-project).
