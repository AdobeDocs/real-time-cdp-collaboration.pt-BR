---
title: Configurar e gerenciar destinos de armazenamento em nuvem
description: Saiba como configurar, exibir e excluir um destino de armazenamento na nuvem no Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 60124235569ca9b17b3bb1cef502d57d39e82e1f
workflow-type: tm+mt
source-wordcount: 885
ht-degree: 1%

---

# Configurar e gerenciar destinos de armazenamento em nuvem

Use este guia para configurar, exibir e excluir destinos de armazenamento em nuvem do espaço de trabalho **[!UICONTROL Ativação]**. Use a guia **[!UICONTROL Catálogo]** para configurar destinos, a guia **[!UICONTROL Destinos]** para gerenciá-los e a guia **[!UICONTROL Públicos-alvo ativados]** para revisar públicos-alvo ativados para destinos.

Após configurar um destino, ele fica disponível quando você ativa públicos. Para ver a lista completa de destinos com suporte, consulte a tabela [destinos disponíveis](./overview.md#available-destinations).

>[!NOTE]
>
> Este guia usa um destino **[!DNL Amazon S3]** como exemplo. O fluxo de trabalho de configuração guiado é compartilhado em todos os tipos de destino de armazenamento na nuvem compatíveis, mas os métodos de autenticação, os campos obrigatórios e os recursos de conector podem variar. Antes de configurar um destino, reveja os [requisitos de destino do armazenamento na nuvem](./cloud-storage-destination-requirements.md), que vinculam à documentação de destino correspondente do Adobe Experience Platform.
>
> O Adobe Experience Platform tem um fluxo de trabalho de configuração separado no Real-Time CDP Collaboration. Para configurá-lo, consulte [Configurar o Adobe Experience Platform como destino](./experience-platform.md).

## Pré-requisitos {#prerequisites}

Antes de configurar um destino, verifique se:

* Você tem acesso ao espaço de trabalho **[!UICONTROL Ativação]**.
* Você tem as informações de conexão exigidas pelo seu provedor de armazenamento na nuvem.
* Se precisar criar uma conta, você terá as credenciais ou permissões necessárias.
* Você analisou os [requisitos para seu destino de armazenamento na nuvem](./cloud-storage-destination-requirements.md).

## Configurar um destino {#configure-destination}

Ao configurar um destino, você conecta uma conta de armazenamento na nuvem ao Real-Time CDP Collaboration e define como os dados do público-alvo são exportados para ele.

Navegue até **[!UICONTROL Ativação]** > **[!UICONTROL Catálogo]**.

A guia **[!UICONTROL Catálogo]** exibe os provedores de destino disponíveis. Cada destino aparece como um cartão. Dependendo do destino, seu cartão pode exibir contas e ações configuradas para exibir informações adicionais.

![A guia Catálogo exibindo cartões de provedor de destino.](/help/assets/destinations/manage-destinations/destination-provider-catalog.png)

Localize o provedor de destino que você deseja configurar e selecione **[!UICONTROL Configurar]**.

A configuração de destino guiada é aberta e orienta você em quatro etapas: **[!UICONTROL Autenticar]**, **[!UICONTROL Criar destino]**, **[!UICONTROL Mapear campos]** e **[!UICONTROL Revisar]**.

### Autenticar {#authenticate}

A etapa **[!UICONTROL Autenticar]** estabelece uma conexão entre o Real-Time CDP Collaboration e a conta de destino.

Se uma conta existente estiver disponível, selecione-a no seletor de contas. Para criar uma conta, selecione **[!UICONTROL Nova conta]**.

Selecione um método de autenticação e forneça as informações de conta necessárias. Os métodos e campos de autenticação disponíveis dependem do provedor de destino selecionado. Para obter os requisitos específicos do conector, consulte [Requisitos do destino de armazenamento na nuvem](./cloud-storage-destination-requirements.md).

Selecione **[!UICONTROL Conectar ao Amazon S3]**. Para outros provedores de destino, o botão exibe o nome do provedor correspondente.

Depois que a conta for validada com êxito, selecione **[!UICONTROL Avançar]**.

![A etapa Autenticar, que mostra a seleção de conta e a criação de uma nova conta.](/help/assets/destinations/manage-destinations/authenticate-destination-account.png)

### Criar destino {#create-destination}

A etapa **[!UICONTROL Criar destino]** define onde e como os arquivos de exportação de público-alvo são entregues.

Insira um nome de destino e conclua as configurações de armazenamento e exportação necessárias. Os campos disponíveis dependem do provedor de destino selecionado. Para obter definições e requisitos específicos do conector, consulte a documentação de destino vinculada aos [requisitos de destino de armazenamento na nuvem](./cloud-storage-destination-requirements.md).

Após preencher todos os campos obrigatórios, selecione **[!UICONTROL Avançar]**. A configuração guiada avança para a etapa de mapeamento de campo.

![A etapa Criar destino exibindo campos de configuração de destino.](/help/assets/destinations/manage-destinations/configure-new-destination.png)

### Mapear campos {#map-fields}

A etapa **[!UICONTROL Mapear campos]** define como as chaves de correspondência de público-alvo são mapeadas para os campos de identidade esperados pelo destino.

Diferentemente do workflow padrão de destinos do Real-Time CDP, o Real-Time CDP Collaboration configura esses mapeamentos enquanto o destino é criado. As chaves de correspondência de público-alvo são exibidas como campos de origem. Mapeie cada campo de origem para a identidade de destino correspondente para que o destino possa reconhecer os identificadores exportados e associá-los aos usuários pretendidos.

Selecione **[!UICONTROL Adicionar campo]** para adicionar outro mapeamento de chave de correspondência ou selecione o ícone excluir para remover um mapeamento. Revise e configure todos os mapeamentos necessários.

Quando os mapeamentos estiverem concluídos, selecione **[!UICONTROL Avançar]**. A configuração guiada avança para a etapa de revisão.

![A etapa Mapear campos exibindo a configuração de mapeamento de chaves correspondente de ativação.](/help/assets/destinations/manage-destinations/map-destination-fields.png)

### Revisar {#review-destination}

A etapa **[!UICONTROL Revisar]** resume a configuração de destino antes de ela ser criada.

Revise as configurações de destino. Para fazer alterações, selecione o ícone de lápis ![O ícone de lápis.](../../assets/icons/edit.png) para a seção aplicável e atualize a configuração.

Quando a configuração estiver correta, selecione **[!UICONTROL Concluído]**. O destino é criado e fica disponível para ativação de público.

![A etapa Revisão exibindo o resumo da configuração de destino antes da conclusão.](/help/assets/destinations/manage-destinations/review-destination-configuration.png)

## Exibir destinos configurados {#view-configured-destinations}

Após configurar um destino, ele é exibido no inventário de destino. No inventário, é possível revisar o status e os públicos-alvo ativados para ele.

Navegue até **[!UICONTROL Ativação]** > **[!UICONTROL Destinos]**. A guia **[!UICONTROL Destinos]** exibe uma tabela de destinos configurados.

![A guia Destinos exibe os destinos configurados.](/help/assets/destinations/manage-destinations/configured-destinations-list.png)

## Excluir um destino {#delete-destination}

Exclua um destino quando ele não for mais necessário para a ativação de públicos-alvo. A exclusão de um destino o remove do inventário de destino e impede que os públicos-alvo sejam ativados para ele no futuro.

>[!IMPORTANT]
>
>A exclusão de um destino não remove os dados de público-alvo que foram exportados anteriormente para ele. Remova os dados exportados anteriormente diretamente do armazenamento de dados de destino.

Navegue até **[!UICONTROL Ativação]** > **[!UICONTROL Destinos]**.

Localize o destino que deseja remover, selecione o ícone de reticências na coluna **[!UICONTROL Ação]** e selecione **[!UICONTROL Excluir]**.

![A guia Destinos do espaço de trabalho Ativação com o ícone de reticências e a ação Excluir realçada.](/help/assets/destinations/manage-destinations/delete-configured-destination.png)

Uma caixa de diálogo de confirmação é exibida. Revise o destino que será removido e selecione **[!UICONTROL Excluir]** para confirmar.

O destino é removido do inventário de destino e não está mais disponível para ativação de público.

## Próximas etapas {#next-steps}

Após configurar um destino, você pode começar a [ativar públicos-alvo](../collaborate/activate.md) nos seus projetos.
