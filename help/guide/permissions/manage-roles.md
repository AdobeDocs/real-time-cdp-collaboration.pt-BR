---
title: Gerenciar funções por meio de permissões
description: Entenda todos os recursos de função disponíveis que fornecem acesso a diferentes componentes na interface do Real-Time CDP Collaboration.
audience: admin
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
TQID: https://experienceleague.adobe.com/dB7nEQtEGG8PvCSE7eDDelH-ml2EhKOQ8ovvGXG1Ejg
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 623
ht-degree: 1%

---

# Gerenciar funções {#manage-roles}

{{limited-availability-release-note}}

Para gerenciar o acesso do usuário a diferentes componentes da interface do Adobe Real-Time CDP Collaboration, um [administrador](./manage-user-access.md#system-admin-gain-access) pode definir e atribuir funções. As funções definem o acesso que um administrador ou usuário tem a [recursos](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#permissions){target="_blank"} em sua organização. Este guia fornecerá informações sobre as funções padrão fornecidas no Real-Time CDP Collaboration, bem como as permissões individuais que você pode atribuir às funções personalizadas.

Para começar a gerenciar funções, um administrador precisará acessar o produto Experience Platform. Para obter informações sobre como obter acesso administrativo ou acesso ao Experience Platform, leia o guia [gerenciar acesso do usuário](./manage-user-access.md#manage-user-access-through-permissions).

## Funções padrão {#standard-roles}

Há duas funções padrão fornecidas que preenchem dois casos de uso comuns de controle de acesso. Essas são funções &quot;somente leitura&quot;, o que significa que não podem ser personalizadas.

| Nome da função | Descrição da função | Permissões |
| --- | --- | --- |
| Gerentes da Collaboration | É uma permissão de acesso integral que contém todas as 15 permissões. Isso permite que o usuário leia, crie e edite todos os dados. Ele também fornece acesso à sandbox **[!UICONTROL Prod]** no Experience Platform, permitindo importar públicos para o Real-Time CDP Collaboration. | Tudo na tabela abaixo. |
| Visualizadores do Collaboration | Esta é uma permissão de acesso somente leitura. Um usuário pode ler e descobrir dados, atividades, conexões e muito mais. Ele também fornece acesso à sandbox **[!UICONTROL Prod]** no Experience Platform, permitindo importar públicos para o Real-Time CDP Collaboration. | Todas as permissões de leitura da tabela abaixo. |

{style="table-layout:auto"}

## Criar funções de acesso específicas {#specific-access-roles}

É provável que você queira criar funções adicionais para fornecer vários níveis de acesso a diferentes usuários. Ao criar funções, você pode gerenciar diferentes níveis de acesso selecionando permissões específicas no recurso **[!UICONTROL Colaborações]**. Para saber como criar e gerenciar funções, consulte o guia [funções](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"}.

>[!NOTE]
> Para obter acesso ao Collaboration, um usuário deve ter acesso à sandbox **[!UICONTROL Prod]** no Adobe Experience Platform. Para conceder ao usuário acesso a esta sandbox, ele deve ser atribuído a uma função que contenha a permissão **[!UICONTROL Prod]** no recurso **[!UICONTROL Sandboxes]**.

Veja abaixo uma lista das permissões disponíveis no recurso Colaborações:

| Permissão de alto nível | Descrição |
| --- | --- |
| Gerenciar instâncias do Collaboration | Exibir, criar, atualizar e excluir as instâncias de colaboração de uma organização. Descubra as instâncias de colaboração de outras organizações. |
| Ler instâncias do Collaboration | Leia as instâncias de colaboração de uma organização e descubra as instâncias de colaboração de outras organizações. |
| Gerenciar convites de conexão | Exibir, criar e excluir convites de conexão iniciados por sua organização. Aceitar e recusar convite de conexão iniciado por outras organizações. |
| Ler convites de conexão | Exibir convites de conexão. |
| Gerenciar conexões do Collaboration | Um colaborador pode exibir, criar e atualizar configurações, bem como enviar e excluir conexões. |
| Ler conexões do Collaboration | Exibir conexões. |
| Gerenciar dados de público-alvo | Integre e descubra públicos-alvo. Atualize públicos-alvo públicos, privados e personalizados e gerencie configurações de metadados do Audience Inventory. |
| Read Audience Data | Read and discover audiences. |
| Manage Measurement Data | Onboard, update, and delete measurement data. |
| Read Measurement Data | Read measurement data. |
| Manage Projects | View, create, update, and delete projects for any of the discover, activate, and measurement activities. |
| Read Projects | View projects for any of the discover, activate, and measurement activities. |
| Read User Activities | Read user activities. |
| Export User Activities | Export user activities. |
| Read Collaboration Credit Monitoring | Credit monitoring at the organization and instance level. |

{style="table-layout:auto"}

## Próximas etapas

After creating roles that define access to Collaboration, you&#39;ll need to [assign the roles](./manage-user-access.md#assign-a-role) to administrators and users. Refer to the [manage permissions for a role](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions) guide for a complete overview of managing roles.
