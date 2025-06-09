---
title: Gerenciar conexões de dados
description: Saiba como gerenciar conexões de dados, incluindo chaves de correspondência, agendamento, casos de uso e filtragem de público-alvo no Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 15%

---

# Gerenciar conexões de dados

{{limited-availability-release-note}}

## Visão geral

Use conexões de dados no Real-Time CDP Collaboration para importar públicos de várias fontes. Saiba como gerenciar chaves de correspondência e agendar importações de dados para suas conexões de dados existentes. Além disso, você poderá filtrar públicos-alvo por atributos diferentes para obter insights mais granulares.

## Exibir conexões de dados

Para exibir as conexões de dados existentes, navegue até **[!UICONTROL Instalação]** e selecione a guia **[!UICONTROL Minhas conexões de dados]**. Todas as conexões de dados atuais são exibidas, mostrando uma breve visão geral de cada conexão. Para obter uma exibição completa das informações de uma conexão de dados, incluindo suas chaves de correspondência, detalhes do agendamento e públicos-alvo, selecione **[!UICONTROL Exibir conexão de dados]** na conexão correspondente.

![O espaço de trabalho de Instalação com a exibição de guia Minhas conexões de dados foi exibido e realçado.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### Chaves de correspondência {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Chaves de correspondência"
>abstract="As chaves de correspondência determinam como os dados de diferentes fontes serão correspondidos. Escolha as chaves de correspondência mais relevantes para seus casos de uso e diretrizes de privacidade."

As chaves de correspondência são identificadores usados para reconciliar membros entre públicos-alvo de diferentes fontes de dados. Não é possível editar as chaves de correspondência selecionadas inicialmente para a conexão de dados.

As chaves de correspondência disponíveis incluem:

- **Email com hash**

![Um espaço de trabalho de conexões de dados com a seção Corresponder chaves realçada.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Agendamento {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Agendamento"
>abstract="Essa exibição mostra as opções de agendamento selecionadas inicialmente para a conexão de dados."

Não é possível editar as opções de agendamento selecionadas inicialmente para a conexão de dados. Para obter mais informações sobre opções de agendamento, exiba a [seção de agendamento](/help/guide/setup/onboard-audiences.md#schedule) no documento de fluxo de trabalho de importação de público-alvo.

![Um espaço de trabalho de conexões de dados com a seção Agendamento realçada.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## Excluir conexão de dados

A exclusão de uma conexão de dados removerá todos os públicos-alvo subjacentes, as configurações associadas e o uso na plataforma. Essa ação não pode ser desfeita.

Para excluir uma conexão de dados existente, selecione o ícone de exclusão (![Ícone de exclusão](/help/assets/common/delete.svg)) no espaço de trabalho de uma conexão de dados individual.

![Um espaço de trabalho de conexões de dados com a opção de exclusão realçada.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

Uma caixa de diálogo de confirmação será exibida. Selecione **[!UICONTROL Excluir]** para concluir a exclusão da conexão de dados.

![A caixa de diálogo Excluir conexão de dados com a opção Excluir foi realçada.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Gerenciar públicos {#manage-audiences}

Uma lista de públicos-alvo anexados à conexão de dados é exibida na parte inferior do espaço de trabalho. A lista exibe uma breve visão geral de cada público-alvo, incluindo status, origem e acesso à conexão. Para editar as categorias, o acesso à conexão ou a visibilidade dos metadados de um público, selecione o nome do público. Para obter um guia completo sobre como gerenciar um público, consulte o guia [exibir públicos-alvo individuais](./onboard-audiences.md#view-individual-audiences).

![Um espaço de trabalho de conexões de dados com os públicos-alvo realçados.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Próximas etapas

Depois de gerenciar suas conexões de dados, você pode [descobrir sobreposições](/help/guide/collaborate/discover.md) entre os públicos-alvo e os públicos que o seu colaborador tornou visíveis.
