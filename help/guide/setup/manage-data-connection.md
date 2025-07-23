---
title: Gerenciar conexões de dados
description: Saiba como gerenciar conexões de dados, incluindo chaves de correspondência, agendamento, casos de uso e filtragem de público-alvo no Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 12%

---

# Gerenciar conexões de dados

{{limited-availability-release-note}}

## Visão geral

Use conexões de dados no Real-Time CDP Collaboration para originar públicos-alvo de várias plataformas. Saiba como gerenciar chaves de correspondência e agendar a atualização de dados para suas conexões de dados existentes. Além disso, você poderá filtrar públicos-alvo por atributos diferentes para obter insights mais granulares.

## Exibir conexões de dados

Para exibir as conexões de dados existentes, navegue até **[!UICONTROL Instalação]** e selecione a guia **[!UICONTROL Minhas conexões de dados]**. Todas as conexões de dados atuais são exibidas, mostrando uma breve visão geral de cada conexão. Para obter uma exibição completa das informações de uma conexão de dados, incluindo suas chaves de correspondência, detalhes do agendamento e públicos-alvo, selecione **[!UICONTROL Exibir conexão de dados]** na conexão correspondente.

![O espaço de trabalho de Instalação com a exibição de guia Minhas conexões de dados foi exibido e realçado.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### Chaves de correspondência {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Chaves de correspondência"
>abstract="As chaves de correspondência determinam como os dados de diferentes fontes serão correspondidos. Escolha as chaves de correspondência mais relevantes para seus casos de uso e diretrizes de privacidade."

As chaves de correspondência são identificadores usados para reconciliar membros entre públicos-alvo de diferentes fontes de dados. Não é possível editar as chaves de correspondência selecionadas inicialmente para a conexão de dados.

>[!IMPORTANT]
> 
>As chaves de correspondência não podem ser editadas após a criação da conexão de dados. Para atualizar chaves de correspondência, você deve criar uma nova conexão de dados.

As chaves de correspondência disponíveis incluem:

- **Email com hash**

![Um espaço de trabalho de conexões de dados com a seção Corresponder chaves realçada.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Agendamento {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Agendamento"
>abstract="Exiba os detalhes de agendamento da conexão de dados e edite a frequência de atualização, se necessário."

Exibir e gerenciar as configurações de agendamento para suas conexões de dados. O agendamento determina a frequência com que o público-alvo é atualizado.

Após criar uma conexão de dados, você poderá atualizar sua frequência de atualização diretamente na seção **[!UICONTROL Agendamento]** do espaço de trabalho da conexão de dados.

>[!NOTE]
>
>Ao fornecer públicos-alvo da Adobe Experience Platform, os públicos-alvo se tornam disponíveis em 24 horas após a conexão de dados ser estabelecida. Após a importação inicial, os dados do público-alvo são atualizados de acordo com a frequência definida.

Para obter mais informações sobre agendamento, consulte a [seção de agendamento](/help/guide/setup/onboard-audiences.md#schedule) no guia para configurar públicos.

![Um espaço de trabalho de conexão de dados com a seção Agendamento realçada.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

#### Editar agendamento {#edit-scheduling}

É possível editar a frequência de uma conexão de dados existente para controlar melhor a frequência com que os públicos-alvo são atualizados. Para editar o agendamento, selecione **[!UICONTROL Editar]** na conexão de dados do cartão de agendamento.

Na caixa de diálogo **[!UICONTROL Agendamento]**, selecione o menu suspenso para atualizar a **[!UICONTROL Frequência]**. Defina a frequência de atualização para ser executada diariamente ou a cada dois ou seis dias. Quando terminar, selecione **[!UICONTROL Salvar]** para aplicar as alterações.

![A caixa de diálogo Agendamento, mostrando opções para definir a frequência e o intervalo de datas.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## Excluir conexão de dados

A exclusão de uma conexão de dados removerá todos os públicos-alvo subjacentes, as configurações associadas e o uso no Collaboration. Essa ação não pode ser desfeita.

Para excluir uma conexão de dados existente, selecione o ícone de exclusão (![Ícone de exclusão](/help/assets/common/delete.svg)) no espaço de trabalho de uma conexão de dados individual.

![Um espaço de trabalho de conexões de dados com a opção de exclusão realçada.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

Uma caixa de diálogo de confirmação será exibida. Selecione **[!UICONTROL Excluir]** para concluir a exclusão da conexão de dados.

![A caixa de diálogo Excluir conexão de dados com a opção Excluir foi realçada.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Gerenciar públicos {#manage-audiences}

Uma lista de públicos-alvo anexados à conexão de dados é exibida na parte inferior do espaço de trabalho. A lista exibe uma breve visão geral de cada público-alvo, incluindo status, origem e acesso à conexão. Para editar as categorias, o acesso à conexão ou a visibilidade dos metadados de um público, selecione o nome do público. Para obter um guia completo sobre como gerenciar um público, consulte o guia [exibir públicos-alvo individuais](./onboard-audiences.md#view-individual-audiences).

![Um espaço de trabalho de conexões de dados com os públicos-alvo realçados.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Próximas etapas

Depois de gerenciar suas conexões de dados, você pode [descobrir sobreposições](/help/guide/collaborate/discover.md) entre os públicos-alvo e os públicos que o seu colaborador tornou visíveis.
