---
title: Integração e gerenciamento da organização
description: Saiba como integrar e gerenciar vários aspectos da sua organização no Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 860138b95abc4d6af94bbbf722cf498463570c1b
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 19%

---

# Integrar e gerenciar sua organização

{{limited-availability-release-note}}

Saiba como integrar sua organização à Real-Time CDP Collaboration e gerenciar vários aspectos da empresa. Esta página descreve as etapas para integrar uma organização ao Adobe Real-Time CDP Collaboration, incluindo a configuração de chaves de correspondência, identidades preferenciais e mais opções.

![O espaço de trabalho de configuração da organização apresentando suas configurações atuais.](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## Configuração inicial da organização

Primeiro, você deve configurar sua organização e os detalhes organizacionais. Se esta for sua primeira organização, você será direcionado imediatamente para o processo de integração, começando com a configuração dos [detalhes da sua conta](#set-up-details).

Para adicionar outras organizações, navegue até **[!UICONTROL Configuração]** no painel esquerdo e selecione o ícone adicionar (![ícone Adicionar.](/help/assets/icons/plus.png)) no canto superior direito. Em seguida, selecione **[!UICONTROL Conta]**.

![O espaço de trabalho de instalação com a opção Conta realçada.](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

### Configurar detalhes {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="Email de contato"
>abstract="Forneça um email de equipe ou baseado em funções, como `collaboration@yourcompany.com`. Endereços de email pessoais ou individuais não devem ser usados."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Código de conexão"
>abstract="O código de conexão é um identificador exclusivo para a sua organização. Ele é usado para estabelecer conexões com outras organizações na Real-Time CDP Collaboration."

<!-- Move the above to new section for invite on this page when its created -->

Para começar a integrar sua organização, primeiro você deve configurar os detalhes da organização. Isso requer que você adicione as seguintes informações:

* Adicione um **[!UICONTROL Nome da organização]** à sua empresa.
* Adicione uma **[!UICONTROL Descrição]** sobre sua empresa.
* Selecione sua **[!UICONTROL Função da empresa]**. Você pode selecionar entre **[!UICONTROL Anunciante]** e **[!UICONTROL Publicador]**. Leia o [documento de fluxo de trabalho completo](/help/guide/end-to-end-workflow.md) para ver semelhanças e pequenas diferenças no fluxo de trabalho entre os dois tipos de função organizacional.
* Selecione o **[!UICONTROL Setor]** da sua organização. Alguns exemplos incluem **[!UICONTROL Varejo]**, **[!UICONTROL Telecomunicações]** ou **[!UICONTROL Serviços financeiros]**.
* Selecione a **[!UICONTROL Região]** da sua organização. Na versão atual do produto, a **[!UICONTROL América do Norte]** é a seleção padrão predefinida.
* Adicione um **[!UICONTROL Email de contato]** para sua organização. Esse deve ser um endereço de email de equipe ou baseado em funções. Endereços de email pessoais não devem ser fornecidos.
* Carregue um **[!UICONTROL Logotipo]** para sua empresa. Atualmente, imagens do tipo SVG são compatíveis.
* Selecione uma imagem para a imagem do cabeçalho da empresa.

>[!NOTE]
>
>Embora você possa editar a maioria desses detalhes a qualquer momento, a **[!UICONTROL Função]** e a **[!UICONTROL Região]** não serão editáveis após a configuração inicial.

![O espaço de trabalho Configurar organização com a seção Detalhes exibida.](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

Quando terminar, use **[!UICONTROL Avançar]** para prosseguir para a próxima página e selecionar as chaves de correspondência desejadas que sua organização usará.

### Configurar chaves de correspondência {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Chaves de correspondência"
>abstract="As chaves de correspondência são identificadores usados para reconciliar membros entre públicos-alvo de diferentes fontes de dados. Inclua todas as chaves de correspondência com as quais sua empresa pode trabalhar."

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
>As chaves de correspondência selecionadas durante a configuração da organização determinarão as chaves de correspondência disponíveis para as conexões criadas com outras organizações. Embora você possa remover chaves de correspondência durante a configuração da conexão, não é possível adicionar novas chaves de correspondência posteriormente. É importante selecionar todas as chaves de correspondência que você planeja usar em campanhas futuras durante a configuração da organização.

As chaves de correspondência, como endereços de email, IDs de dispositivo ou IDs de cliente, ajudam anunciantes e editores a trabalharem juntos, permitindo uma sincronização de dados precisa e centrada em privacidade, permitindo um direcionamento e uma medição de público mais precisos.

![Slide mostrando os identificadores disponíveis para a primeira versão do Real-Time CDP Collaboration.](/help/assets/setup/manage-organization/available-identifiers.png)

Selecione as chaves de correspondência que deseja usar ao reconciliar membros de públicos-alvo de editores e anunciantes. Inclua todas as chaves de correspondência com as quais sua empresa pode trabalhar. Planeje para o futuro e selecione as chaves de correspondência que você antecipa que usará em campanhas futuras de editor-anunciante. Se você precisar selecionar chaves de correspondência adicionais para sua organização, também poderá fazer isso posteriormente, no fluxo de trabalho [editar organização](#edit-organization).

![O espaço de trabalho Configurar organização com a seção Chaves de correspondência exibida.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

Selecione até cinco chaves de correspondência que você planeja usar. Mais tarde, ao configurar conexões, você pode remover chaves de correspondência indesejadas, mas não pode adicionar novas.

As chaves de correspondência disponíveis no Real-Time CDP Collaboration podem ser de três tipos:

* IDs próprias de pessoas
* IDs de dispositivos próprios
* IDs de parceiros

As chaves de correspondência disponíveis para a primeira versão do Real-Time CDP Collaboration são:

* Email com hash

Quando estiver pronto, selecione **[!UICONTROL Concluir]** para concluir o fluxo de trabalho de configuração da organização.

## Editar organização {#edit-organization}

Depois de configurar inicialmente sua organização, você pode editar determinados aspectos e detalhes da organização a qualquer momento. Para editar sua organização, selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Minha organização]** do espaço de trabalho **[!UICONTROL Instalação]**.

![O espaço de trabalho de Instalação com a guia Minha organização e a opção Editar foi realçado.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

Agora é possível editar os detalhes da organização, com exceção da **[!UICONTROL Função]** e da **[!UICONTROL Região]**.

![A caixa de diálogo Editar detalhes da organização.](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

Você também pode atualizar as chaves de correspondência selecionadas inicialmente ao integrar sua organização. Selecione **[!UICONTROL Editar]** na seção **[!UICONTROL Chaves de correspondência]** para adicionar as chaves de correspondência desejadas.

![O espaço de trabalho de Instalação com a opção Editar realçada na seção Chaves de correspondência da organização.](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## Próximas etapas

Depois de configurar sua organização, você estará pronto para [importar públicos-alvo](/help/guide/setup/onboard-audiences.md) para a Real-Time CDP Collaboration.
