---
title: Visão geral de públicos-alvo
description: Saiba mais sobre os públicos-alvo no Real-Time CDP Collaboration, incluindo de onde eles podem ser obtidos.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: f7cd44177d60bfd3d3db384f7b1a250ace4c3633
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 3%

---


# Visão geral de públicos-alvo

{{limited-availability-release-note}}

No Adobe Real-Time CDP Collaboration, os públicos-alvo são grupos de usuários ou clientes que você traz para o Collaboration. Após o fornecimento, você pode usar públicos para descobrir sobreposições com colaboradores, ativar públicos e medir o desempenho da campanha. Você pode originar públicos-alvo de vários tipos de origem, incluindo Adobe Experience Platform, sistemas de armazenamento e compartilhamento em nuvem e fluxos de trabalho de upload de arquivos, dependendo de onde seus dados de público-alvo já estão.

## O que você pode fazer com os públicos {#audiences-in-collaboration}

Depois que um público-alvo é originado no Collaboration, ele se torna disponível para uso em fluxos de trabalho de colaboração compatíveis.

Use os públicos no Collaboration para:

* Comparar seu público-alvo com públicos-alvo de colaboração
* Identificar sobreposições e oportunidades
* Ativar públicos-alvo
* Medir resultados e desempenho da campanha
* Gerenciar a visibilidade do público-alvo e as configurações relacionadas

## Como os públicos-alvo se encaixam no Collaboration {#conceptual-diagram}

>[!NOTE]
>
> O diagrama a seguir fornece uma visualização de alto nível de como os públicos-alvo de origem se encaixam no Collaboration e são usados em projetos.

```text
Source → Data connection → Audience → Project
                                         │
                          ┌──────────────┼──────────────┐
                          ▼              ▼              ▼
                      Discover       Activate       Measure
                                         │
                                         ▼
                                    Destination
```

## Conceitos principais {#core-concepts}

Os conceitos a seguir descrevem os principais objetos envolvidos na origem de público-alvo e nos fluxos de trabalho de colaboração.

**Source**\
O sistema ou local onde os dados do público-alvo são originados, como Adobe Experience Platform, um local de armazenamento na nuvem ou um upload de arquivo.

**Conexão de dados**\
A conexão configurada que o Collaboration usa para acessar dados do público-alvo de uma origem. Uma conexão de dados inclui detalhes de configuração específicos da origem, como autenticação, mapeamento de campo e agendamento.

**Público-alvo**\
Um grupo de usuários ou clientes que foi incluído no Collaboration e está disponível para uso em projetos.

**Conexão**\
O relacionamento de colaboração entre sua organização e outra organização.

**Projeto**\
O espaço de trabalho em que os colaboradores usam os públicos-alvo juntos para casos de uso compatíveis, como descoberta, ativação e medição.

**Destino**\
A plataforma externa ou o sistema para o qual os públicos-alvo ativados são enviados.

**Corresponder chaves**
Identificadores que a Collaboration usa para corresponder registros em conjuntos de dados e colaboradores. As teclas de correspondência são compatíveis com fluxos de trabalho como sobreposição de público-alvo, ativação e medição.

## Ciclo de vida do público {#audience-lifecycle}

No Collaboration, você origina públicos-alvo por meio de conexões de dados, gerencia-os na **[!UICONTROL Instalação]** e os usa em projetos para casos de uso com suporte.

1. **Públicos-alvo do Source**: leve dados do público-alvo para o Collaboration por meio de uma conexão de dados.
2. **Gerenciar públicos-alvo**: revise e gerencie detalhes do público-alvo, visibilidade e configurações relacionadas.
3. **Usar públicos-alvo em projetos**: usar públicos-alvo de origem em projetos para casos de uso com suporte, incluindo **Descobrir**, **Ativar** e **Medir**.

Nem todo público-alvo é usado em todos os casos de uso. Por exemplo, um público pode ser originado e usado para **Discover** sem ser ativado ou pode ser usado em fluxos de trabalho de **Measure** sem ser enviado para um destino.

Para obter mais informações sobre seleção de fornecedor e gerenciamento de públicos, consulte [Source e gerenciar públicos](./onboard-audiences.md). Para obter informações sobre o gerenciamento de conexões de dados, consulte [Gerenciar conexões de dados](./manage-data-connection.md).

## De onde os públicos-alvo vêm {#supported-sources}

O Collaboration oferece suporte a vários tipos de fonte de público-alvo. A origem escolhida determina o fluxo de configuração, os pré-requisitos, os requisitos de autenticação, o formato de dados, o mapeamento de campos, o comportamento de atualização e as opções de configuração disponíveis para trazer públicos-alvo para a Collaboration.

* Adobe Experience Platform
* Armazenamento na nuvem, incluindo Amazon S3, Google Cloud Storage e armazenamento Azure
* Serviços de compartilhamento de dados, incluindo Snowflake e compartilhamento delta de databricks
* Adobe Audience Manager
* Upload de arquivo CSV

Para obter uma lista de origens com suporte e etapas de configuração específicas da origem, consulte [Visão geral das origens](./source-overview.md#available-sources).

## Do que os públicos-alvo são compostos {#match-keys}

Os públicos-alvo no RTCDP Collaboration são compostos de chaves de correspondência. Dependendo da configuração de sua conta, as chaves de correspondência com suporte podem incluir **IDs de Pessoas**, **IDs de Dispositivos** e **IDs de Parceiros**. As chaves de correspondência oferecem suporte a fluxos de trabalho como **sobreposição de público**, **ativação** e **medição**.

Para saber mais, consulte [Configurar chaves de correspondência](../setup/onboard-account.md#set-up-match-keys) e [Gerenciar conexões de dados](../setup/manage-data-connection.md#match-keys)

## Usar públicos-alvo em projetos {#audiences-in-projects}

Os projetos fornecem o contexto para colaborar com outra organização. Em um projeto, você pode usar os públicos-alvo para casos de uso de colaboração compatíveis:

* **Descobrir**: comparar públicos e analisar insights de sobreposição. Consulte [Descobrir sobreposição de público](../collaborate/discover.md).
* **Ativar**: ativar os públicos selecionados para uso da campanha. A ativação foi iniciada a partir da guia [!UICONTROL Ativar] no espaço de trabalho do projeto e envia públicos para o destino configurado da conexão. Consulte [Ativar públicos-alvo](../collaborate/activate.md).
* **Medida**: revise os relatórios de entrega e conversão de campanha associados ao projeto. Consulte [Medir desempenho](../collaborate/measure.md).

Para obter mais informações sobre como criar e gerenciar projetos, consulte [Criar e gerenciar projetos](../collaborate/manage-projects.md). Para obter informações sobre como configurar destinos, consulte [Visão geral sobre destinos](../destinations/overview.md).

## Próximas etapas {#next-steps}

* [Revisar fontes de público disponíveis](./source-overview.md)
* [Source e gerenciar públicos](./onboard-audiences.md)
* [Criar e gerenciar projetos](../collaborate/manage-projects.md)
* [Descobrir sobreposição de público](../collaborate/discover.md)
* [Ativar públicos-alvo](../collaborate/activate.md)
* [Medir desempenho](../collaborate/measure.md)
* [Visão geral dos destinos](../destinations/overview.md)
