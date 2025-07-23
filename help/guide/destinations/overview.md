---
title: Visão geral de destinos
description: Saiba mais sobre destinos no Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 6%

---

# Visão geral dos destinos

{{limited-availability-release-note}}

Destinos são integrações usadas para enviar públicos-alvo direcionados para plataformas externas. Essas integrações permitem ativar públicos em vários canais e plataformas de marketing para uso em campanhas e no engajamento do cliente.

Atualmente, os destinos só estão disponíveis para editores no Adobe Real-Time CDP Collaboration. Os editores podem configurar destinos para enviar públicos para plataformas externas, como o Adobe Experience Platform, para uso em campanhas. Os anunciantes podem [ativar públicos-alvo em um projeto](../collaborate/activate.md), que são enviados para o destino configurado do editor.

>[!IMPORTANT]
>
>Atualmente, quando os anunciantes ativam os públicos-alvo em seu projeto, eles são automaticamente enviados para o destino configurado de um editor. Como publicador, você **deve** configurar um destino *antes* que seu colaborador ative um público. Se nenhum destino estiver configurado, o público-alvo será enviado para você e ficará visível na guia **[!UICONTROL Ativar]** em um projeto, mas não será ativado.

## Configurar destinos {#configure-destinations}

Para configurar um destino, navegue até **[!UICONTROL Configuração]** e selecione a guia **[!UICONTROL Meus destinos]**. Aqui, você pode visualizar todos os destinos disponíveis.

>[!NOTE]
>
> Atualmente, somente o Adobe Experience Platform está disponível como destino de autoatendimento no Collaboration. Se você estiver interessado em configurar um destino como o Amazon S3 ou o Snowflake, entre em contato com o representante da Adobe.

![A guia Meus destinos no espaço de trabalho da Instalação mostrando os destinos disponíveis.](/help/assets/destinations/overview/my-destinations-overview.png)

Para começar a configurar um destino, selecione a opção **[!UICONTROL Configurar]** no destino de sua escolha. Para obter informações sobre como configurar destinos específicos, consulte os guias na tabela [destinos disponíveis](#available-destinations).

![O espaço de trabalho Meus destinos com a opção Configurar realçada para o destino do Adobe Experience Platform.](/help/assets/destinations/overview/my-destinations-set-up.png)

### Destinos disponíveis {#available-destinations}

Os seguintes destinos estão disponíveis para configuração no Collaboration. Para exibir o guia de configuração desse destino, selecione o nome do destino na tabela abaixo. Se você estiver interessado em configurar um destino que não esteja disponível no momento, entre em contato com o representante da Adobe.

| Destino | Disponibilidade |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | Disponível |
| Amazon S3 | Em breve. |
| Snowflake | Em breve. |
| Google Cloud Storage | Em breve. |
| Armazenamento Azure Blob | Em breve. |

## Próximas etapas

Depois de configurar o destino, você pode começar a [ativar públicos-alvo direcionados](../collaborate/activate.md) nos seus projetos.
