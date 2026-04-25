---
title: Criar e gerenciar projetos
description: Saiba como criar e gerenciar projetos no Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: ae492846-bc0a-4422-86ca-577bcc1fa60c
TQID: https://experienceleague.adobe.com/IZIkK4lv29vqrah48fsJsnMOFtyh7rOo1IT2yLOW9Ec
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 680
ht-degree: 11%

---

# Criar e gerenciar projetos

{{limited-availability-release-note}}

Os projetos são a parte central do fluxo de trabalho no Adobe Real-Time CDP Collaboration. Depois de se conectar com colaboradores, crie um projeto para executar cálculos de sobreposição de público e descobrir públicos relevantes para campanhas.

>[!TIP]
>
>Geralmente, os projetos devem ser associados a uma única campanha.

![O painel Colaborar mostrando todos os projetos atuais.](/help/assets/collaborate/manage-view-projects/projects-overview-page.png){zoomable="yes"}

Você pode usar filtros para exibir somente os projetos iniciados com determinados colaboradores, conforme mostrado abaixo:

![Exibição filtrada de projetos com um único colaborador.](/help/assets/collaborate/manage-view-projects/filtered-project-view.png){zoomable="yes"}

## Criar projeto {#create-project}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_create_project_advertisername_amc"
>title="Nome do anunciante (Amazon Marketing Cloud)"
>abstract="Para conexões do Amazon Marketing Cloud (AMC), esse campo representa a instância do AMC à qual o logon do Amazon Ads tem acesso. Ele não reflete um nome de anunciante. Se a instância exigida não estiver listada, entre em contato com o(a) admin do Amazon Marketing Cloud para solicitar acesso."

Para criar um projeto, primeiro [estabeleça uma conexão](/help/guide/connect/establishing-connections.md) com um colaborador. Depois que a conexão for estabelecida, você poderá criar um projeto com esse colaborador.

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_projects_advertisername"
>title="Nome do anunciante"
>abstract="Selecione o nome do anunciante no menu suspenso. As opções são pré-configuradas pelo editor nas configurações de conexão para garantir a compatibilidade com seus sistemas."

Navegue até **[!UICONTROL Colaborar]** e depois **[!UICONTROL Meus Projetos]**. Se este for seu primeiro projeto, você pode selecionar **[!UICONTROL Criar um projeto]**. Caso contrário, você pode selecionar o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)) para criar um novo projeto a qualquer momento.

![Selecione o símbolo de adição ou Crie um projeto para configurar um novo projeto.](/help/assets/collaborate/manage-view-projects/create-project.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Criar projeto]** é exibida. Selecione o **[!UICONTROL Colaborador]** com o qual você está criando o projeto por meio da lista suspensa. Se você for um publicador e definir nomes de anunciante durante a configuração da conexão, poderá selecionar o **[!UICONTROL Nome do anunciante]**.

>[!NOTE]
>
> Se você tiver configurado um único nome de anunciante nas configurações de conexão, ele aparecerá por padrão. Se nenhum nome de anunciante foi configurado, o **[!UICONTROL Nome]** do anunciante será pré-selecionado como o **[!UICONTROL Nome do anunciante]**.

![Criar caixa de diálogo de projeto com colaborador selecionado e nome de anunciante realçado.](/help/assets/collaborate/manage-view-projects/create-project-advertiser-names.png){zoomable="yes"}

Em seguida, adicione um **[!UICONTROL Nome do projeto]** e uma **[!UICONTROL Descrição]** para o seu projeto. Em seguida, selecione uma imagem para representar o projeto. Esta imagem ajuda a distinguir o projeto na página de visão geral do projeto. Quando terminar, selecione **[!UICONTROL Criar]** para criar o projeto.

![Opções necessárias para configurar um novo projeto](/help/assets/collaborate/manage-view-projects/create-project-required-info.png){zoomable="yes"}

Agora você pode visualizar o novo projeto, seus detalhes e as seções disponíveis com base nos casos de uso selecionados durante a configuração da conexão.

![O espaço de trabalho de visão geral do projeto.](/help/assets/collaborate/manage-view-projects/project-overview.png){zoomable="yes"}

## Gerenciar ID da campanha {#manage-campaign-id}

Uma **ID de Campanha** vincula seu projeto a uma campanha específica e é necessária para [gerar relatórios de medição](./measure.md#create-measurement-report). Você pode adicionar várias IDs de campanha a um projeto se executar várias campanhas com o mesmo colaborador. Todas essas campanhas estão disponíveis para seleção nos relatórios.

- **Publicadores**: insira ou atualize IDs de campanha e nomes associados na interface do usuário do Collaboration antes de executar os relatórios.
- **Anunciantes**: solicite ao seu colaborador (editor) que adicione IDs de campanha conforme necessário.

Para adicionar ou atualizar IDs de campanha, navegue até o espaço de trabalho **[!UICONTROL Colaborar]** e selecione **[!UICONTROL Exibir]** no cartão de projeto relevante.

![O espaço de trabalho Colaborar destacando a opção Exibir em um cartão de projeto.](/help/assets/collaborate/manage-view-projects/view-project.png){zoomable="yes"}

O espaço de trabalho **[!UICONTROL Visão geral do projeto]** correspondente aparece com uma seção **[!UICONTROL ID e nome da campanha]** que lista todas as campanhas vinculadas ao projeto. Se você ainda não tiver adicionado uma campanha, selecione **[!UICONTROL Adicionar]**. Se já houver campanhas presentes, selecione **[!UICONTROL Editar]** para atualizar detalhes ou adicionar outros.

![O espaço de trabalho de visão geral do projeto exibindo a ID da Campanha e a seção de nome com a opção Editar realçada.](/help/assets/collaborate/manage-view-projects/edit-campaign-id.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL ID e nome da campanha]**, selecione **[!UICONTROL Adicionar ID da campanha]** para adicionar uma nova linha, onde você pode inserir os detalhes da campanha.

![A caixa de diálogo ID e nome da campanha exibindo a linha de campanha vazia após selecionar a opção Adicionar ID da campanha.](/help/assets/collaborate/manage-view-projects/add-campaign-row.png){zoomable="yes"}

Forneça a **[!UICONTROL ID da Campanha]** e o **[!UICONTROL nome da campanha]** e selecione **[!UICONTROL Salvar]**.

![Caixa de diálogo de ID e nome da campanha mostrando os novos detalhes da campanha e a opção Salvar realçada.](/help/assets/collaborate/manage-view-projects/save-campaign-id.png){zoomable="yes"}

Verifique a seção **[!UICONTROL ID e nome da campanha]** para exibir suas campanhas mais recentes e as alterações recentes. Agora você pode usar as novas IDs de campanha para gerar relatórios de medição.

![O espaço de trabalho de visão geral do projeto exibindo a ID da campanha e a seção de nome atualizadas.](/help/assets/collaborate/manage-view-projects/view-updated-campaigns.png){zoomable="yes"}
