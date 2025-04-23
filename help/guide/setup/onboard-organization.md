---
title: Integração e gerenciamento da organização
description: Saiba como integrar e gerenciar vários aspectos da sua organização no Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: f146a39ab69a9a41bb12aeb59b0d23ae567cf4c2
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Integração e gerenciamento da organização

{{limited-availability-release-note}}

Saiba como integrar sua organização à Real-Time CDP Collaboration e gerenciar vários aspectos da empresa. Esta página descreve as etapas para integrar uma organização ao Adobe Real-Time CDP Collaboration, incluindo a configuração de chaves de correspondência, identidades preferenciais e mais opções.

![Página de instalação](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## Configuração inicial da organização

Primeiro, você deve configurar sua organização e os detalhes organizacionais. Navegue até **[!UICONTROL Configuração]** no painel esquerdo, selecione o símbolo **+** no canto superior direito e selecione **[!UICONTROL Conta]**.

>[!TIP]
>
>Depois de configurar uma conta inicial para trabalhar, é possível usar o mesmo fluxo de trabalho para configurar contas adicionais na mesma organização.

![Selecione a Conta para adicionar uma nova organização à Real-Time CDP Collaboration](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

O fluxo de trabalho para configurar sua organização inclui as duas páginas abaixo:

* [Configurar detalhes](#set-up-details)
* [Configurar chaves de correspondência](#set-up-match-keys)

>[!IMPORTANT]
>
>Quaisquer *chaves de correspondência* selecionadas no nível da organização serão percorridas até o [nível do projeto](/help/guide/collaborate/manage-projects.md) na colaboração entre anunciantes e editores. No nível do projeto, você pode remover qualquer chave de correspondência, mas *não* pode adicionar outras chaves que não foram selecionadas no nível da organização nesta tela.

### Configurar detalhes {#set-up-details}

![As etapas de detalhes e casos de uso para configurar uma organização](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. Adicione um **[!UICONTROL Nome da organização]** à sua empresa.
2. Adicione uma **[!UICONTROL Descrição]** sobre sua empresa.
3. Selecione sua **[!UICONTROL Função da empresa]**. Você pode selecionar entre **[!UICONTROL Anunciante]** e **[!UICONTROL Publicador]**. Leia o [documento de fluxo de trabalho completo](/help/guide/end-to-end-workflow.md) para ver semelhanças e pequenas diferenças no fluxo de trabalho entre os dois tipos de função organizacional.
4. Selecione o **[!UICONTROL Setor]** da sua organização. Alguns exemplos incluem **[!UICONTROL Varejo]**, **[!UICONTROL Telecomunicações]** ou **[!UICONTROL Serviços financeiros]**.
5. Selecione a **[!UICONTROL Região]** da sua organização. Na versão atual do produto, a **[!UICONTROL América do Norte]** é a seleção padrão predefinida.
6. <span class="preview"> Somente editor</span>: ao configurar uma organização publicadora, você deve ler e confirmar que será detectado pelos anunciantes no catálogo do publicador.
   ![Mensagem de aceitação específica do editor.](/help/assets/setup/manage-organization/publisher-specific-optin-message.png){zoomable="yes"}
7. Carregue um **[!UICONTROL Logotipo]** para sua empresa. Atualmente, imagens do tipo SVG são compatíveis.
8. Selecione uma imagem para a imagem do cabeçalho da empresa.

Quando estiver satisfeito com sua seleção, use **[!UICONTROL Avançar]** para prosseguir para a próxima página e selecione as chaves de correspondência desejadas que sua organização deve usar.

### Configurar chaves de correspondência {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Coincidir chaves"
>abstract="As chaves de correspondência são identificadores usados para reconciliar membros entre públicos-alvo de diferentes fontes de dados. Inclua todas as chaves de correspondência com as quais sua empresa pode trabalhar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="IDs de pessoas primárias"
>abstract="IDs de pessoas primárias, como endereços de email com hash ou números de telefone, são conectadas diretamente a um perfil individual. As IDs compatíveis no momento são emails com hash e números de telefone."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="IDs de dispositivo próprio"
>abstract="As IDs de dispositivo próprio, como ECID ou endereços IP, estão diretamente conectadas a dispositivos, que podem ser compartilhadas entre vários indivíduos. IPv4 é a única ID de dispositivo própria compatível no momento."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="IDs de parceiros compatíveis"
>abstract="As IDs de parceiros associadas a perfis expandem o alcance para um determinado perfil."

As chaves de correspondência, como endereços de email, IDs de dispositivo ou IDs de cliente, ajudam anunciantes e editores a trabalharem juntos, permitindo uma sincronização de dados precisa e compatível com a privacidade, o que permite um direcionamento e uma medição de público mais precisos.

![Slide mostrando os identificadores disponíveis para a primeira versão do Real-Time CDP Collaboration.](/help/assets/setup/manage-organization/available-identifiers.png)

Selecione as chaves de correspondência que deseja usar ao reconciliar membros de públicos-alvo de editores e anunciantes. Inclua todas as chaves de correspondência com as quais sua empresa pode trabalhar. Planeje para o futuro e selecione as chaves de correspondência que você antecipa que usará em campanhas futuras de editor-anunciante. Se você precisar selecionar chaves de correspondência adicionais para sua organização, também poderá fazer isso posteriormente, no fluxo de trabalho [editar organização](#edit-organization).

![Etapa de seleção de chaves de correspondência.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

Selecione até cinco chaves de correspondência que você planeja usar. Mais tarde, ao configurar conexões, você pode remover chaves de correspondência indesejadas, mas não pode adicionar novas.

As chaves de correspondência disponíveis no Real-Time CDP Collaboration podem ser de três tipos:

* IDs de pessoas primárias
* IDs de dispositivo próprio
* IDs de parceiros

As chaves de correspondência disponíveis para a primeira versão do Real-Time CDP Collaboration são:

* Email com hash

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

Quando estiver pronto, selecione **[!UICONTROL Concluir]** para concluir o fluxo de trabalho de configuração da organização.

## Editar organização {#edit-organization}

Depois de configurar inicialmente sua organização, você pode editar determinados aspectos e detalhes da organização a qualquer momento. Para editar sua organização, selecione **[!UICONTROL Editar]** na exibição **[!UICONTROL Minha organização]**.

![Controle de edição da organização destacado.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

Nesse ponto, é possível atualizar o nome, a descrição, o logotipo e a imagem do perfil da organização.

![Opções editáveis para organizações.](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

Você também pode atualizar as chaves de correspondência selecionadas inicialmente ao integrar sua organização, bem como o limite mínimo para identidades correspondentes a chaves de correspondência serem visíveis e utilizáveis em sobreposições de público-alvo e outras áreas de produtos. Selecione **[!UICONTROL Editar]** na guia **[!UICONTROL Chaves de correspondência]** para adicionar outras chaves de correspondência desejadas ou atualizar limites de identidade.

![Editar chaves de correspondência](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## Próximas etapas

Depois de configurar sua organização, você estará pronto para [importar públicos-alvo](/help/guide/setup/onboard-audiences.md) para a Real-Time CDP Collaboration.
