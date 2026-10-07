---
title: Criar públicos de expansão em Expandir
description: Saiba como criar públicos de expansão de um público inicial usando a população de público-alvo de um colaborador no Adobe Real-Time CDP Collaboration.
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
source-git-commit: 5b308de53e76129c8d5f3870ff4646424c2dd69e
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 1%
---
# (Beta) Criar públicos de expansão em Expandir

Use a guia **[!UICONTROL Expandir]** em um projeto para criar um público-alvo de expansão de um de seus públicos-alvo. O Collaboration usa a população de público-alvo do seu colaborador para encontrar perfis que se assemelham ao seu público-alvo inicial, ajudando você a alcançar novos clientes potenciais sem expor os dados de público-alvo subjacentes do seu colaborador. O público-alvo de expansão resultante é enviado ao colaborador para ativação.

## Pré-requisitos {#prerequisites}

Antes de usar a guia **[!UICONTROL Expandir]**, você deve ter:

* [Fornecido](/help/guide/setup/onboard-audiences.md) pelo menos um público-alvo para usar como um público-alvo de propagação
* [Conectado](/help/guide/connect/establishing-connections.md) com um colaborador
* [Criou um projeto](/help/guide/collaborate/manage-projects.md) com esse colaborador
* Se você estiver recebendo um público de expansão, um [destino](/help/guide/destinations/overview.md) configurado para receber públicos ativados

## Expandir visão geral {#expand-overview}

Navegue até **[!UICONTROL Colaborar]** > **[!UICONTROL Meus projetos]**, abra um projeto e selecione a guia **[!UICONTROL Expandir]**.

A página **[!UICONTROL Expandir]** mostra os públicos-alvo de expansão criados para este colaborador e a opção para criar um novo.

![A guia Expandir mostrando a tabela de públicos-alvo de Expansão com as colunas Nome, Status, Tamanho do modelo, Alcance do público-alvo e Última atualização.](/help/assets/collaborate/expand/expand-overview.png){zoomable="yes"}

A tabela **[!UICONTROL Públicos-alvo de expansão]** lista cada público-alvo de expansão criado no projeto:

| Coluna | Descrição |
|---|---|
| **[!UICONTROL Nome]** | O nome do público-alvo de expansão. O padrão é o nome do público-alvo inicial até a edição. |
| **[!UICONTROL Status]** | O status atual do público-alvo de expansão. Consulte [status do público-alvo de expansão](#expansion-audience-status) para obter detalhes. |
| **[!UICONTROL Tamanho do modelo]** | O tamanho do público de expansão gerado. Não disponível até que o modelo conclua o processamento. |
| **[!UICONTROL Alcance do público-alvo]** | A configuração de alcance de público usada para o público de expansão. |
| **[!UICONTROL Última atualização]** | A data e a hora em que o público-alvo de expansão foi atualizado pela última vez. |

{style="table-layout:auto"}

### Status do público-alvo de expansão {#expansion-audience-status}

Um público-alvo de expansão passa pelos seguintes status:

| Status | Descrição |
|---|---|
| **[!UICONTROL Processando]** | O modelo de expansão ainda está gerando o público-alvo de expansão. |
| **[!UICONTROL Rascunho]** | O modelo foi concluído e o público-alvo de expansão está pronto para ser revisado e enviado ao colaborador. |
| **[!UICONTROL Ativo]** | Você enviou o público-alvo de expansão para seu colaborador. |

{style="table-layout:auto"}

>[!NOTE]
>
>O status não é atualizado em tempo real. Reabra ou atualize a guia **[!UICONTROL Expandir]** para ver o status mais recente.

## Criar um público-alvo de expansão {#create-expansion-audience}

Para criar um novo público-alvo de expansão, selecione o ícone adicionar (![Ícone Adicionar.](/help/assets/icons/plus.png)) na página **[!UICONTROL Expandir]**, selecione **[!UICONTROL Criar um público-alvo expandido]**.


A caixa de diálogo **[!UICONTROL Gerar um público-alvo de expansão]** é exibida. Preencha todos os campos para gerar o público-alvo de expansão.

![A caixa de diálogo Gerar expansão de público-alvo com os campos Seed audience, Audience reach, Match key e Seed audience member.](/help/assets/collaborate/expand/generate-expansion-audience-dialog.png){zoomable="yes"}

### Selecione seu público inicial {#select-seed-audience}

Selecione um dos seus próprios públicos na lista suspensa **[!UICONTROL Selecione seu público alvo inicial]**. O Collaboration usa esse público-alvo como a base para encontrar perfis semelhantes na população do colaborador.

![O campo Seed audience na caixa de diálogo Gerar expansão de público-alvo.](/help/assets/collaborate/expand/select-seed-audience.png){zoomable="yes"}

### Selecionar uma chave correspondente {#select-match-key}

Ative uma chave de correspondência para o público-alvo de expansão. Não é possível habilitar mais de um.

| IDs de pessoas | IDs de dispositivos |
|---|---|
| **[!UICONTROL Email com hash]** | **[!UICONTROL IPv4]** com hash |
| **[!UICONTROL Telefone com hash]** | **[!UICONTROL GAID]** |
| **[!UICONTROL ID de fidelidade]** | **[!UICONTROL IDFA]** |
| **[!UICONTROL ID DO CRM]** | **[!UICONTROL ID do Demdex]** |

{style="table-layout:auto"}

>[!NOTE]
>
>Se o público-alvo inicial não incluir uma determinada chave de correspondência, essa opção aparecerá desativada e não poderá ser selecionada.

![A seção Chave de correspondência na caixa de diálogo Gerar expansão de público-alvo com as opções de chave de correspondência disponíveis.](/help/assets/collaborate/expand/select-match-key.png){zoomable="yes"}

### Selecione seu alcance de público {#select-audience-reach}

Use a lista suspensa **[!UICONTROL Alcance de público-alvo]** para equilibrar a similaridade com seu público-alvo inicial com o alcance geral. Selecione **[!UICONTROL Balanceado]** para um meio-termo entre a similaridade com seu público-alvo de propagação e o alcance geral.

![O campo Alcance do público-alvo na caixa de diálogo Gerar expansão de público-alvo com a opção Equilibrado selecionada e o texto de descrição abaixo dele.](/help/assets/collaborate/expand/select-audience-reach.png){zoomable="yes"}

### Incluir ou excluir seu público-alvo inicial {#include-exclude-seed-audience}

Use os botões de opção **[!UICONTROL Seed audience]** para escolher se o público alvo inicial original será incluído ou excluído do público-alvo da expansão final.

![O campo Membros do público-alvo de propagação na caixa de diálogo Gerar expansão de público-alvo com os botões de opção Sim e Não.](/help/assets/collaborate/expand/include-exclude-seed-audience.png){zoomable="yes"}

### Gerar o público-alvo de expansão {#generate-expansion-audience}

Depois que todos os campos forem concluídos, selecione **[!UICONTROL Gerar público-alvo de expansão]**. Uma mensagem de confirmação confirma que o Collaboration está criando o público-alvo de expansão e que você pode acompanhar seu progresso na página **[!UICONTROL Expandir]**.

## Revisar e enviar um público-alvo de expansão {#review-send-expansion-audience}

Depois que o status de um público-alvo de expansão for atualizado para **[!UICONTROL Rascunho]**, selecione seu nome na tabela **[!UICONTROL Públicos-alvo de expansão]** para abri-lo.

![A página de detalhes Expansão de Público-Alvo, que mostra os metadados do público-alvo, o tamanho do modelo, o tamanho do público-alvo de propagação e o botão Enviar.](/help/assets/collaborate/expand/expansion-audience-detail.png){zoomable="yes"}

Nessa visualização, é possível:

* Editar o nome do público-alvo de expansão
* Visualizar a data e a hora da criação
* Comparar o tamanho do público-alvo de propagação com o tamanho do público-alvo de expansão gerado
* Revisar a chave de correspondência usada para gerar o público-alvo

Quando estiver pronto, selecione **[!UICONTROL Enviar para parceiro]** para enviar o público-alvo de expansão para seu colaborador. O público-alvo permanece com o status de **[!UICONTROL Rascunho]** até que você o envie e, em seguida, atualiza para **[!UICONTROL Ativo]**.

>[!NOTE]
>
>Se o seu colaborador não tiver um destino configurado, **[!UICONTROL Enviar para parceiro]** não estará disponível. Uma mensagem explica que seu colaborador precisa configurar um destino primeiro.

>[!IMPORTANT]
>
>Um público-alvo de expansão expira 7 dias após ser gerado, caso não seja enviado para o colaborador.

## Receber e ativar um público-alvo de expansão {#receive-activate-expansion-audience}

Ao enviar um público-alvo de expansão, o Collaboration o entrega ao seu colaborador de acordo com a configuração de ativação definida para a conexão:

* Se a **ativação automática** estiver habilitada, o Collaboration ativará automaticamente o público-alvo de expansão para o destino configurado do seu colaborador e ele aparecerá na [guia Ativar](./activate.md#activated-audiences).
<!-- Beta release: automatic activation is the only available activation setting. Uncomment the manual activation guidance below when manual activation is introduced with the GA release. -->
<!-- * If **manual activation** is enabled, the expansion audience appears in your collaborator's [Received audiences](./activate.md#received-audiences) section of the **[!UICONTROL Activate]** tab, and your collaborator must manually activate it. -->

## Próximas etapas

Depois de enviar o público-alvo de expansão, use a [guia Descobrir](./discover.md) para compará-lo com outros públicos-alvo ou a [guia Ativar](./activate.md) para acompanhar sua ativação.
