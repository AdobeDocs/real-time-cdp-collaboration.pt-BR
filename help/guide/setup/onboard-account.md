---
title: Configurar e gerenciar sua conta
description: Saiba como configurar e gerenciar vários aspectos da sua conta no Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '1363'
ht-degree: 14%

---

# Configurar e gerenciar sua conta

{{limited-availability-release-note}}

Saiba como configurar sua conta no Real-Time CDP Collaboration para se preparar para conexões com outros colaboradores. Este guia aborda a configuração inicial da conta, incluindo a adição de detalhes da conta, a seleção de chaves de correspondência e o gerenciamento das configurações da conta.

![O espaço de trabalho de instalação mostra uma conta configurada.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## Configurar sua conta {#set-up-account}

Ao acessar o Collaboration pela primeira vez, você será solicitado a configurar sua conta. Esse é um processo único que permite configurar os detalhes da sua conta e as chaves de correspondência. Se esta for a primeira conta da sua organização, você será direcionado para o processo de integração imediatamente, começando com a configuração dos [detalhes da sua conta](#set-up-details).

Para adicionar outras organizações, navegue até **[!UICONTROL Configuração]** no painel esquerdo e selecione o ícone adicionar (![ícone Adicionar.](/help/assets/icons/plus.png)) no canto superior direito. Em seguida, selecione **[!UICONTROL Conta]**.

![O espaço de trabalho de instalação com a guia Minha conta e a opção Conta realçada.](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### Configurar detalhes {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="Email de contato"
>abstract="Forneça um email de equipe ou baseado em funções, como **collaboration@yourcompany.com**. Endereços de email pessoais ou individuais não devem ser usados."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Código de conexão"
>abstract="O código de conexão é um identificador exclusivo para a conta. Ele é usado para estabelecer conexões com outros colaboradores na Real-Time CDP Collaboration."

Para começar a configurar sua conta, primeiro você deve definir os detalhes da conta. Isso requer que você adicione as seguintes informações:

* Adicione um **[!UICONTROL Nome da conta]** que represente claramente sua marca.
* Adicione uma **[!UICONTROL Descrição]** sobre sua marca. Isso é opcional, mas ajuda outros colaboradores a entender melhor sua marca.
* Selecione sua **[!UICONTROL Função]**. Você pode selecionar entre **[!UICONTROL Anunciante]** e **[!UICONTROL Publicador]**. Leia o guia [funções](/help/guide/overview/roles.md) para ver semelhanças e pequenas diferenças no fluxo de trabalho entre os dois tipos de função de conta.
* Selecione o **[!UICONTROL Setor]** da sua conta. Alguns exemplos incluem **[!UICONTROL Varejo]**, **[!UICONTROL Telecomunicações]** ou **[!UICONTROL Serviços financeiros]**.
* A **[!UICONTROL Região]** é automaticamente definida com base em sua conta da Adobe Experience Cloud. Isso não pode ser alterado a qualquer momento.
* Adicione um **[!UICONTROL Email de contato]** para sua conta. Esse deve ser um endereço de email de equipe ou baseado em funções. Endereços de email pessoais não devem ser fornecidos.
* Carregue um **[!UICONTROL Logotipo]** para sua conta. Atualmente, imagens do tipo SVG são compatíveis. Isso é opcional, mas carregar um logotipo ajuda a representar visualmente sua marca na interface do Collaboration
* Selecione uma imagem para a imagem do cabeçalho da conta.

>[!NOTE]
>
>Embora você possa editar a maioria desses detalhes a qualquer momento, a **[!UICONTROL Função]** não é editável após a configuração inicial. Quando terminar, use **[!UICONTROL Avançar]** para prosseguir para a próxima página e selecionar as chaves de correspondência desejadas que sua organização usará.

![O espaço de trabalho Configurar conta com a seção Detalhes exibida e a opção Avançar realçada.](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### Configurar chaves de correspondência {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Chaves de correspondência"
>abstract="As chaves de correspondência são identificadores usados para reconciliar perfis de público-alvo de diferentes fontes de dados. Inclua todas as chaves de correspondência com as quais sua marca pode trabalhar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_setup_match_keys"
>title="chaves de correspondência"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="IDs próprias para pessoas"
>abstract="As IDs de pessoas primárias, como endereços de email e números de telefone com hash ou IDs do CRM são conectadas diretamente a um perfil individual."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="IDs próprias para dispositivos"
>abstract="As IDs de dispositivos próprios, como ECID ou endereços IP, estão diretamente conectadas a dispositivos, que podem ser compartilhados entre várias pessoas. O IPv4 é a única ID própria para dispositivo compatível no momento."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="IDs de parceiros compatíveis"
>abstract="As IDs de parceiros são identificadores fornecidos por parceiros externos para reconciliação de público-alvo. As IDs de parceiros não estão conectadas diretamente a um perfil individual."

![Chaves de correspondência com suporte.](/help/assets/setup/manage-account/match-keys.png){zoomable="yes"}

>[!IMPORTANT]
>
>As chaves de correspondência selecionadas durante a configuração da conta determinarão as chaves de correspondência disponíveis em suas conexões. Embora você possa [remover chaves de correspondência indesejadas](../connect/establishing-connections.md#connection-settings) durante a configuração da conexão, chaves de correspondência não podem ser adicionadas após uma conexão ser estabelecida. É importante que você selecione **todas** as chaves de correspondência que planeja usar em campanhas futuras durante a configuração da conta.

As chaves de correspondência ajudam os colaboradores a trabalhar em conjunto, permitindo uma sincronização de dados precisa e centrada em privacidade, permitindo um direcionamento e uma medição de público mais precisos. As chaves de correspondência selecionadas durante a configuração da conta determinarão quais chaves de correspondência estarão disponíveis em conexões futuras. Eles também são usados para [mapear campos](./onboard-audiences.md#map-fields) da sua conexão de dados para os campos de destino no Collaboration ao fornecer públicos-alvo.

Selecione as teclas de correspondência que deseja usar ao reconciliar perfis de público-alvo. Planeje para o futuro e inclua todas as chaves de correspondência que você possa trabalhar e usar em campanhas futuras. Se você precisar selecionar chaves de correspondência adicionais para sua conta posteriormente, poderá fazê-lo no fluxo de trabalho [editar conta](#edit-account). No entanto, as teclas de correspondência adicionadas após a configuração inicial não estarão disponíveis para uso em conexões existentes.

#### Chaves de correspondência compatíveis {#supported-match-keys}

O Collaboration oferece suporte a três tipos de chaves de correspondência: IDs de pessoas primárias, IDs de dispositivos primários e IDs de parceiros. Todas as chaves de correspondência devem atender aos seguintes requisitos:

* As chaves correspondentes devem ser **cortadas**, **em minúsculas**
* As chaves de correspondência com hash devem ser **SHA256-hash**.
* Se você fornecer valores com hash que usam caracteres em maiúsculas, o Collaboration os converterá automaticamente em minúsculas.
* Se sua origem contiver **identificadores de texto sem formatação**, use a opção **[!UICONTROL Aplicar transformação]** durante a [configuração da conexão de dados](./manage-data-connection.md#match-keys) para aplicar o hash. Essa opção só está disponível ao fornecer públicos-alvo do Experience Platform e não tem suporte para fontes baseadas em nuvem.

##### IDs próprias para pessoas

As IDs de pessoas primárias estão conectadas diretamente a um perfil individual. As IDs compatíveis no momento são:

* **[!UICONTROL Email com hash]**
* **[!UICONTROL Telefone com hash]**
* **[!UICONTROL IDs do CRM]**
* **[!UICONTROL IDs de fidelidade]**
<!-- * **[!UICONTROL Custom ID]**: Custom identifiers -->

##### IDs próprias para dispositivos

As IDs de dispositivo próprio são identificadores conectados a um dispositivo específico. As IDs compatíveis no momento são:

* **[!UICONTROL IPv4]** com hash: endereços IPv4 com hash

##### IDs de parceiros

As IDs de parceiros são identificadores fornecidos por parceiros externos para reconciliação de público-alvo. As IDs compatíveis no momento são:

* **[!UICONTROL ID do Adfixus]**

>[!NOTE]
>
>A integração do Adobe com [!DNL Adfixus] mapeia as [!UICONTROL IDs do Adfixus] exclusivas de cada conta para um formato comum codificado em Adobe. Esses mapeamentos são usados para identificar sobreposições entre colaboradores. Ao ativar públicos-alvo usando a **[!UICONTROL ID do Adfixus]**, as IDs originais serão usadas. O formato codificado em Adobe nunca sai do Collaboration.

Ao selecionar **[!UICONTROL Adfixus ID]**, você precisará fornecer a ID correspondente do seu parceiro externo na seção **[!UICONTROL Credenciais da conta]**. Esta opção só estará disponível *após* alternando em **[!UICONTROL Adfixus ID]**. Insira a ID do Adfixus no campo **[!UICONTROL ID da Conta]**, certificando-se de verificar novamente a precisão do valor.

![A caixa de diálogo Corresponder chaves com Adfixus ID foi ativada e a seção Credenciais da conta foi realçada.](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

Depois de selecionar todas as chaves de correspondência desejadas, selecione **[!UICONTROL Concluir]** para concluir o fluxo de trabalho de configuração da conta.

![O espaço de trabalho Configurar conta com a seção Chaves de correspondência é exibido.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## Editar conta {#edit-account}

Após configurar sua conta, você pode editar os detalhes e as chaves de correspondência a qualquer momento.

### Editar detalhes {#edit-details}

Você pode editar a maioria dos detalhes da sua conta a qualquer momento, com exceção da **[!UICONTROL Função]**. A região é automaticamente definida com base em sua conta da Adobe Experience Cloud e não pode ser alterada.

Para editar sua conta, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Minha conta]** do espaço de trabalho **[!UICONTROL Instalação]**.

![O espaço de trabalho Instalação com a guia Minha conta e a opção Editar foi realçado.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

Agora você pode editar os detalhes da sua conta. Atualize todos os campos que deseja alterar e selecione **[!UICONTROL Salvar]** para confirmar as alterações.

![A caixa de diálogo Editar detalhes da conta.](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### Editar chaves de correspondência {#edit-match-keys}

>[!IMPORTANT]
>
>A edição de chaves de correspondência não afetará suas conexões existentes. Depois que uma conexão é estabelecida, as chaves de correspondência selecionadas durante a configuração da conexão são corrigidas. É importante que você selecione **todas** as chaves de correspondência que planeja usar em campanhas futuras durante a configuração da conta.

Você também pode atualizar as chaves de correspondência selecionadas inicialmente ao criar sua conta. Essas chaves de correspondência determinarão as chaves de correspondência disponíveis para conexões futuras.

Selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Chaves de correspondência]**.

![O espaço de trabalho de Instalação com a opção Editar realçada na seção Chaves de correspondência da conta.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Chaves de correspondência]** é exibida. Ative e desative qualquer chave de correspondência ou atualize sua **[!UICONTROL ID de Conta]** para sua [!UICONTROL ID de Adfixo] e selecione **[!UICONTROL Salvar]** para confirmar as alterações.

>[!IMPORTANT]
>
>Alterar sua [!UICONTROL ID do Adfixus] não acionará uma atualização de [rascunho de dados](../glossary.md#sketches) para suas conexões de dados existentes usando a chave de correspondência. Depois que os dados forem esboçados, as alterações na [!UICONTROL ID de Adfixo] não serão refletidas até a próxima atualização de público-alvo seguindo as configurações da [agenda de conexão de dados](./manage-data-connection.md#scheduling). Se você precisar de alterações antes da próxima atualização, poderá excluir e recriar sua conexão de dados.

![A caixa de diálogo Corresponder chaves com a opção Salvar foi realçada.](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

## Próximas etapas

Depois de configurar suas contas, você estará pronto para [originar públicos-alvo](/help/guide/setup/onboard-audiences.md) na Real-Time CDP Collaboration.
