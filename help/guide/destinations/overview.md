---
title: Visão geral de destinos
description: Saiba mais sobre destinos no Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
TQID: https://experienceleague.adobe.com/1VvnSt3Z65dfQBfXnjJJi3H0Oj9BxFStexq3icVKxkY
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 7ab1bc21a4d644e2e6a481d8de594d6a509a92a5
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 6%

---

# Visão geral dos destinos

{{limited-availability-release-note}}

>[!NOTE]
>
>Esta página aborda os destinos nos quais os públicos-alvo são ativados de **a**, como as plataformas de armazenamento em nuvem. Para ativar os públicos-alvo **para um colaborador** em um projeto compartilhado, consulte o guia [ativar públicos-alvo](/help/guide/collaborate/activate.md).

Destinos são integrações usadas para enviar públicos-alvo direcionados para plataformas externas. Essas integrações permitem ativar públicos em vários canais e plataformas de marketing para uso em campanhas e no engajamento do cliente.

Os colaboradores podem configurar destinos para enviar públicos-alvo para plataformas externas, como o Adobe Experience Platform ou uma plataforma de armazenamento em nuvem, para uso em campanhas. Os colaboradores podem [ativar públicos-alvo em um projeto](../collaborate/activate.md), que são enviados para o destino configurado de sua conexão. A ativação pode ser feita por qualquer um dos colaboradores, dependendo das configurações de ativação de público-alvo [definidas na conexão](/help/guide/connect/establishing-connections.md#configure-connection-settings).

>[!IMPORTANT]
>
>Atualmente, quando os colaboradores ativam os públicos-alvo em um projeto, eles são automaticamente enviados para o destino configurado da conexão. Você **deve** configurar um destino para que seu colaborador possa ativar públicos-alvo em um projeto.

## Destinos disponíveis {#available-destinations}

Os seguintes destinos estão disponíveis para configuração no Collaboration. Para exibir o guia de configuração desse destino, selecione o nome do destino na tabela abaixo.

| Destino | Disponibilidade |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | Disponível |
| [[!DNL Amazon S3]](./manage-destinations.md) | Disponível |
| [[!DNL Snowflake]](./manage-destinations.md) | Disponível |
| [[!DNL Google Cloud Storage]](./manage-destinations.md) | Disponível |
| [[!DNL Azure Blob Storage]](./manage-destinations.md) | Disponível |
| [[!DNL SFTP]](./manage-destinations.md) | Disponível |
| [[!DNL Data Landing Zone]](./manage-destinations.md) | Disponível |

>[!NOTE]
>
>**[!DNL Google Cloud Storage]** nesta tabela refere-se a **destinos** (em que o Collaboration envia públicos-alvo durante a ativação). Para **originar públicos-alvo de** um bucket de GCS no espaço de trabalho **[!UICONTROL Configuração]**, consulte [Configurar GCS para fornecimento de público-alvo](../setup/configure-gcs-audience-sourcing.md).

## Próximas etapas

Para configurar um destino, consulte o guia [configurar e gerenciar um destino](./manage-destinations.md). Depois de configurar o destino, você pode começar a [ativar públicos-alvo direcionados](../collaborate/activate.md) nos seus projetos.
