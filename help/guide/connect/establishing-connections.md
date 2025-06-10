---
title: Conectar-se a anunciantes ou editores
description: Depois de descobrir possíveis colaboradores, saiba como estabelecer conexões e começar a colaborar em projetos.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: c9b96753a9a78bd85002ede3369c5f20eb430548
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 11%

---

# Conectar-se a anunciantes ou editores

{{limited-availability-release-note}}

Antes que os colaboradores (normalmente um anunciante e um editor) possam trabalhar juntos em campanhas, eles devem estabelecer uma conexão. Essa conexão permite que eles ativem públicos, criem projetos e executem relatórios sobre o desempenho da campanha.

## Fluxo de trabalho de alto nível

Para estabelecer uma conexão entre um anunciante e um editor, as seguintes etapas são necessárias:

1. O anunciante [navega por editores e descobre](/help/guide/connect/discover-publishers.md) um com o qual gostaria de trabalhar.
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

![O painel Conectar com a opção Conectar foi realçado em um editor específico.](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

Depois que o convite for enviado, você poderá visualizar (mas não editar) as configurações de conexão. Exibir convites pendentes na guia **[!UICONTROL Minhas conexões]**. O status da conexão aparece como **[!UICONTROL Convite enviado]**.

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
>abstract="Esta seção determina quem está pagando pelas atividades correspondentes no Real-Time CDP Collaboration."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Compartilhamento de público-alvo"
>abstract="Os créditos de ativação de público são consumidos com base no número de IDs correspondentes preparadas para ativação."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="Medição"
>abstract="Execute atividades para gerar relatórios e insights de desempenho da campanha. Os créditos são consumidos com base no número de linhas nos relatórios de campanha em todas as campanhas e na frequência dos relatórios (diariamente, a cada três dias ou semanalmente)."

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

### Configurações de conexão do anunciante {#advertiser-connection-settings}

Depois que seu colaborador aceitar a conexão, defina as configurações de conexão. Essas configurações definem os termos de colaboração, incluindo os casos de uso nos quais você trabalhará, as chaves de correspondência para projetos e outras configurações.

Para começar, navegue até **[!UICONTROL Minhas conexões]**. Para qualquer conexão com o status **[!UICONTROL Pendente]**, você pode selecionar **[!UICONTROL Configurar conexão]** para definir as configurações de conexão.

![O espaço de trabalho Minhas conexões com uma conexão Pendente e sua opção Configurar conexão foi realçada.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

É possível editar e definir os campos abaixo:

![O espaço de trabalho de configurações de conexão antes de ser preenchido.](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++Casos de uso

Os casos de uso são preenchidos previamente com todas as opções disponíveis. Para personalizá-los, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Casos de uso]** e desative os que não desejar. Os casos de uso selecionados determinam quais modos de exibição e opções estão [disponíveis em seus projetos](../collaborate/manage-projects.md#project-use-cases).

![As configurações de casos de uso no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++Teclas de correspondência

As chaves de correspondência são preenchidas previamente com aquelas que você selecionou ao [configurar sua organização](/help/guide/setup/onboard-organization.md#set-up-match-keys). Você pode desativar as chaves de correspondência que não deseja usar, mas não pode adicionar chaves de correspondência que não foram selecionadas durante a configuração da organização.

![As configurações da chave Corresponder no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++Divisão de crédito

Use a seção divisão de crédito para determinar qual das duas partes colaboradoras cobrirá os custos das atividades. As opções de divisão de crédito são determinadas pelos casos de uso selecionados para a conexão. Embora o caso de uso **[!UICONTROL Medição]** exija que uma parte cubra os custos, o caso de uso **[!UICONTROL Ativação - Correspondência]** oferece uma opção adicional para que cada parte cubra seus próprios custos. Para obter informações sobre o detalhamento de custos, leia o guia [tipos de atividade de crédito](/help/guide/setup/my-activity.md#types-of-activities).

>[!NOTE]
>
>Público-alvo - A saída é sempre coberta pelo colaborador que recebe o público-alvo, portanto, nenhuma seleção é necessária.

![A caixa de diálogo Divisão de crédito com opções no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}
+++

+++Contratos

Antes de prosseguir com essa conexão, você deve reconhecer que existe um acordo de compartilhamento de dados entre as duas partes.

![A seção Contrato legal é destacada e confirmada no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

Depois de fazer suas seleções, selecione **[!UICONTROL Enviar]** para enviar as configurações sugeridas ao seu colaborador para revisão.

### Configurações de conexão do editor {#publisher-connection-settings}

Em seguida, o editor precisa revisar as configurações de conexão e aceitá-las ou rejeitá-las. Para examinar as configurações de conexão, navegue até **[!UICONTROL Minhas conexões]** e selecione **[!UICONTROL Examinar configurações de conexão]** no cartão de conexão.

![A opção Revisar configurações de conexão foi realçada na exibição Minhas conexões.](/help/assets/connect/establish-connection/review-connection-settings.png){zoomable="yes"}

Revise as configurações propostas pelo colaborador. Antes de aceitar as configurações de conexão, você deve reconhecer que um contrato legal está em vigor entre você e o colaborador. Além disso, você pode adicionar qualquer nome de anunciante pelo qual o anunciante seja conhecido em seus sistemas.

![O espaço de trabalho de configurações de conexão com as configurações propostas do colaborador e das seções de Nomes e Contratos de Anunciante realçadas.](/help/assets/connect/establish-connection/publisher-connection-settings.png){zoomable="yes"}

+++Nomes do anunciante

Como editor trabalhando nas configurações de conexão, você pode optar por adicionar qualquer nome de anunciante pelo qual ele seja conhecido em seus sistemas. Como editor, você pode adicionar vários nomes de anunciante a uma conexão, por exemplo, em casos em que o anunciante com o qual você trabalha tem presença em várias regiões geográficas. Em uma parte posterior do processo, ao [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para colaborar, você ou seu colaborador poderão selecionar o nome do anunciante a ser associado ao projeto.

![A caixa de diálogo Nomes de anunciante no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/add-advertiser-names-modal.png)

Veja como a seleção de nome do anunciante funciona ao criar um projeto:

1. **Nenhum nome de anunciante definido**: se nenhum nome de anunciante for adicionado, o padrão da Real-Time CDP Collaboration será usar o nome do anunciante como o nome do anunciante.
2. **Um conjunto de nomes de anunciante**: se um único nome de anunciante for adicionado, o Real-Time CDP Collaboration usará automaticamente esse nome como o nome de anunciante do projeto.
3. **Conjunto de vários nomes de anunciante**: se mais de um nome de anunciante for adicionado, você ou seu colaborador poderá selecionar qualquer um dos nomes fornecidos ao criar o projeto.

![O espaço de trabalho de configurações de conexão com a seção de nomes de anunciante foi preenchida.](/help/assets/connect/establish-connection/advertiser-names.png)

+++

>[!NOTE]
>
> Depois de aceitar as configurações de conexão, você não poderá mais adicionar ou editar nomes de anunciante.

Se você estiver satisfeito com as configurações de conexão propostas, selecione **[!UICONTROL Aceitar]** para estabelecer a conexão. Se você deseja solicitar alterações nas configurações de conexão, selecione **[!UICONTROL Rejeitar]**. Em seguida, o colaborador pode revisar as configurações de conexão e reenviá-las para revisão.

## Excluir conexões {#delete-connections}

Você pode excluir qualquer conexão com colaboradores com os quais não deseja continuar trabalhando. Para excluir conexões existentes, navegue até **[!UICONTROL Conectar]**. Os anunciantes devem navegar para **[!UICONTROL Minhas conexões]**. Selecione **[!UICONTROL Exibir conexão]** no cartão de conexão para abrir a conexão que deseja excluir.

![A opção de conexão Exibir foi realçada na exibição Minhas conexões.](/help/assets/connect/establish-connection/delete-view-connection.png){zoomable="yes"}

Selecione o ícone de exclusão ![ícone de exclusão](/help/assets/common/delete.svg) no espaço de trabalho de conexão para excluir a conexão.

![O ícone de exclusão foi realçado no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

Uma caixa de diálogo de confirmação é exibida, solicitando que você confirme a exclusão da conexão. Selecione **[!UICONTROL Excluir]** para confirmar a exclusão.

![A caixa de diálogo de confirmação para excluir uma conexão.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Depois que a conexão for excluída, você não estará mais conectado ao colaborador e todos os projetos existentes que fazem parte da colaboração serão excluídos permanentemente e irrecuperáveis.

## Próximas etapas

Depois de estabelecer uma conexão com seu colaborador, você e ele agora podem [criar projetos](/help/guide/collaborate/manage-projects.md#create-project).
