---
title: Visão geral do controle de acesso
description: Saiba como obter acesso ao Adobe Real-Time Customer Data Platform (CDP) Collaboration.
audience: admin
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: af48f5ea-8258-42a6-a39e-f4a4ca5b4a69
source-git-commit: 1f825bb4a81dbf65c43ddadcfd444923a37a906e
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 2%

---

# Visão geral do controle de acesso

{{limited-availability-release-note}}

>[!IMPORTANT]
>
> Se você for um usuário final que deseja acessar o Adobe Real-Time CDP Collaboration, entre em contato com o administrador do sistema ou do produto para verificar o acesso existente. Caso não saiba quem é o administrador do sistema, entre em contato com o representante da Adobe.

O controle de acesso do Adobe Real-Time CDP Collaboration é fornecido por meio da Admin Console e de permissões no [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}. Neste guia, você aprenderá a conceder acesso a si mesmo ou a outros membros de sua equipe, dependendo do caso de uso.

## Hierarquia de controle de acesso {#hierarchy}

Para configurar o controle de acesso ao Collaboration, você **deve** ter privilégios de administrador do sistema ou do produto. Um administrador do sistema não tem restrições e é provisionado durante o processo de integração. Enquanto isso, um administrador de produto pode fornecer funções administrativas para todos os produtos aos quais foram atribuídos. Um administrador de produto deve receber acesso administrativo e de produto por um administrador do sistema.

Esses guias descreverão a configuração do acesso para administradores de sistema, administradores de produtos e usuários finais. Consulte a tabela abaixo para entender a principal diferença entre as funções.

| Função | Descrição |
| --- | --- |
| Administrador do sistema | O superusuário da organização. Eles podem executar todas as tarefas administrativas no Admin Console e têm permissões para delegar funções administrativas a outros usuários. |
| Administrador do produto | Administra os produtos atribuídos a eles e todas as funções administrativas associadas, como adicionar usuários a organizações, adicionar ou remover usuários de perfis de produtos e adicionar ou remover outros administradores de produtos de um produto. |
| Usuário final | Os usuários em sua organização que usam os produtos. |

{style="table-layout:auto"}

Para obter mais informações sobre funções administrativas, visite a [Central de Ajuda da Adobe](https://helpx.adobe.com/br/enterprise/using/admin-roles.html).

>[!TIP]
>
>O uso de **administradores** nesses guias se referirá a **administradores do sistema e do produto**.

## Produtos adicionais {#products}

Antes de conceder acesso ao Collaboration, você precisará acessar vários produtos, dependendo do seu [caso de uso](#use-cases). Os guias de controle de acesso podem funcionar por meio de várias interfaces de usuário à medida que você avança, cada uma servindo a um propósito específico no processo de configuração de acesso. Consulte a tabela abaixo para obter uma compreensão mais profunda de para que cada produto será usado.

| Produto | Usos |
| --- | --- |
| [Admin Console](https://adminconsole.adobe.com/) | Os administradores usam isso para atribuir aos usuários acesso de produto e/ou administrador. |
| [Permissões](https://experience.adobe.com/) | Os administradores usam isso para atribuir funções de administradores ou usuários finais. |
| [Experience Platform](https://platform.adobe.com/) | Administradores e usuários finais precisam receber acesso ao produto Experience Platform para atribuí-los a funções. |

## Onde começar {#use-cases}

Agora que você tem uma compreensão mais profunda das funções de usuário e administrativas, bem como dos diferentes produtos da Experience Cloud, pode começar a conceder acesso ao Collaboration. Há dois fatores principais que influenciam as etapas que você precisará seguir:

- se estiver atribuindo acesso de administrador ou usuário final
- se os usuários já tiverem acesso ao produto Experience Platform

Consulte o gráfico abaixo para determinar quem é necessário para configurar os privilégios e onde começar com base no seu caso de uso de controle de acesso. **Siga o tutorial até o final do guia, do seu ponto de partida.**

>[!TIP]
>
> Um superusuário se refere ao mais alto nível de acesso a ser obtido pelo administrador do sistema. Um superusuário pode executar todas as tarefas administrativas e a funcionalidade do usuário. Um administrador do sistema não tem funcionalidade de produto pronta para uso e precisa conceder a si mesmo o acesso apropriado, conforme mostrado no gráfico abaixo.

| Caso de uso | Função necessária | Onde começar |
| --- | --- | --- |
| Superusuário sem acesso existente ao produto Experience Platform. | Um administrador do sistema. | [Configurar acesso de administrador de produto](./manage-user-access.md#admin-access) |
| Superusuário para um administrador de sistema do Experience Platform existente **com acesso à interface do usuário do Experience Platform**. | Um administrador do sistema. | [Configurar o acesso ao Collaboration](./manage-user-access.md#RTCDP-collab-access) |
| Superusuário para um administrador de sistema do Experience Platform existente **sem** acesso à interface do usuário do Experience Platform. | Um administrador do sistema. | [Configurar acesso de administrador de produto](./manage-user-access.md#admin-access) |
| Privilégios de administrador de produto e acesso ao Collaboration para um novo administrador de produto. | Um administrador do sistema. | [Configurar acesso de administrador de produto](./manage-user-access.md#admin-access) |
| Acesso ao Collaboration para um administrador de produto existente do Experience Platform **com acesso à interface do usuário do Experience Platform**. | Um administrador de sistema ou de produto. | [Configurar o acesso ao Collaboration](./manage-user-access.md#RTCDP-collab-access) |
| Acesso ao Collaboration para um administrador de produto existente do Experience Platform **sem** acesso à interface do usuário do Experience Platform. | Um administrador de sistema ou de produto. | [Configurar acesso do usuário](./manage-user-access.md#user-access) |
| Acesso ao Collaboration para um novo usuário final. | Um administrador de sistema ou de produto. | [Configurar acesso do usuário](./manage-user-access.md#user-access) |
| Acesso ao Collaboration para um usuário existente com acesso ao Experience Platform. | Um administrador de sistema ou de produto. | [Configurar o acesso ao Collaboration](./manage-user-access.md#RTCDP-collab-access) |

{style="table-layout:auto"}

## Permissões adicionais

Depois de obter acesso ao Collaboration, talvez você precise de algumas permissões adicionais do Experience Platform para obter funcionalidades específicas.

### Audience sourcing {#audience-sourcing}

Antes de começar a enviar públicos-alvo para colaboradores, é necessário fornecer públicos-alvo para a Collaboration. Atualmente, a única conexão de dados de autoatendimento compatível com a importação de públicos é o Experience Platform. Para começar, os usuários que gerenciam a integração de público-alvo precisarão receber uma função com as seguintes permissões de recurso de **[!UICONTROL Gerenciamento de perfil]**:

| Permissão | Descrição |
| ---- | ---- |
| [!UICONTROL Exibir Segmentos] | Permite que o usuário veja a lista de públicos-alvo disponíveis em uma sandbox. |
| [!UICONTROL Exibir Perfis] | Permite que o usuário veja os campos disponíveis para mapeamento para campos de colaboração. |

Abaixo, você pode ver um exemplo de função com as permissões acima adicionadas. Para obter mais informações sobre como criar ou atribuir funções, consulte o guia [gerenciar funções](./manage-roles.md).

![O espaço de trabalho de recursos em Permissões com as permissões Exibir Segmentos e Exibir Perfis adicionadas ao recurso Gerenciamento de Perfil.](../../assets/permissions/sample-audience-role.png)

>[!NOTE]
>
>Os usuários podem trabalhar com públicos-alvo no Collaboration após serem adquiridos sem as permissões acima.

## Próximas etapas

Depois de determinar por onde começar, siga o link do caso de uso para começar a configurar o acesso. Se quiser saber mais sobre como configurar o acesso ao Collaboration como administrador, além desses casos de uso, consulte o guia [gerenciar acesso de usuário](manage-user-access.md). Para saber mais sobre as funções e sua parte na configuração do acesso a vários componentes do Collaboration, consulte o guia [gerenciar funções](manage-roles.md).
