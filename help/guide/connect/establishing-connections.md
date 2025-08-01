---
title: Estabelecimento de conexões
description: Depois de descobrir possíveis colaboradores, saiba como estabelecer conexões e começar a colaborar em projetos.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: d460cb12b43b6c250a5fb491c1efc223c53abb23
workflow-type: tm+mt
source-wordcount: '3213'
ht-degree: 7%

---

# Estabelecimento de conexões

{{limited-availability-release-note}}

Antes que os colaboradores possam trabalhar juntos em campanhas, eles devem estabelecer uma conexão. Essa conexão permite que eles ativem públicos, criem projetos e executem relatórios sobre o desempenho da campanha.

As conexões são estabelecidas com base no padrão de colaboração escolhido. A Collaboration oferece suporte a dois principais padrões de colaboração: anunciante-editor e marca-a-marca. Para ler mais sobre esses padrões, consulte o guia [casos de uso](/help/guide/overview/use-cases.md).

<!-- REPLACE THE LINK ABOVE WITH THE CORRECT LINK AFTER PAGE IS ESTABLISHED -->

Para saber como estabelecer uma conexão, leia a seção abaixo que corresponde ao seu padrão de colaboração:

- [Conexão do anunciante com o editor](#advertiser-to-publisher-connection)
- [Conexão marca a marca](#brand-to-brand-connection)

## Conexão do anunciante com o editor {#advertiser-to-publisher-connection}

![Diagrama de alto nível do processo de conexão anunciante-publicador.](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

No padrão anunciante para editor, um anunciante descobre um editor com o qual deseja trabalhar por meio do espaço de trabalho **[!UICONTROL Descobrir editores]** e envia um convite de conexão. O editor então revisa o convite e o aceita, permitindo que o anunciante proponha configurações de conexão. Quando o editor aceita as configurações de conexão, a conexão é estabelecida e ambos os colaboradores podem começar a trabalhar juntos nos projetos.

### Visão geral de alto nível

Para estabelecer uma conexão entre um anunciante e um editor, as seguintes etapas estão envolvidas:

1. [Descobrir editores](#discover-publishers): o anunciante identifica possíveis editores com os quais colaborar.
1. [Enviar convite](#send-invite): o anunciante envia um convite de conexão para o editor selecionado.
1. [Aceitar convite](#accept-invite): o editor revisa e aceita o convite.
1. [Definir configurações de conexão](#configure-connection-settings): o anunciante define as configurações de conexão e as envia ao editor para revisão.
1. [Confirmar configurações de conexão](#establish-connection): o publicador revisa as configurações de conexão e as aceita ou rejeita. Se aceita, a conexão é estabelecida. Se rejeitado, o editor pode fornecer feedback para revisões fora do produto. O anunciante poderá então revisar as configurações e reenviá-las para revisão.

Depois que as configurações de conexão forem aceitas, a conexão será estabelecida e os colaboradores estarão prontos para [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para começar a colaborar em campanhas.

## Conexão marca a marca {#brand-to-brand-connection}

![Diagrama de alto nível do processo de conexão marca a marca.](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>O termo **marca** é usado para se referir a uma empresa ou marca fora da Collaboration. O termo **colaborador** se refere a qualquer conta que possa formar uma conexão no Collaboration, independentemente de ser um anunciante ou um editor.

No padrão marca a marca, duas marcas que se comunicaram fora do produto podem se conectar diretamente ao Collaboration usando um [convite de conexão privada](#private-connection-invite). Uma marca pode ser um anunciante ou um editor. Esse padrão é particularmente útil para marcas que podem não se encaixar no modelo tradicional de anunciante-editor, como dois anunciantes ou dois editores.

Para começar, um colaborador envia um convite de conexão privada para outro colaborador. O recipient revisa o convite e o aceita, permitindo que o proprietário proponha configurações de conexão. Depois que o recipient aceitar as configurações de conexão, a conexão será estabelecida e ambos os colaboradores poderão começar a trabalhar juntos nos projetos.

### Visão geral de alto nível

>[!TIP]
>
>Ao discutir o processo de conexão, haverá uma distinção entre **proprietário** e **destinatário**. O proprietário é o colaborador que inicia a conexão enviando o convite, enquanto o destinatário é o colaborador que recebe e revisa o convite.

O processo de conexão entre duas marcas envolve várias etapas. Antes de o processo de conexão começar, alguns pré-requisitos devem ser atendidos:

1. Duas marcas se comunicam fora do produto para discutir a conexão potencial.
1. As marcas [criam contas](/help/guide/setup/onboard-account.md) na Collaboration, se ainda não o fizeram, certificando-se de selecionar o tipo de função apropriado (anunciante ou editor).

   Depois que os pré-requisitos forem atendidos, o processo de conexão poderá ser iniciado. As etapas a seguir descrevem o processo:

1. [Enviar convite de conexão privada](#send-private-connection-invite): um colaborador envia um convite de conexão privada para outro colaborador.
1. [Aceitar convite de conexão privada](#accept-private-connection-invite): o destinatário revisa e aceita o convite de conexão privada.
1. [Definir configurações de conexão](#configure-connection-settings): o proprietário define as configurações de conexão e as envia ao destinatário para revisão e aceitação.
1. [Confirmar configurações da conexão](#establish-connection): o destinatário revisa as configurações da conexão e as aceita ou rejeita.

Depois que as configurações de conexão forem aceitas, a conexão será estabelecida e os colaboradores estarão prontos para [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para começar a colaborar em campanhas.

## Conectar {#connect}

O espaço de trabalho **[!UICONTROL Conectar]** é onde você pode gerenciar suas conexões com colaboradores, enviar convites de conexão e onde os anunciantes podem navegar pelo diretório do editor. O espaço de trabalho é dividido em duas guias principais:

### Descobrir editores {#discover-publishers}

>[!IMPORTANT]
>
>Somente anunciantes podem descobrir editores usando o espaço de trabalho **[!UICONTROL Descobrir editores]**. Para saber mais sobre como se conectar com colaboradores, independentemente da função deles, leia a seção [conexão marca a marca](#brand-to-brand-connection).

Para descobrir editores, navegue até o espaço de trabalho **[!UICONTROL Descobrir editores]** na guia **[!UICONTROL Conectar]**. Aqui, você pode navegar pela lista de editores disponíveis usando os controles de paginação na parte inferior do espaço de trabalho. Para saber mais sobre o espaço de trabalho **[!UICONTROL Descobrir editores]**, consulte o guia [descobrir editores](/help/guide/connect/discover-publishers.md).

![O espaço de trabalho de editores do Discover está exibindo uma lista de editores disponíveis.](/help/assets/connect/establish-connection/discover-publishers.png){zoomable="yes"}

### Enviar convite {#send-invite}

>[!IMPORTANT]
>
>Esta seção descreve o processo de envio de convites de conexão por anunciantes para editores por meio do espaço de trabalho **[!UICONTROL Descobrir editores]**. Para saber mais sobre como formar conexões entre marcas, independentemente de suas funções, leia a seção [conexão marca a marca](#brand-to-brand-connection) ou visite a seção [convite de conexão privada](#private-connection-invite).

Depois de identificar o fornecedor com o qual deseja colaborar, selecione a opção **[!UICONTROL Conectar]** no cartão do fornecedor. Esta ação inicia o processo de conexão.

![A opção Conectar foi realçada em um editor específico no espaço de trabalho Descobrir editores.](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

Uma caixa de diálogo é exibida, solicitando que você envie um convite de conexão para o editor. Selecione **[!UICONTROL Enviar convite]** para continuar.

![A caixa de diálogo Enviar convite de conexão com o botão Enviar convite está realçada.](/help/assets/connect/establish-connection/send-connection-invite-dialog.png){zoomable="yes"}

>[!NOTE]
>
>Se quiser se conectar com um fornecedor com quem se comunicou fora do produto, use a opção de convite de conexão privada. Para saber mais, consulte a seção [convite de conexão privada](#private-connection-invite).

O convite pendente é exibido na guia **[!UICONTROL Minhas conexões]** na seção **[!UICONTROL Ação necessária]**. O status da conexão aparece como **[!UICONTROL Convite enviado]**. Você pode visualizar as configurações de conexão selecionando **[!UICONTROL Visualizar conexão]**, mas não pode editá-las até que o editor aceite o convite.

![A conexão pendente é exibida no espaço de trabalho Minhas conexões na seção Ação necessária.](/help/assets/connect/establish-connection/preview-connection.png){zoomable="yes"}

### Convite de conexão privada {#private-connection-invite}

Convites de conexão privada permitem que você se conecte com colaboradores com os quais você se comunicou fora do produto usando um **[!UICONTROL Código de conexão]**. Para formar uma conexão privada, você precisa obter o **[!UICONTROL Código de conexão]** do colaborador com o qual deseja se conectar fora do produto. Você pode usar este código para enviar um convite de conexão privada ao colaborador no espaço de trabalho **[!UICONTROL Connect]**.

#### Código de conexão {#connect-code}

Antes de enviar um convite de conexão privada, o colaborador desejado deve fornecer o **[!UICONTROL Código de conexão]** exclusivo. Para localizar e copiar seu **[!UICONTROL Código de conexão]**, navegue até a guia **[!UICONTROL Minha conta]** no espaço de trabalho **[!UICONTROL Configuração]**. O **[!UICONTROL Código de conexão]** é exibido nos detalhes da sua conta.

![A guia Minha conta no espaço de trabalho Instalação com o código Conectar realçado.](/help/assets/connect/establish-connection/connect-code.png){zoomable="yes"}

Selecione o ícone de cópia (![ícone de cópia](/help/assets/icons/copy.png)) ao lado do **[!UICONTROL Código de conexão]** para copiá-lo para a área de transferência. Em seguida, você pode compartilhar esse código com seu colaborador fora do produto.

![O código Connect com o ícone de cópia está realçado.](/help/assets/connect/establish-connection/copy-connect-code.png){zoomable="yes"}

##### Atualizando o código de conexão {#refresh-connect-code}

Você pode atualizar o **[!UICONTROL Código de conexão]** a qualquer momento. Atualizar o código gera um novo código exclusivo que pode ser compartilhado com os colaboradores. Isso é útil se você quiser invalidar o código anterior por motivos de segurança. Quaisquer conexões estabelecidas usando o código antigo permanecerão ativas, mas os novos colaboradores precisarão usar o novo código para se conectarem com você.

>[!IMPORTANT]
>
>Atualizar o **[!UICONTROL Código de conexão]** durante um convite pendente pode impedir que o convite seja aceito. Se você atualizar seu código, talvez seu colaborador precise reenviar o convite de conexão privada usando o novo código.

Para atualizar seu **[!UICONTROL Código de conexão]**, selecione o ícone de atualização (![ícone de atualização](/help/assets/icons/refresh.png)) ao lado do **[!UICONTROL Código de conexão]**.

![O código Connect com o ícone de atualização está realçado.](/help/assets/connect/establish-connection/refresh-connect-code.png){zoomable="yes"}

>[!IMPORTANT]
>
>Todas as contas criadas antes da introdução do recurso **[!UICONTROL Código de conexão]** não terão um código de conexão gerado, e o campo de conexão será exibido como **[!UICONTROL Indisponível]**. Use a opção de atualização para gerar um novo código de conexão.

#### Enviar convite de conexão privada {#send-private-connection-invite}

Depois de receber o **[!UICONTROL Código de conexão]** do seu colaborador, você poderá enviar um convite de conexão privada. Para fazer isso, navegue até o espaço de trabalho **[!UICONTROL Conectar]** e selecione o ícone de adição (![ícone de adição](/help/assets/icons/plus.png)) no canto superior direito.

![O ícone de adição destacado no espaço de trabalho do Connect.](/help/assets/connect/establish-connection/private-connection-invite.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Conectar]** é exibida, solicitando que você insira o **[!UICONTROL Código de conexão]** do colaborador com o qual deseja se conectar. Cole o código no campo de texto e selecione **[!UICONTROL Continuar]** para continuar.

![A caixa de diálogo Conectar com o campo Conectar código foi preenchida e a opção Continuar foi realçada.](/help/assets/connect/establish-connection/private-connection-invite-connect.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Conectar]** exibirá o colaborador ao qual o código está associado, permitindo que você confirme se está se conectando com o colaborador correto. Se o colaborador estiver correto, selecione **[!UICONTROL Conectar]** para enviar o convite de conexão privada.

![A caixa de diálogo Conectar com os detalhes do colaborador foi exibida e a opção Conectar foi realçada.](/help/assets/connect/establish-connection/private-connection-invite-connect-confirm.png){zoomable="yes"}

### Aceitar convite {#accept-invite}

>[!TIP]
>
>Ao discutir o processo de conexão, haverá uma distinção entre **proprietário** e **destinatário**. O proprietário é o colaborador que inicia a conexão enviando o convite, enquanto o destinatário é o colaborador que recebe e revisa o convite.

Antes que o proprietário possa definir as configurações de conexão, o destinatário deve aceitar o convite de conexão. Para fazer isso, navegue até o espaço de trabalho **[!UICONTROL Conectar]** e localize a conexão pendente na seção **[!UICONTROL Ação necessária]**. O status da conexão aparece como **[!UICONTROL Convite recebido]**. Selecione **[!UICONTROL Aceitar]** para aceitar o convite.

![A conexão pendente é exibida na seção Ação necessária do espaço de trabalho Conectar com a opção Aceitar realçada.](/help/assets/connect/establish-connection/accept-connection.png){zoomable="yes"}

A caixa de diálogo é exibida solicitando que você aceite o convite. Selecione **[!UICONTROL Aceitar convite]** para continuar.

![A caixa de diálogo Aceitar convite de conexão com a opção Aceitar convite está realçada.](/help/assets/connect/establish-connection/accept-connection-invite.png){zoomable="yes"}

O status da conexão é alterado para **[!UICONTROL Pendente]**. O proprietário agora pode definir as configurações de conexão.

### Definir configurações de conexão {#configure-connection-settings}

As configurações de conexão definem os termos entre dois colaboradores. Essas configurações incluem casos de uso, chaves de correspondência, divisão de crédito e contratos legais. Os colaboradores que se conectam com anunciantes também podem adicionar nomes de anunciantes às configurações de conexão, que serão usadas ao criar projetos.

Depois que o recipient aceitar o convite, o proprietário poderá definir as configurações de conexão. Para fazer isso, navegue até **[!UICONTROL Minhas conexões]** e localize a conexão pendente na seção **[!UICONTROL Ação necessária]**. Selecione **[!UICONTROL Configurar conexão]** para definir as configurações de conexão.

![O espaço de trabalho Conectar com a opção Configurar conexão foi realçado na seção Ação necessária.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

O espaço de trabalho de configurações de conexão é exibido, permitindo definir as várias configurações para a conexão.

![O espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/connection-set-up.png){zoomable="yes"}

<!-- FIX THE ABOVE SCREENSHOT TO INCLUDE ADV NAMES, AS WELL AS THE ONES BELOW -->

#### Configurações de conexão {#connection-settings}

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
>abstract="Esta seção determina quem está pagando pelas atividades correspondentes na Collaboration. "

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Compartilhamento de público-alvo"
>abstract="Os créditos de ativação de público-alvo são consumidos com base no número de IDs correspondentes preparadas para ativação."

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
>abstract="<p>Configuração opcional. Indica o nome e a ID pelos quais o editor conhece o anunciante.</p><p>O nome do anunciante adicionado aqui será preenchido previamente na etapa de criação do projeto.</p><ul><li>Se o editor tiver configurado vários nomes, selecione um deles na lista.</li><li>Se apenas um nome tiver sido configurado, ele será pré-selecionado automaticamente.</li><li>Se nenhum nome tiver sido configurado, o campo será preenchido previamente com o nome da conta do anunciante da Collaboration.</li></ul>"
>additional-url="https://experienceleague.adobe.com/pt-br/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="Criar um projeto"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_activation"
>title="Ativação de público-alvo"
>abstract="A Ativação de público-alvo permite selecionar qual colaborador pode iniciar a ativação de público-alvo."

Você pode definir as seguintes configurações de conexão:

+++Ativação de público-alvo

>[!IMPORTANT]
>
>Qualquer conexão criada antes do recurso **[!UICONTROL Ativação de público-alvo]** ser introduzido automaticamente terá a configuração de ativação de público definida como o proprietário da conexão. Se você quiser permitir que ambos os colaboradores ativem públicos, será necessário [excluir a conexão atual](#delete-connections) e criar uma nova com as configurações atualizadas.

A ativação de público permite selecionar qual colaborador pode ativar públicos-alvo na conexão. A ativação de público só será uma opção se o caso de uso **[!UICONTROL Ativação de público-alvo]** for selecionado. Se você optar por remover o caso de uso durante o processo de conexão, a configuração de ativação do público-alvo será removida das configurações de conexão. Para saber mais sobre a ativação de público, consulte o guia [ativar](/help/guide/collaborate/activate.md).

Para configurar a ativação de público-alvo, selecione **[!UICONTROL Configurar]** na seção **[!UICONTROL Ativação de público-alvo]**. Use o menu suspenso para especificar qual colaborador pode ativar públicos-alvo. Você pode escolher um único colaborador ou permitir que ambos os colaboradores ativem públicos.

![A caixa de diálogo de ativação de público-alvo com opções no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/audience-activation.png){zoomable="yes"}

Quando terminar, selecione **[!UICONTROL Salvar]** para salvar suas alterações.

![A caixa de diálogo de ativação de público-alvo com a opção Salvar no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/audience-activation-confirm.png){zoomable="yes"}

+++

+++Casos de uso

Os casos de uso são preenchidos automaticamente com todas as opções disponíveis. Os casos de uso selecionados determinam quais exibições e opções estão disponíveis em seus projetos. Para saber mais, leia o guia [casos de uso do projeto](/help/guide/collaborate/manage-projects.md#project-use-cases).

Para personalizar seus casos de uso, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Casos de uso]** e desative aqueles que você não deseja incluir em nenhum projeto com seu colaborador. Quando terminar, selecione **[!UICONTROL Salvar]** para salvar suas alterações.

![As configurações de casos de uso no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++Teclas de correspondência

As chaves de correspondência são preenchidas automaticamente com as que você selecionou ao [configurar sua conta](/help/guide/setup/onboard-account.md#set-up-match-keys). Você pode desativar as chaves de correspondência que não deseja usar, mas não pode adicionar chaves de correspondência que não foram selecionadas durante a configuração da conta.

Para personalizar suas chaves de correspondência, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Chaves de correspondência]** e desative todas as chaves de correspondência que não desejar usar nesta conexão. Quando terminar, selecione **[!UICONTROL Salvar]** para salvar suas alterações.

![As configurações da chave Corresponder no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++Divisão de crédito

Use a seção divisão de crédito para determinar qual das duas partes colaboradoras cobrirá os custos das atividades. As opções de divisão de crédito são determinadas pelos casos de uso selecionados para a conexão. Embora o caso de uso **[!UICONTROL Medição]** exija que uma parte cubra os custos, o caso de uso **[!UICONTROL Ativação - Correspondência]** oferece uma opção adicional para que cada parte cubra seus próprios custos. Para obter informações sobre o detalhamento de custos, leia o guia [tipos de atividade de crédito](/help/guide/setup/my-activity.md#types-of-activities).

>[!NOTE]
>
>Público-alvo - A saída é sempre coberta pelo colaborador que recebe o público-alvo, portanto, nenhuma seleção é necessária.

Para configurar a divisão de crédito, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Divisão de crédito]**. Em seguida, você pode selecionar as opções apropriadas para cada caso de uso. Quando terminar, selecione **[!UICONTROL Salvar]** para salvar suas alterações.

![A caixa de diálogo Divisão de crédito com opções no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}

+++

+++Contratos

Você deve reconhecer que um contrato legal está em vigor entre você e seu colaborador. Este contrato descreve os termos de compartilhamento e colaboração de dados. Você pode marcar a caixa de seleção **[!UICONTROL Confirmar e confirmar]** para confirmar se esse contrato existe.

![A seção Contrato legal é destacada e confirmada no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

+++Nomes do anunciante

>[!NOTE]
>
>Essa opção pode aparecer durante a configuração das configurações de conexão ou a revisão das configurações de conexão, dependendo de quem inicia a conexão.

Se você for um editor que está fazendo uma conexão com um anunciante, poderá optar por adicionar nomes de anunciante nas configurações de conexão. Isso permite adicionar vários nomes pelos quais o anunciante é conhecido em seus sistemas. Isso é particularmente útil se o anunciante tiver presença em várias regiões geográficas ou se forem conhecidos por nomes diferentes em contextos diferentes. Posteriormente, ao criar um projeto, você pode selecionar o nome do anunciante apropriado na lista de nomes configurados nas configurações de conexão.

![Os nomes de anunciante no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/advertiser-names.png){zoomable="yes"}

Para adicionar nomes de anunciante, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Nomes de anunciante]**. Você pode inserir a **[!UICONTROL ID do anunciante]** que o anunciante é conhecido por você como em seu sistema e um **[!UICONTROL Nome do anunciante]** para associar a essa ID no Collaboration. Você pode adicionar vários nomes de anunciante selecionando a opção **[!UICONTROL Adicionar]**.

![A caixa de diálogo Nomes de anunciante com opções no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/advertiser-names-dialog.png){zoomable="yes"}

Quando terminar, selecione **[!UICONTROL Salvar]** para salvar suas alterações.

Ao criar um projeto, o nome do anunciante será pré-preenchido com base nas seguintes configurações estabelecidas durante a conexão    :

1. **Nenhum nome de anunciante definido**: se nenhum nome de anunciante for adicionado, o padrão da Collaboration será usar o nome do anunciante como o nome do anunciante.
1. **Um conjunto de nomes de anunciante**: se um único nome de anunciante for adicionado, o Collaboration usará automaticamente esse nome como o nome de anunciante do projeto.
1. **Conjunto de vários nomes de anunciante**: se mais de um nome de anunciante for adicionado, você ou seu colaborador poderá selecionar qualquer um dos nomes fornecidos ao criar o projeto.

>[!NOTE]
>
> Depois de enviar as configurações de conexão, você não poderá mais adicionar ou editar nomes de anunciante.

![O espaço de trabalho de configurações de conexão com a seção de nomes de anunciante foi preenchida.](/help/assets/connect/establish-connection/add-advertiser-names.png)

+++

Depois de fazer suas seleções, selecione **[!UICONTROL Enviar]** para enviar as configurações sugeridas ao destinatário para revisão.

### Revisar configurações da conexão {#review-connection-settings}

Em seguida, o recipient precisa revisar as configurações de conexão propostas pelo proprietário. O destinatário pode fazer isso navegando até a guia **[!UICONTROL Minhas conexões]** no espaço de trabalho **[!UICONTROL Conectar]**. A conexão será exibida na seção **[!UICONTROL Ação necessária]**. Selecione **[!UICONTROL Revisar configurações de conexão]** para revisar as configurações de conexão propostas.

![O espaço de trabalho Minhas conexões com a opção Revisar configurações de conexão foi realçado.](/help/assets/connect/establish-connection/review-connection-settings.png){zoomable="yes"}

Revise as configurações propostas pelo colaborador. Você pode aceitar ou rejeitar as configurações de conexão. Se você rejeitar as configurações de conexão, precisará se comunicar com o colaborador sobre as alterações que você deseja fazer fora do produto. As informações de contato do colaborador são exibidas na seção **[!UICONTROL Contato]** do espaço de trabalho de configurações de conexão. O proprietário pode então revisar as configurações de conexão e reenviá-las para revisão.

Se você estiver satisfeito com as configurações de conexão propostas, deverá reconhecer que um contrato legal está em vigor entre você e o colaborador. Marque a caixa de seleção **[!UICONTROL Confirmar e confirmar]** para confirmar se esse contrato existe.

![A seção Contrato Legal foi realçada no espaço de trabalho de configurações de conexão.](/help/assets/connect/establish-connection/legal-agreement-review.png){zoomable="yes"}

Além disso, se você for um publicador conectado a um anunciante, poderá adicionar nomes de anunciante nas configurações de conexão. Para saber mais sobre este processo, consulte a seção [configurações de conexão](#connection-settings).

>[!NOTE]
>
> Depois de aceitar as configurações de conexão, você não poderá mais adicionar ou editar nomes de anunciante.

Em seguida, selecione **[!UICONTROL Aceitar]** para continuar com a conexão. O status da conexão será alterado para **[!UICONTROL Ativo]**, e agora você pode começar a colaborar em projetos.

## Excluir conexões {#delete-connections}

Você pode excluir qualquer conexão com colaboradores com os quais não deseja continuar trabalhando. Para excluir conexões existentes, navegue até **[!UICONTROL Conectar]**. Como editor, sua conexão existente será exibida. Como anunciante, você deve navegar até **[!UICONTROL Minhas conexões]**.

Selecione **[!UICONTROL Exibir conexão]** no cartão de conexão que deseja excluir.

![A opção de conexão Exibir foi realçada na exibição Minhas conexões.](/help/assets/connect/establish-connection/delete-view-connection.png){zoomable="yes"}

Selecione o ícone de exclusão ![ícone de exclusão](/help/assets/common/delete.svg) no espaço de trabalho de conexão para excluir a conexão.

![O ícone de exclusão foi realçado no espaço de trabalho de conexão.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

Uma caixa de diálogo de confirmação é exibida, solicitando que você confirme a exclusão da conexão. Selecione **[!UICONTROL Excluir]** para confirmar a exclusão.

![A caixa de diálogo de confirmação para excluir uma conexão.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Depois que a conexão for excluída, todos os projetos existentes na colaboração serão permanentemente excluídos e irrecuperáveis. A solicitação de conexão permanecerá em um estado pendente, mas a conexão e suas configurações não estarão mais ativas. Você precisará restabelecer a conexão se quiser se conectar com o colaborador novamente.

## Próximas etapas

Depois de estabelecer uma conexão com seu colaborador, você e ele agora podem [criar projetos](/help/guide/collaborate/manage-projects.md#create-project).
