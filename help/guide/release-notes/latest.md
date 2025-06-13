---
title: Notas de versão mais recentes do Real-Time CDP Collaboration
description: Seguir as versões mais recentes do Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: b52fd181d80d5a70331571f7a4cbe3e5a7ec1d7c
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 3%

---

# Notas de versão mais recentes do Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Última atualização**: abril de 2025.

Essas notas de versão abordam a funcionalidade lançada no Real-Time Customer Data Platform Collaboration. As versões do Real-Time CDP Collaboration operam em um modelo de entrega contínua, que permite uma cadência de lançamento mensal aproximada. Essas notas de versão são atualizadas com frequência. Portanto, verifique-as regularmente.

## Maio de 2025 {#may-2025}

* O Real-Time CDP Collaboration agora está disponível para clientes na **Austrália** e na **Nova Zelândia**. Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate nessas regiões.
* O Real-Time CDP Collaboration agora oferece [destinos de autoatendimento](../setup/manage-destinations.md) por meio da guia **[!UICONTROL Meus destinos]** na seção **[!UICONTROL Configuração]**. Os destinos permitem ativar públicos-alvo em plataformas de terceiros, como redes de publicidade ou plataformas de gerenciamento de dados, para alcançar seus clientes em vários canais. No momento, somente os destinos do Adobe Experience Platform são compatíveis. Se você estiver interessado em configurar um destino diferente, entre em contato com o representante da Adobe. Para saber mais sobre destinos, leia o guia [visão geral dos destinos](../destinations/overview.md).

   * Destinos também adiciona suporte para exibir públicos da Real-Time CDP Collaboration no [portal de público-alvo da Adobe Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences.).

* Agora você pode editar a frequência de atualização do público-alvo para conexões de dados existentes no Real-Time CDP Collaboration. Atualmente, você pode optar por atualizar os públicos-alvo diariamente ou a cada dois ou seis dias. Para saber mais sobre como editar a frequência de atualização do público-alvo, leia o guia [gerenciar conexões de dados](../setup/manage-data-connection.md#scheduling).
* As divisões de crédito entre colaboradores agora são definidas para cada caso de uso selecionado na conexão. Você pode definir diferentes regras de consumo de crédito para cada caso de uso para controlar melhor como seus créditos são usados. Para saber mais sobre a funcionalidade de divisão de crédito, leia o guia [configurações de conexão](../connect/establishing-connections.md#connection-settings). Para saber mais sobre como os créditos são consumidos, leia o guia [tipos de atividade de crédito](../setup/my-activity.md#types-of-activities). <br> ![Tela de configurações de conexão mostrando a funcionalidade de divisão de crédito.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Agora, os editores podem definir nomes e IDs de anunciante antes de aceitar as configurações de conexão de um anunciante. Os editores podem definir nomes e IDs que se alinham a seus sistemas internos, que podem ser diferentes dos nomes e IDs do anunciante. Para saber mais sobre como adicionar nomes e IDs de anunciante, leia o guia [configurações de conexão](../connect/establishing-connections.md#connection-settings.md). <br> ![Tela de configurações de conexão mostrando o publicador definindo nomes e IDs de anunciante.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## Abril de 2025 {#april-2025}

* Uma nova coluna **[!UICONTROL Entradas Processadas]** foi adicionada à tabela de atividade de consumo de crédito. Essa coluna exibe o número total de entradas (por exemplo, IDs ou linhas) processadas para cada atividade. [Leia mais](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Coluna processada de entradas realçada na exibição Minha atividade.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Uma nova opção de email de contato foi adicionada à criação da conta. Isso ajuda os colaboradores do parceiro a contatarem você, conforme necessário, durante o processo de conexão. [Leia mais](../setup/onboard-organization.md).

## Março de 2025 {#march-2025}

* Ao [importar públicos](/help/guide/setup/onboard-audiences.md) para o Real-Time CDP Collaboration, agora é possível definir uma frequência de atualização de público de **a cada um a seis dias** para gerenciar melhor a [atividade de crédito de Gerenciamento de público](/help/guide/setup/my-activity.md#types-of-activities). [Leia mais](/help/guide/setup/onboard-audiences.md#schedule). <br> ![A tela Agendar mostra intervalos de frequência diferentes para atualizar a associação de público-alvo.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Tela de agendamento mostrando intervalos de frequência diferentes para atualizar associação de público-alvo."){width="250" align="center" zoomable="yes"}
* Ao estabelecer uma conexão com um colaborador, agora é possível selecionar **casos de uso** predefinidos. O caso de uso selecionado determina quais seções do projeto e funcionalidades do produto ficam disponíveis. [Leia mais](/help/guide/collaborate/manage-projects.md#project-use-cases).
   * *A medição* habilita a seção de projeto **Medida**.
   * A *descoberta de público-alvo* habilita a seção de projeto **Descoberta**.
   * *A ativação de público* habilita as **Ativar** seções de projeto <br>
* Agora você pode excluir conexões com colaboradores com os quais não deseja mais trabalhar. [Leia mais](/help/guide/connect/establishing-connections.md#delete-connections).


## Fevereiro de 2025 - Disponibilidade geral para clientes dos EUA {#february-2025-ga}

O Real-Time CDP Collaboration, criado especificamente para permitir que anunciantes e editores descubram, ativem e meçam públicos-alvo de alto valor sem cookies de terceiros, agora está disponível de modo geral nos Estados Unidos.

### Introdução

1. **Configuração do Access**: os administradores do sistema configuram permissões de acesso para usuários. [Leia mais](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access).
2. **Conectar Fontes de Dados**: importe audiências para usar no Real-Time CDP Collaboration. [Leia mais](/help/guide/setup/onboard-audiences.md).
3. **Estabelecer Conexões de Parceiro**: comece a colaborar com marcas ou editores confiáveis. [Leia mais](/help/guide/connect/establishing-connections.md).
4. **Descobrir e ativar**: crie projetos para identificar segmentos de público-alvo valiosos e ativar em campanhas. [Leia mais](/help/guide/collaborate/manage-projects.md).

### Disponibilidade

* No momento, o Real-Time CDP Collaboration está disponível somente para clientes dos EUA.
* Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate

Para obter mais informações, leia:

* [Visão geral do Real-Time CDP Collaboration](/help/guide/home.md)
* [Fluxo de trabalho de ponta a ponta](/help/guide/end-to-end-workflow.md)
* [Visão geral de permissões](/help/guide/permissions/overview.md)
