---
title: Configurar o Adobe Experience Platform como destino
description: Saiba como configurar e gerenciar o Adobe Experience Platform como destino no Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
TQID: https://experienceleague.adobe.com/vOAlNzIaEKC6cZC-zMxShPTn77kmV3WbUuvZU8Svzh4
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2: id: b5520579-b31f-4df7-9281-f0d9f91e2edcid: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: ff2b9b37-92e0-45fc-b853-379d44c08c89
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1534
ht-degree: 14%

---

# Configurar o Adobe Experience Platform como destino

{{limited-availability-release-note}}

Configure esse destino para ativar públicos do seu projeto para a Adobe Experience Platform. A ativação de públicos para o Adobe Experience Platform permite que você aproveite os recursos da plataforma para segmentação de público, análise e ativação em vários canais de marketing. Para saber mais sobre o Adobe Experience Platform, consulte a [visão geral do Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/landing/home){target="_blank"}.

>[!WARNING]
>
>Não é possível atualizar um destino após sua criação. Se precisar alterar alguma configuração, exclua o destino existente e crie um novo.

## Configurar destino {#configure-destination}

Para configurar o Adobe Experience Platform como destino, navegue até **[!UICONTROL Instalação]** e selecione a guia **[!UICONTROL Meus destinos]**. Selecione **[!UICONTROL Configurar]** para o Adobe Experience Platform.

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
>id="rtcdp_collaboration_destinations_activation_mapping"
>title="Saiba mais"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Namespaces de destino"
>abstract="Os namespaces de destino especificam para qual namespace de identidade a chave de correspondência será mapeada na Adobe Experience Platform. As chaves de correspondência com hash devem ser mapeadas para um namespace de destino que ofereça suporte a valores com hash."

Todas as chaves de correspondência ativadas para sua conta são incluídas no mapeamento de ativação por padrão. Se você não quiser mapear diretamente uma chave de correspondência para um namespace de destino, poderá usar a opção linked key para substituí-la por uma chave de correspondência diferente. Para obter mais informações sobre chaves vinculadas, consulte a [seção abaixo](#linked-keys).

#### Mapear namespaces de destino {#map-target-namespaces}

Para mapear cada chave correspondente a um namespace de destino, selecione o campo **[!UICONTROL Namespaces de destino]** ao lado da chave correspondente. A caixa de diálogo **[!UICONTROL Selecionar campo de origem]** é exibida. Localize o namespace alvo na lista ou procure um namespace específico. Selecione o namespace de destino que você deseja usar para a chave de correspondência e selecione **[!UICONTROL Selecionar]**.

>[!IMPORTANT]
>
>As chaves de correspondência com hash devem ser mapeadas para um namespace de destino que ofereça suporte a valores com hash. Por exemplo, a chave de correspondência **[!UICONTROL Email com hash]** deve ser mapeada para o namespace de identidade **[!UICONTROL Email(SHA256, em minúsculas)]** no Adobe Experience Platform. Você não pode mapear a chave de correspondência de **[!UICONTROL email com hash]** para o namespace de identidade **[!UICONTROL Email]**, pois esse namespace não oferece suporte a valores com hash.

![A caixa de diálogo Selecionar campo de origem com a opção Selecionar foi realçada..](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

Repita esse processo para cada chave de correspondência que você deseja incluir no mapeamento de ativação. Se você não quiser incluir uma chave de correspondência, remova-a ou use a opção linked key para substituí-la por uma chave de correspondência diferente.

#### Chaves vinculadas {#linked-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="Chave vinculada"
>abstract="As chaves vinculadas permitem especificar que uma chave de correspondência distinta deve ser usada no lugar da chave de correspondência original durante a ativação. Para que um perfil seja ativado, ele deve ter valores para a chave de correspondência original e para a chave de correspondência vinculada."

As chaves vinculadas permitem especificar que uma chave de correspondência distinta deve ser usada no lugar da chave de correspondência original durante a ativação. Para entender melhor como as teclas vinculadas funcionam, considere o seguinte exemplo:

Um retailer deseja enviar os dados que estão sendo ativados para o Experience Platform para o sistema CRM. O retailer ativou o IP com hash como uma chave de correspondência para que sua conta aumente a taxa de correspondência ao ativar públicos-alvo. No entanto, o sistema CRM da retailer não oferece suporte a IP com hash como um namespace de identidade. Portanto, é desejável usar a chave de correspondência da ID do CRM ao ativar públicos-alvo para o Experience Platform. A retailer pode usar a opção de chave vinculada para ativar públicos-alvo para o Experience Platform usando a ID do CRM em vez de IP com hash.

>[!NOTE]
>
>Para que um perfil seja ativado, ele deve ter valores para a chave de correspondência original e para a chave de correspondência vinculada. Por exemplo, se a ID com hash estiver vinculada à ID do CRM, um perfil deverá ter valores para a ID com hash e a ID do CRM serem ativadas. Se um dos valores estiver ausente, o perfil não será ativado.

Para usar uma chave vinculada, alterne na opção **[!UICONTROL Chave vinculada]** ao lado da chave de correspondência que você deseja usar em seu lugar. A seção **[!UICONTROL Chave vinculada]** é exibida solicitando a criação do mapeamento.

![A opção Chave vinculada e a seção destacadas no fluxo de trabalho Criar destino.](/help/assets/destinations/adobe-experience-platform/linked-key.png)

Selecione a **[!UICONTROL Chave vinculada]** que deseja usar no menu suspenso. Seguindo o exemplo acima, o retailer selecionaria **[!UICONTROL ID do CRM]** como a chave vinculada.

![A lista suspensa Chave vinculada foi realçada em Criar fluxo de trabalho de destino.](/help/assets/destinations/adobe-experience-platform/select-linked-key.png)

Em seguida, você deseja especificar o namespace alvo para a chave vinculada, se ainda não tiver feito isso. Se você já tiver selecionado o namespace de destino para a chave correspondente na seção **[!UICONTROL Criar mapeamento de ativação]**, ele será preenchido automaticamente. Se você ainda não tiver selecionado um namespace de destino para a chave vinculada, poderá fazê-lo agora.

Selecione o campo **[!UICONTROL Namespaces de destino]** ao lado da chave vinculada. A caixa de diálogo **[!UICONTROL Selecionar campo de origem]** é exibida. Localize o namespace alvo na lista ou procure um namespace específico. Selecione o namespace de destino que deseja usar para a chave vinculada e selecione **[!UICONTROL Selecionar]**.

![A caixa de diálogo Selecionar campo de origem.](/help/assets/destinations/adobe-experience-platform/select-linked-key-target-namespace.png)

A chave vinculada agora está configurada.

>[!NOTE]
>
>Você só pode usar um namespace alvo de chave vinculado por mapeamento de ativação. Por exemplo, se você vincular a ID com hash à ID do CRM, alternar a opção de chave vinculada para outro campo também a vinculará à ID do CRM.

Quando terminar de mapear todas as chaves de correspondência, revise suas configurações. A seção **[!UICONTROL Visualizar]** fornece um resumo da sua configuração.

![A seção Visualizar no fluxo de trabalho Criar destino.](/help/assets/destinations/adobe-experience-platform/preview.png)

>[!IMPORTANT]
>
>Atualmente, cada chave de correspondência é ativada para o Experience Platform como um público-alvo separado. Por exemplo, se você tiver [!UICONTROL email com hash] e [!UICONTROL telefone com hash] como chaves de correspondência, dois públicos separados serão criados no Portal de público-alvo quando um público-alvo for ativado.

Quando estiver satisfeito com sua configuração, selecione **[!UICONTROL Criar destino]**. Uma mensagem de confirmação é exibida, indicando que o destino foi criado com sucesso.

## Using Adobe Experience Platform as a destination

Once you&#39;ve configured Experience Platform as a destination, you can begin [activating audiences](../collaborate/activate.md) to the platform through your projects. Currently, the activation process is a single-step process initiated by the collaborator. For example, when an advertiser activates an audience, it is sent to the publisher’s pre-configured destination (Experience Platform). The publisher does not need to take any additional steps to send the audience to the destination. The same holds true for the brand-to-brand collaboration pattern.

>[!IMPORTANT]
>
>You **must** configure Experience Platform as a destination *before* your collaborator activates an audience. If the destination is not configured, the audience will be sent to you and visible in the **[!UICONTROL Activate]** tab within a project, but will not be activated to Experience Platform.

After the audience is activated, it will be available in [Audience Portal](#audience-portal) in Experience Platform with Real-Time CDP Collaboration as the origin.  These audiences can then be used in campaigns and customer engagement.

### Portal de público-alvo {#audience-portal}

Now that you have configured Adobe Experience Platform as a destination, you can view the activated audiences in the Audience Portal. Audience Portal is a central hub within Adobe Experience Platform that allows you to view and manage your audiences. Audience portal now provides Real-Time CDP Collaboration as an origin when filtering your audiences.

>[!IMPORTANT]
>
>You are responsible for applying any necessary data usage labels to the audiences you activate to Adobe Experience Platform. For more information, refer to the [data usage labels](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/overview){target="_blank"} guide.

![The Audience Portal with Real-Time CDP Collaboration as an origin in the filter options.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

To learn more about Audience Portal, refer to the [Audience Portal overview](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"} guide.
