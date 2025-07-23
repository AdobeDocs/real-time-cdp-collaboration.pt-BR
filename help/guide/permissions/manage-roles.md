---
title: Gerenciar funções por meio de permissões
description: Entenda todos os recursos de função disponíveis que fornecem acesso a diferentes componentes na interface do Real-Time CDP Collaboration.
audience: admin
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# Gerenciar funções {#manage-roles}

{{limited-availability-release-note}}

Para gerenciar o acesso do usuário a diferentes componentes da interface do Adobe Real-Time CDP Collaboration, um [administrador](./manage-user-access.md#system-admin-gain-access) pode definir e atribuir funções. As funções definem o acesso que um administrador ou usuário tem a [recursos](https://experienceleague.adobe.com/pt-br/docs/experience-platform/access-control/home#permissions){target="_blank"} em sua organização. Este guia fornecerá informações sobre as funções padrão fornecidas no Real-Time CDP Collaboration, bem como as permissões individuais que você pode atribuir às funções personalizadas.

Para começar a gerenciar funções, um administrador precisará acessar o produto Experience Platform. Para obter informações sobre como obter acesso administrativo ou acesso ao Experience Platform, leia o guia [gerenciar acesso do usuário](./manage-user-access.md#manage-user-access-through-permissions).

## Funções padrão {#standard-roles}

Há duas funções padrão fornecidas que preenchem dois casos de uso comuns de controle de acesso. Essas são funções &quot;somente leitura&quot;, o que significa que não podem ser personalizadas.

| Nome da função | Descrição da função | Permissões |
| --- | --- | --- | 
| Gerentes da Collaboration | É uma permissão de acesso integral que contém todas as 15 permissões. Isso permite que o usuário leia, crie e edite todos os dados. Ele também fornece acesso à sandbox **[!UICONTROL Prod]** no Experience Platform, permitindo importar públicos para o Real-Time CDP Collaboration. | Tudo na tabela abaixo. |
| Visualizadores do Collaboration | Esta é uma permissão de acesso somente leitura. Um usuário pode ler e descobrir dados, atividades, conexões e muito mais. Ele também fornece acesso à sandbox **[!UICONTROL Prod]** no Experience Platform, permitindo importar públicos para o Real-Time CDP Collaboration. | Todas as permissões de leitura da tabela abaixo. |

{style="table-layout:auto"}

## Criar funções de acesso específicas {#specific-access-roles}

É provável que você queira criar funções adicionais para fornecer vários níveis de acesso a diferentes usuários. Ao criar funções, você pode gerenciar diferentes níveis de acesso selecionando permissões específicas no recurso **[!UICONTROL Colaborações]**. Para saber como criar e gerenciar funções, consulte o guia [funções](https://experienceleague.adobe.com/pt-br/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"}.

>[!NOTE]
> Para obter acesso ao Collaboration, um usuário deve ter acesso à sandbox **[!UICONTROL Prod]** no Adobe Experience Platform. Para conceder ao usuário acesso a esta sandbox, ele deve ser atribuído a uma função que contenha a permissão **[!UICONTROL Prod]** no recurso **[!UICONTROL Sandboxes]**.

Veja abaixo uma lista das permissões disponíveis no recurso Colaborações:

| Permissão de alto nível | Descrição |
| --- | --- |
| Gerenciar instâncias do Collaboration | Exibir, criar, atualizar e excluir as instâncias de colaboração de uma organização. Descubra as instâncias de colaboração de outras organizações. |
| Ler instâncias do Collaboration | Leia as instâncias de colaboração de uma organização e descubra as instâncias de colaboração de outras organizações. |
| Gerenciar convites de conexão | Exibir, criar e excluir convites de conexão iniciados por sua organização. Aceitar e recusar convite de conexão iniciado por outras organizações. |
| Ler convites de conexão | Exibir convites de conexão. |
| Gerenciar conexões do Collaboration | Um anunciante pode exibir, criar e atualizar configurações, bem como enviar e excluir conexões. Um editor pode exibir, aceitar ou recusar conexões. |
| Ler conexões do Collaboration | Exibir conexões. |
| Gerenciar dados de público-alvo | Integre e descubra públicos-alvo. Atualize públicos-alvo públicos, privados e personalizados e gerencie configurações de metadados do Audience Inventory. |
| Ler dados de público-alvo | Leia e descubra públicos-alvo. |
| Gerenciar dados de medição | Integrar, atualizar e excluir dados de medição. |
| Ler dados de medição | Ler dados de medição. |
| Gerenciar projetos | Exiba, crie, atualize e exclua projetos para qualquer uma das atividades de descoberta, ativação e medição. |
| Ler Projetos | Visualize projetos para qualquer uma das atividades de descoberta, ativação e medição. |
| Ler atividades do usuário | Leia as atividades do usuário. |
| Exportar atividades do usuário | Exportar atividades do usuário. |
| Ler Monitoramento de Crédito da Collaboration | Monitoramento de crédito no nível da organização e da instância. |

{style="table-layout:auto"}

## Próximas etapas

Depois de criar funções que definem o acesso ao Collaboration, será necessário [atribuir as funções](./manage-user-access.md#assign-a-role) a administradores e usuários. Consulte o guia [gerenciar permissões para uma função](https://experienceleague.adobe.com/pt-br/docs/experience-platform/access-control/abac/permissions-ui/permissions) para obter uma visão geral completa das funções de gerenciamento.
