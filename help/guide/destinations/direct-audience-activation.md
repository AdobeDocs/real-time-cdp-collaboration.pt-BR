---
title: Ativar públicos diretamente (Audience Activation 1P) - Beta
description: Saiba como ativar públicos-alvo primários próprios ou compartilhados sem um projeto, selecionar um destino, revisar mapeamentos de campos e definir um agendamento de ativação.
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%
---

# Ativar públicos diretamente (Audience Activation 1P) {#activate-audiences-directly}

Use a ativação direta de público primário (1P) no [!DNL Adobe Real-Time CDP Collaboration] para enviar públicos-alvo para um destino sem criar um projeto. Ative os públicos que você possui ou os públicos compartilhados com você para uso próprio.

Comece a partir de um destino configurado para **[!UICONTROL Públicos-alvo ativados]**, selecione públicos-alvo e defina o agendamento de ativação.

Para enviar e ativar públicos-alvo por meio de um projeto de colaboração, consulte [Enviar e ativar públicos-alvo em um projeto](/help/guide/collaborate/activate.md).

## Acesso de público para ativação {#audience-access-for-activation}

Verifique a origem do público-alvo para determinar se você precisa de uma concessão antes da ativação.

| Fonte do público-alvo | Requisito de acesso |
| --- | --- |
| Seus próprios públicos-alvo | Você é o proprietário dos públicos-alvo. |
| Públicos-alvo compartilhados com você | Você precisa de uma concessão ativa com permissão de ativação direta. O provedor retém a propriedade. |

{style="table-layout:auto"}

Uma concessão de público-alvo virtual fornece acesso a um público-alvo compartilhado por referência sem mover seus dados. Em seguida, você pode ativar o público-alvo para enviar os dados ao destino selecionado.

Para obter detalhes sobre concessões e controles de provedor, consulte [Acesso de público-alvo virtual (concessões de público-alvo)](/help/guide/setup/virtual-audience-access.md).

## Pré-requisitos {#prerequisites}

Antes de começar, confirme se você tem:

* Um público-alvo que você possui ou um público-alvo compartilhado por meio de uma concessão de qualificação primária (1P).
* Um destino configurado que você controla e que oferece suporte à ativação direta.
* Pelo menos um mapeamento de campo de chave de correspondência para o destino.

Para ativar um público-alvo compartilhado, confirme se sua concessão ativa com escopo de conexão atende às [condições de qualificação](#check-shared-audience-access). Use o espaço de trabalho **[!UICONTROL Ativação]**. Você não precisa de um projeto.

### Elegibilidade de público compartilhado {#check-shared-audience-access}

A concessão deve atender a cada condição para apoiar a ativação direta.

| Requisito | Condição |
| --- | --- |
| Permissão de público | A concessão inclui permissão de ativação direta. |
| Duração do acesso | A concessão está ativa indefinidamente ou dentro do intervalo de datas especificado. |

{style="table-layout:auto"}

A permissão **[!UICONTROL Criar novo público-alvo]** separada permite que você use um público-alvo compartilhado para a criação de um público-alvo de coorte. Você não precisa dessa permissão para a ativação direta.

### Mapeamentos de campo de destino {#review-destination-field-mappings}

A ativação direta usa os mapeamentos de chaves de correspondência configurados para o seu destino. Você não seleciona chaves correspondentes durante a ativação.

Para configurar destinos, consulte [visão geral sobre destinos](../destinations/overview.md).

## Iniciar ativação direta {#start-direct-activation}

Inicie a partir de um destino configurado ou da lista de públicos-alvo ativados. Os destinos do Adobe Experience Platform não oferecem suporte à ativação própria.

### Iniciar de um destino {#start-from-a-destination}

Para abrir o fluxo de trabalho com um destino selecionado, comece com esse destino configurado. Primeiro, abra o espaço de trabalho **[!UICONTROL Ativação]** e selecione **[!UICONTROL Destinos]**.

Em seguida, selecione **[!UICONTROL Ativar públicos-alvo]** nas ações para o destino que deseja usar.

O fluxo de trabalho é aberto com o destino selecionado. Em seguida, continue com [Configurar a ativação](#configure-the-activation).

### Iniciar com base em públicos ativados {#start-from-activated-audiences}

Para escolher um destino no fluxo de trabalho, comece na lista de públicos ativados. Primeiro, abra o espaço de trabalho **[!UICONTROL Ativação]** e selecione **[!UICONTROL Públicos ativados]**.

Em seguida, inicie o fluxo de trabalho selecionando **[!UICONTROL Ativar público-alvo]** na página ou selecionando o ícone adicionar (![Adicionar uma ativação de público-alvo.](/help/assets/icons/plus.png)) e **[!UICONTROL Ativar público-alvo]**.

O fluxo de trabalho é aberto sem um destino selecionado. Em seguida, continue com [Configurar a ativação](#configure-the-activation).

## Configurar a ativação {#configure-the-activation}

Selecione um público-alvo por ativação dos seus próprios públicos-alvo ou públicos-alvo compartilhados com você. Use o destino pré-selecionado ou escolha um destino configurado se nenhum estiver selecionado. O fluxo de trabalho aplica os [mapeamentos existentes](#review-destination-field-mappings) configurados para esse destino.

Escolha quando executar a ativação e revise o público-alvo, o destino e o agendamento selecionados antes de enviar.

## Acessar alterações e execuções programadas {#access-changes-and-scheduled-runs}

Ative um público compartilhado somente enquanto o provedor conceder o acesso.

| Alteração de acesso | Efeito |
| --- | --- |
| A concessão expira | O sistema processa a expiração a cada hora. O recipient perde o acesso do público-alvo virtual após o processamento da expiração. |
| O provedor revoga a concessão | O recipient perde o acesso ao público-alvo virtual imediatamente. |
| Uma ativação agendada é executada | O sistema verifica a concessão. Públicos-alvo com concessões revogadas ou expiradas não são qualificados para ativação. |

{style="table-layout:auto"}

A expiração ou revogação não remove os dados do público-alvo já entregues a um destino.

## Próximas etapas {#next-steps}

Após ativar os públicos-alvo, use esses guias para gerenciar destinos ou conexões de colaborador.

* [Configurar e gerenciar destinos](/help/guide/destinations/manage-destinations.md)
* [Gerenciar conexões do collaborator](/help/guide/connect/manage-connections.md)
