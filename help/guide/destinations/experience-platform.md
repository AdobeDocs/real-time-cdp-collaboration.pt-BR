---
title: Configurar o Adobe Experience Platform como destino
description: Saiba como configurar e gerenciar o Adobe Experience Platform como destino no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: 4ef7f8c7c27935f0e5b3620da63e7129f2714b37
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 11%

---

# Configurar o Adobe Experience Platform como destino

{{limited-availability-release-note}}

Configure esse destino para ativar públicos do seu projeto para a Adobe Experience Platform. A ativação de públicos para o Adobe Experience Platform permite que você aproveite os recursos da plataforma para segmentação de público, análise e ativação em vários canais de marketing. Para saber mais sobre o Adobe Experience Platform, consulte a [visão geral do Experience Platform](https://experienceleague.adobe.com/pt-br/docs/experience-platform/landing/home){target="_blank"}.

## Configurar destino {#configure-destination}

Para configurar o Adobe Experience Platform como destino, navegue até **[!UICONTROL Instalação]** e selecione a guia **[!UICONTROL Destinos]**. Selecione **[!UICONTROL Configurar]** para o Adobe Experience Platform.

![O espaço de trabalho Meus destinos com a opção Configurar foi realçado para o destino do Adobe Experience Platform.](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

O fluxo de trabalho **[!UICONTROL Criar destino]** é exibido.

![O fluxo de trabalho Criar destino para o Adobe Experience Platform.](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### Configurar sandbox {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="Expiração de público-alvo"
>abstract="O período após o qual o público-alvo não estará mais disponível na Adobe Experience Platform. A expiração padrão é de 30 dias, mas você pode defini-la como qualquer valor entre 1 e 30 dias."

Primeiro, selecione a sandbox para onde os dados do público-alvo serão enviados.

>[!IMPORTANT]
>
>Você só pode selecionar uma sandbox à qual o usuário tenha acesso. Por padrão, todos os usuários do Collaboration têm acesso à sandbox **Prod**. Para obter acesso a sandboxes adicionais, um administrador deve adicionar sandboxes adicionais a uma função atribuída ao usuário. Para obter mais informações sobre como gerenciar funções, consulte o guia [gerenciar funções](../permissions/manage-roles.md).

Na seção **[!UICONTROL Configurar sandbox]**, selecione a lista suspensa **[!UICONTROL Sandbox]** ou digite o nome de uma sandbox.

![A lista suspensa Sandbox foi realçada em Criar fluxo de trabalho de destino.](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

Como alternativa, você pode selecionar **[!UICONTROL Procurar sandbox]** para exibir todas as sandboxes disponíveis, bem como seu **[!UICONTROL Tipo]**, **[!UICONTROL Status]** e **[!UICONTROL Região]**. Selecione a sandbox que deseja usar e selecione **[!UICONTROL Salvar]**.

Em seguida, configure a **[!UICONTROL Expiração do público-alvo]**. Por padrão, a expiração do público-alvo é definida como 30 dias. Você pode optar por definir a expiração em qualquer lugar, de 1 a 30 dias. Após a data de expiração, o público-alvo não estará mais disponível no Adobe Experience Platform.

![A seção Expiração de Público-Alvo foi destacada no fluxo de trabalho Criar destino.](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### Criar mapeamento de ativação {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="Chaves de correspondência de ativação"
>abstract="As chaves de correspondência de ativação são exibidas com base nas chaves de correspondência selecionadas ao criar sua organização."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Namespaces de destino"
>abstract="Os namespaces de destino especificam para qual namespace de identidade a chave de correspondência será mapeada na Adobe Experience Platform. As chaves de correspondência com hash devem ser mapeadas para um namespace de destino que ofereça suporte a valores com hash."

Em seguida, crie um mapeamento de ativação para definir como os dados do público-alvo serão enviados para o Adobe Experience Platform. Você pode mapear cada [chave de correspondência](../setup/onboard-account.md#set-up-match-keys) selecionada ao criar sua organização em um namespace de destino. Os namespaces de destino especificam para qual [namespace de identidade](https://experienceleague.adobe.com/pt-br/docs/experience-platform/identity/features/namespaces#standard){target="_blank"} a chave correspondente será mapeada no Adobe Experience Platform.

>[!IMPORTANT]
>
>As chaves de correspondência com hash devem ser mapeadas para um namespace de destino que ofereça suporte a valores com hash. Por exemplo, a chave de correspondência **[!UICONTROL Email com hash]** deve ser mapeada para o namespace de identidade **[!UICONTROL Email(SHA256, em minúsculas)]** no Adobe Experience Platform. Você não pode mapear a chave de correspondência de **[!UICONTROL email com hash]** para o namespace de identidade **[!UICONTROL Email]**, pois esse namespace não oferece suporte a valores com hash.

Selecione o campo **[!UICONTROL Namespaces de destino]** ao lado de cada chave correspondente. A caixa de diálogo **[!UICONTROL Selecionar campo de origem]** é exibida. Localize o namespace alvo na lista ou procure um namespace específico. Selecione o namespace de destino que você deseja usar para a chave de correspondência e selecione **[!UICONTROL Selecionar]**.

![A caixa de diálogo Selecionar campo de origem com a opção Selecionar foi realçada..](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

Quando terminar de mapear todas as chaves de correspondência, revise suas configurações e selecione **[!UICONTROL Criar]** para concluir a criação do destino.

## Utilização do Adobe Experience Platform como destino

Depois de configurar o Adobe Experience Platform como destino, você pode começar a [ativar públicos-alvo](../collaborate/activate.md) para a plataforma por meio de seus projetos. Atualmente, o processo de ativação é um processo de etapa única iniciado pelo anunciante. Quando o anunciante ativa um público-alvo, ele é enviado para o destino pré-configurado do editor (nesse caso, o Adobe Experience Platform). O editor não precisa realizar nenhuma etapa adicional para enviar o público-alvo para o destino.

>[!IMPORTANT]
>
>Você **deve** configurar o Adobe Experience Platform como um destino *antes* que seu colaborador ative um público-alvo. Se o destino não estiver configurado, o público-alvo será enviado para você e ficará visível na guia **[!UICONTROL Ativar]** em um projeto, mas não será ativado para a Adobe Experience Platform.

Depois que o público-alvo for ativado, ele estará disponível no [Portal de público-alvo](#audience-portal) no Experience Platform com o Real-Time CDP Collaboration como origem.  Esses públicos-alvo podem ser usados em campanhas e no envolvimento do cliente.

### Portal de público-alvo {#audience-portal}

Agora que você configurou o Adobe Experience Platform como destino, é possível visualizar os públicos ativados no Portal de público-alvo. O Portal de público-alvo é um hub central no Adobe Experience Platform que permite visualizar e gerenciar os públicos-alvo. O portal de público-alvo agora fornece o Real-Time CDP Collaboration como origem ao filtrar os públicos-alvo.

>[!IMPORTANT]
>
>Você é responsável por aplicar os rótulos de uso de dados necessários aos públicos-alvo ativados no Adobe Experience Platform. Para obter mais informações, consulte o guia [rótulos de uso de dados](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/overview){target="_blank"}.

![O Portal de Público-Alvo com Real-Time CDP Collaboration como origem nas opções de filtro.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Para saber mais sobre o Audience Portal, consulte o guia [Visão geral do Audience Portal](https://experienceleague.adobe.com/pt-br/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"}.
