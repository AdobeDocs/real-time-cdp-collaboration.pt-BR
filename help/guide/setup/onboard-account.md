---
title: Configurar e gerenciar sua conta
description: Saiba como configurar e gerenciar vários aspectos da sua conta no Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 13%

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
>abstract="O código de conexão é um identificador exclusivo da sua conta. É usado para estabelecer conexões com outros colaboradores no Real-Time CDP Collaboration."

<!-- Move the above popover to new section for invite on this page when its created -->

Para começar a configurar sua conta, primeiro você deve definir os detalhes da conta. Isso requer que você adicione as seguintes informações:

* Adicione um **[!UICONTROL Nome da conta]** que represente claramente sua marca.
* Adicione uma **[!UICONTROL Descrição]** sobre sua marca. Isso é opcional, mas ajuda outros colaboradores a entender melhor sua marca.
* Selecione sua **[!UICONTROL Função]**. Você pode selecionar entre **[!UICONTROL Anunciante]** e **[!UICONTROL Publicador]**. Leia o [documento de fluxo de trabalho completo](/help/guide/end-to-end-workflow.md) para ver semelhanças e pequenas diferenças no fluxo de trabalho entre os dois tipos de função organizacional.
<!-- The above will need to be updated when I update things for B2B -->
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
>abstract="As chaves de correspondência são identificadores usados para reconciliar membros entre públicos-alvo de diferentes fontes de dados. Inclua todas as chaves de correspondência com as quais sua marca pode trabalhar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="IDs próprias de pessoas"
>abstract="As IDs próprias de pessoas, como endereços de email ou números de telefone com hash, são conectadas diretamente a um perfil individual. As IDs compatíveis no momento são emails e números de telefone com hash."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="IDs de dispositivos próprios"
>abstract="As IDs de dispositivos próprios, como ECID ou endereços IP, estão diretamente conectadas a dispositivos, que podem ser compartilhados entre vários indivíduos. IPv4 é a única ID de dispositivos próprios compatível no momento."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="IDs de parceiros compatíveis"
>abstract="As IDs de parceiros associadas a perfis expandem o alcance para um determinado perfil."

>[!IMPORTANT]
>
>As chaves de correspondência selecionadas durante a configuração da conta determinarão as chaves de correspondência disponíveis para as conexões criadas com outros colaboradores. Embora você possa remover chaves de correspondência durante a configuração da conexão, não é possível adicionar novas chaves de correspondência. É importante selecionar **todas** as chaves de correspondência que você planeja usar em campanhas futuras durante a configuração da conta.

As chaves de correspondência, como endereços de email, IDs de dispositivo ou IDs de cliente, ajudam os colaboradores a trabalharem juntos, permitindo uma sincronização de dados precisa e centrada na privacidade, permitindo um direcionamento e uma medição de público mais precisos.

![Slide mostrando os identificadores disponíveis para a primeira versão do Collaboration.](/help/assets/setup/manage-account/available-identifiers.png)

<!-- Eventually replace this image above to match branding better. -->

Selecione as teclas de correspondência que deseja usar ao reconciliar perfis de público-alvo. Inclua todas as chaves de correspondência com as quais você pode trabalhar. Planeje para o futuro e selecione as chaves de correspondência que você prevê que usará em campanhas futuras. Se você precisar selecionar chaves de correspondência adicionais para sua conta posteriormente, poderá fazê-lo no fluxo de trabalho [editar conta](#edit-account).

Selecione até cinco chaves de correspondência que você planeja usar. Mais tarde, ao configurar conexões, você pode remover chaves de correspondência indesejadas, mas não pode adicionar novas.

Há três tipos de chaves de correspondência disponíveis:

* IDs próprias de pessoas
* IDs de dispositivos próprios
* IDs de parceiros

>[!IMPORTANT]
>
>Atualmente, a única chave compatível é o email com hash.

Quando estiver pronto, selecione **[!UICONTROL Concluir]** para concluir o fluxo de trabalho de configuração da organização.

![O espaço de trabalho Configurar organização com a seção Chaves de correspondência exibida.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## Editar conta {#edit-account}

Depois de configurar sua conta, você edita determinados aspectos e detalhes dela a qualquer momento. Para editar sua conta, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Minha conta]** do espaço de trabalho **[!UICONTROL Instalação]**.

![O espaço de trabalho Instalação com a guia Minha conta e a opção Editar foi realçado.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

Agora você pode editar os detalhes da sua conta, com exceção da **[!UICONTROL Função]**. Observe que a região é definida automaticamente com base em sua conta da Adobe Experience Cloud e não pode ser alterada a qualquer momento.

![A caixa de diálogo Editar detalhes da conta.](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

Você também pode atualizar as chaves de correspondência selecionadas inicialmente ao integrar sua organização. Selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Chaves de correspondência]** para adicionar as chaves de correspondência desejadas.

![O espaço de trabalho de Instalação com a opção Editar realçada na seção Chaves de correspondência da conta.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

## Próximas etapas

Depois de configurar suas contas, você estará pronto para [originar públicos-alvo](/help/guide/setup/onboard-audiences.md) na Real-Time CDP Collaboration.
