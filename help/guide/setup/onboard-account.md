---
title: Configurar e gerenciar sua conta
description: Learn how to configure and manage various aspects of your account in Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
TQID: https://experienceleague.adobe.com/PRmSkRSE2tQ-5t5hHKzDAGrkF6-irmZid2Akq6-PQv8
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1393
ht-degree: 13%

---

# Configurar e gerenciar sua conta

{{limited-availability-release-note}}

Learn how to set up your account in Real-Time CDP Collaboration to prepare for connections with other collaborators. This guide covers the initial setup of your account, including adding account details, selecting match keys, and managing your account&#39;s settings.

![The setup workspace showing a configured account.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## Set up your account {#set-up-account}

When you first access Collaboration, you are prompted to set up your account. This is a one-time process that allows you to configure your account details and match keys. If this is your organization&#39;s first account, you&#39;ll be directed through the onboarding process immediately, starting with setting up your [account details](#set-up-details).

To add additional organizations, navigate to **[!UICONTROL Setup]** in the left rail and select the add icon (![Add icon.](/help/assets/icons/plus.png)) in the upper right corner. Next, select **[!UICONTROL Account]**.

![The setup workspace with the My account tab and Account option highlighted.](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### Configurar detalhes {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="Email de contato"
>abstract="Forneça um email de equipe ou baseado em funções, como **collaboration@yourcompany.com**. Endereços de email pessoais ou individuais não devem ser usados."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Código de conexão"
>abstract="O código de conexão é um identificador exclusivo para a conta. Ele é usado para estabelecer conexões com outros colaboradores na Real-Time CDP Collaboration."

To begin configuring your account, you must first set up the account details. This requires you to add the following information:

* Add an **[!UICONTROL Account name]** that clearly represents your brand.
* Add a **[!UICONTROL Description]** about your brand. This is optional, but it helps other collaborators understand your brand better.
* Select your **[!UICONTROL Role]**. You can select between **[!UICONTROL Advertiser]** and **[!UICONTROL Publisher]**. Read the [roles](/help/guide/overview/roles.md) guide to see similarities and slight differences in workflow between the two account role types.
* Select the **[!UICONTROL Industry]** for your account. Some examples include **[!UICONTROL Retail]**, **[!UICONTROL Telecommunications]**, or **[!UICONTROL Financial services]**.
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
>abstract="As IDs de dispositivos próprios, como ECID ou endereços IP, estão diretamente conectadas a dispositivos que podem ser compartilhados entre várias pessoas."

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
* **[!UICONTROL IDFA]**: o Identificador para Anunciantes (IDFA) usado em dispositivos Apple iOS
* **[!UICONTROL GAID]**: ID do Anunciante do Google usada em dispositivos Android

##### IDs de parceiros

As IDs de parceiros são identificadores fornecidos por parceiros externos para reconciliação de público-alvo. As IDs compatíveis no momento são:

* **[!UICONTROL AdFixus ID]**

>[!NOTE]
>
>A integração do Adobe com o [!DNL AdFixus] mapeia as [!UICONTROL IDs do AdFixus] exclusivas de cada conta para um formato comum codificado em Adobe. Esses mapeamentos são usados para identificar sobreposições entre colaboradores. Ao ativar públicos-alvo usando a **[!UICONTROL AdFixus ID]**, as IDs originais serão usadas. O formato codificado em Adobe nunca sai do Collaboration.

Ao selecionar **[!UICONTROL AdFixus ID]**, você precisará fornecer a ID correspondente do seu parceiro externo na seção **[!UICONTROL Credenciais da conta]**. Esta opção só estará disponível *após* alternando em **[!UICONTROL AdFixus ID]**. Digite sua ID do AdFixus no campo **[!UICONTROL ID da Conta]**, certificando-se de verificar novamente a precisão do valor.

![A caixa de diálogo Corresponder chaves com AdFixus ID foi ativada e a seção Credenciais da conta foi realçada.](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

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

Você também pode atualizar as chaves de correspondência selecionadas inicialmente ao criar sua conta. Essas chaves de correspondência determinarão as chaves de correspondência disponíveis para conexões futuras.

Selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Chaves de correspondência]**.

![O espaço de trabalho de Instalação com a opção Editar realçada na seção Chaves de correspondência da conta.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Chaves de correspondência]** é exibida. Ative qualquer chave de correspondência ou atualize sua **[!UICONTROL ID da Conta]** para sua [!UICONTROL AdFixus ID] e selecione **[!UICONTROL Salvar]** para confirmar as alterações.

>[!IMPORTANT]
>
>Alterar sua [!UICONTROL AdFixus ID] não acionará uma atualização de [rascunho de dados](../glossary.md#sketches) para suas conexões de dados existentes usando a chave de correspondência. Depois que os dados forem esboçados, as alterações na [!UICONTROL AdFixus ID] não serão refletidas até a próxima atualização do público-alvo seguindo as configurações da [agenda de conexão de dados](./manage-data-connection.md#scheduling). Se você precisar de alterações antes da próxima atualização, poderá excluir e recriar sua conexão de dados.
>
>No momento, as chaves de correspondência não podem ser removidas depois de adicionadas à sua conta.

![A caixa de diálogo Corresponder chaves com a opção Salvar foi realçada.](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

Uma caixa de diálogo de sucesso confirma que as chaves correspondentes da sua conta foram atualizadas com sucesso.

![Uma caixa de diálogo bem-sucedida confirmando que as chaves de correspondência da sua conta foram atualizadas com êxito.](/help/assets/setup/manage-account/match-key-updated-successfully.png){zoomable="yes"}

## Próximas etapas

After setting up your accounts, you are ready to [source audiences](/help/guide/setup/onboard-audiences.md) into Real-Time CDP Collaboration.
