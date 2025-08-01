---
title: Configurar e gerenciar destinos
description: Saiba como configurar e gerenciar destinos no Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b4b26761-46ac-420f-b9f7-6e829d67aec9
source-git-commit: a7215d453021be578a32ce1af4d659845c3b8493
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 1%

---

# Configurar e gerenciar destinos

{{limited-availability-release-note}}

Destinos são integrações usadas para enviar públicos-alvo direcionados para plataformas externas. Essas integrações permitem ativar públicos em vários canais e plataformas de marketing para uso em campanhas e no engajamento do cliente.

Os colaboradores podem configurar destinos para enviar públicos-alvo para plataformas externas, como o Adobe Experience Platform, para uso em campanhas. Os colaboradores podem [ativar públicos-alvo em um projeto](../collaborate/activate.md), que são enviados para o destino configurado de sua conexão. A ativação pode ser feita por qualquer um dos colaboradores, dependendo das configurações de ativação de público-alvo [definidas na conexão](/help/guide/connect/establishing-connections.md#configure-connection-settings).

![A guia Meus destinos no espaço de trabalho da Instalação mostrando um destino ativo do Adobe Experience Platform.](/help/assets/setup/manage-destinations/my-destinations-overview.png)

Para saber mais sobre destinos, consulte o guia [visão geral dos destinos](../destinations/overview.md).

## Configurar destinos {#configure-destinations}

Os destinos estão configurados na seção **[!UICONTROL Configuração]** do Collaboration. Para configurar um destino, navegue até **[!UICONTROL Configuração]** e selecione a guia **[!UICONTROL Meus destinos]**. Aqui, você pode visualizar todos os destinos disponíveis.

>[!IMPORTANT]
>
>Para configurar e gerenciar destinos, seu usuário deve ter uma função com a permissão **Gerenciar dados de público-alvo** atribuída a ele. Para obter mais informações sobre como gerenciar funções, consulte o guia [gerenciar funções](../permissions/manage-roles.md).

![A guia Meus destinos no espaço de trabalho da Instalação mostrando os destinos disponíveis.](/help/assets/setup/manage-destinations/my-destinations.png)

O processo de configuração para destinos depende do destino que você está configurando. Consulte o catálogo [destinos disponíveis](../destinations/overview.md#available-destinations) para exibir os destinos disponíveis e seus guias de configuração.

>[!NOTE]
>
>Atualmente, somente o Adobe Experience Platform está disponível como destino de autoatendimento no Real-Time CDP Collaboration. Se você estiver interessado em configurar um destino diferente, entre em contato com o representante da Adobe.

## Excluir destinos {#delete-destinations}

Excluir um destino o remove da sua conta, remove qualquer público enviado anteriormente do destino e impede que qualquer público futuro seja enviado para esse destino.

Para excluir um destino, navegue até a guia **[!UICONTROL Meus destinos]** na seção **[!UICONTROL Instalação]**. Selecione a opção **[!UICONTROL Excluir]** para o destino que você deseja remover.

![O espaço de trabalho Meus destinos com a opção Excluir realçada para o destino do Adobe Experience Platform.](/help/assets/setup/manage-destinations/delete-destination.png)

Uma caixa de diálogo de confirmação é exibida, onde você pode confirmar que deseja excluir o destino. Selecione **[!UICONTROL Excluir]** para remover o destino.

![A caixa de diálogo Excluir destino com a opção Excluir foi realçada.](/help/assets/setup/manage-destinations/delete-destination-confirmation.png)

## Próximas etapas

Depois de configurar o destino, você pode começar a colaborar em suas conexões para [ativar públicos-alvo direcionados](../collaborate/activate.md) em seus projetos.
