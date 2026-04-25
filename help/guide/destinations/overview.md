---
title: Visão geral de destinos
description: Saiba mais sobre destinos no Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
TQID: https://experienceleague.adobe.com/1VvnSt3Z65dfQBfXnjJJi3H0Oj9BxFStexq3icVKxkY
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2: id: b5520579-b31f-4df7-9281-f0d9f91e2edcid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 3%

---

# Visão geral dos destinos

{{limited-availability-release-note}}

Destinos são integrações usadas para enviar públicos-alvo direcionados para plataformas externas. Essas integrações permitem ativar públicos em vários canais e plataformas de marketing para uso em campanhas e no engajamento do cliente.

Os colaboradores podem configurar destinos para enviar públicos-alvo para plataformas externas, como o Adobe Experience Platform, para uso em campanhas. Os colaboradores podem [ativar públicos-alvo em um projeto](../collaborate/activate.md), que são enviados para o destino configurado de sua conexão. A ativação pode ser feita por qualquer um dos colaboradores, dependendo das configurações de ativação de público-alvo [definidas na conexão](/help/guide/connect/establishing-connections.md#configure-connection-settings).

>[!IMPORTANT]
>
>Atualmente, quando os colaboradores ativam os públicos-alvo em um projeto, eles são automaticamente enviados para o destino configurado da conexão. Você **deve** configurar um destino para que seu colaborador possa ativar públicos-alvo em um projeto.

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
| [!DNL Amazon S3] | Em breve. |
| [!DNL Snowflake] | Em breve. |
| [!DNL Google Cloud Storage] | Em breve. |
| [!DNL Azure Blob Storage] | Em breve. |

>[!NOTE]
>
>**[!DNL Google Cloud Storage]** nesta tabela refere-se a **destinos** (em que o Collaboration envia públicos-alvo durante a ativação). Para **originar públicos-alvo de** um bucket de GCS no espaço de trabalho **[!UICONTROL Configuração]**, consulte [Configurar GCS para fornecimento de público-alvo](../setup/configure-gcs-audience-sourcing.md).

## Próximas etapas

Depois de configurar o destino, você pode começar a [ativar públicos-alvo direcionados](../collaborate/activate.md) nos seus projetos.
