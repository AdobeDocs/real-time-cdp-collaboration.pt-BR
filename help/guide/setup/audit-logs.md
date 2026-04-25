---
title: Logs de auditoria
description: Learn how to use the Audit Logs functionality in Real-Time CDP Collaboration to track user activities and changes.
audience: admin
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
TQID: https://experienceleague.adobe.com/zb09-bUpxJ2VPDknETHeayMuLpNRCaQ2VTnV9QnTRgE
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 950
ht-degree: 1%

---

# Logs de auditoria

{{limited-availability-release-note}}

In order to increase the transparency and visibility of activities performed in the system, you can audit user activity for various services and capabilities in the form of audit logs in Adobe Experience Platform. These logs form an audit trail that can help with troubleshooting issues in Adobe Real-Time CDP Collaboration, and help your business effectively comply with corporate data stewardship policies and regulatory requirements.

In a basic sense, an audit log tells *who* performed *what* action, and *when*. Each action recorded in a log contains metadata that indicates the action type, date and time, the email ID of the user who performed the action, and additional attributes relevant to the action type.

Use the audit logs functionality in Collaboration to track user activities and changes within the platform. This feature is integrated with the Experience Platform audit service, and the UI for this functionality resides in Experience Platform.

![High-level overview screen of the audit logs functionality.](/help/assets/setup/audit-logs/audit-logs-overview.png)

For more comprehensive information about audit logs, visit the [Experience Platform audit logs documentation](https://experienceleague.adobe.com/pt-br/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Access audit logs

You can access audit logs in two ways, as described in the sections below. Both options display a list of audit logs capturing various activities performed within Collaboration.

### Access audit logs from the Collaboration user interface

1. Navigate to the **[!UICONTROL My Activity]** tab in **[!UICONTROL Setup]** workspace in Collaboration.
2. Select the Experience Platform link in the text at the top of the page.

![Access audit logs from the My activity tab in Collaboration.](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Access audit logs directly in the Experience Platform user interface

1. Navigate to [Experience Platform](https://platform.adobe.com/) and select the **[!UICONTROL Audits]** section from the left-hand menu. Reach out to your organization&#39;s system administrators to obtain the necessary permissions if you cannot view audit logs.

![Access audit logs from Experience Platform.](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Exibir e usar logs de auditoria

Para exibir os logs de auditoria:

1. Navegue até a seção **[!UICONTROL Auditorias]** no Experience Platform.
2. Use os [filtros](#filter-audit-logs) para restringir os logs com base em seus critérios.
3. Selecione uma entrada de log para exibir informações detalhadas, incluindo o carimbo de data e hora, a ID da solicitação, os detalhes do recurso e o status da ação.

![Log de auditoria detalhado](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Atividades capturadas

Os logs de auditoria capturam informações detalhadas sobre as atividades do usuário, incluindo:

* **Carimbo de data/hora**: a data e a hora exatas da ação executada no formato mês/dia/ano:minute AM/PM.
* **Nome do ativo**: o nome do recurso no qual a ação foi executada.
* **Categoria**: o tipo de recurso no qual a ação foi executada.
* **Ação**: a ação específica executada, como criar ou excluir.
* **Usuário**: o endereço de email do usuário que executou a ação.

Esses registros criam uma trilha abrangente de todas as atividades na instância do Collaboration, o que é útil para o controle de dados e a conformidade normativa. Leia mais sobre [gerenciamento de logs de auditoria na interface](https://experienceleague.adobe.com/pt-br/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Filtrar logs de auditoria {#filter-audit-logs}

A interface dos logs de auditoria fornece vários filtros para ajudar você a pesquisar logs específicos:

* **Categoria**: o tipo de recurso no qual a ação foi executada, como Instância do Collaboration ou Convite para Conexão do Collaboration.
* **Ação**: o tipo de ação executada. As ações disponíveis dependem da categoria selecionada. Por exemplo, as ações para a Instância do Collaboration incluem criar, atualizar e excluir.
* **ID da Solicitação**: um identificador exclusivo para a solicitação.
* **Usuário**: o endereço de email do usuário que executou a ação.
* **Status**: o status da ação, como permitir ou negar.
* **Intervalo de datas**: o intervalo de datas para o qual você deseja exibir logs.

Leia mais sobre [filtrando logs de auditoria](https://experienceleague.adobe.com/pt-br/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

## Benefícios

Os logs de auditoria oferecem vários benefícios para organizações que usam o Collaboration:

* **Governança de dados**: use logs de auditoria para garantir que todas as atividades na plataforma sejam rastreadas e auditáveis.
* **Conformidade Normativa**: o recurso fornece uma trilha de atividades do usuário para atender aos requisitos normativos.
* **Solução de problemas**: os logs de auditoria ajudam a identificar e resolver problemas, fornecendo logs detalhados das ações do usuário.

## Referência de categorias e ações

A tabela abaixo fornece uma referência de todas as categorias e ações do Real-Time CDP Collaboration.

![Categorias disponíveis destacadas nos logs de auditoria do Real-Time CDP Collaboration.](/help/assets/setup/audit-logs/available-categories.png)

| Categoria | Ações | Descrição |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Instância do Collaboration]** | criar, atualizar, excluir | Gerenciar contas, inclusive criar, atualizar e excluir contas. Para saber mais, leia o [guia de configuração de contas](/help/guide/setup/onboard-account.md). |
| **[!UICONTROL Convite para Conexão com o Collaboration]** | criar, atualizar, excluir, aprovar, rejeitar | Gerencie convites de conexão, incluindo criação, atualização, exclusão, aprovação e rejeição de convites. Para obter mais informações, leia o guia [estabelecendo conexões](/help/guide/connect/establishing-connections.md). |
| **[!UICONTROL Conexão Collaboration]** | criar, atualizar, excluir, aprovar, rejeitar, solicitar aprovação | Gerenciar conexões, incluindo criação, atualização, exclusão, aprovação, rejeição e solicitação de aprovação para conexões. |
| **[!UICONTROL Conexão de dados do Collaboration]** | criar, atualizar, excluir | Gerencie as conexões de dados de onde você origina e gerencia públicos, incluindo criação, atualização e exclusão de conexões de dados. Para obter mais informações, leia o guia [gerenciamento de conexões de dados](/help/guide/setup/manage-data-connection.md). |
| **[!UICONTROL Entidade de Dados do Collaboration]** | criar, atualizar, excluir | Manage data entities for Collaboration, including creating, updating, and deleting data entities. Data entities in this context refers to audiences. For more information, read the [sourcing and managing audiences](/help/guide/setup/onboard-audiences.md) guide. |
| **[!UICONTROL Collaboration Project]** | create, update, delete | Manage projects within Collaboration, including creating, updating, and deleting projects. For more information, read the [managing projects](/help/guide/collaborate/manage-projects.md) guide. |
| **[!UICONTROL Collaboration Module]** | create, update, delete | Manage different modules within projects, including creating, updating, and deleting various modules in the UI. For example, the ability to [activate audiences](/help/guide/collaborate/activate.md). |

{style="table-layout:auto"}

By leveraging the audit logs functionality, you can maintain a clear and detailed record of all activities within Collaboration, ensuring transparency and accountability.
