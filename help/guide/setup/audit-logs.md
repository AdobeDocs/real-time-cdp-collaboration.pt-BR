---
title: Logs de auditoria
description: Saiba como usar a funcionalidade Logs de auditoria no Real-Time CDP Collaboration para rastrear atividades e alterações do usuário.
audience: admin
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: ff22dde9730fab89481338753b1dc4a0adf1d57e
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# Logs de auditoria

{{limited-availability-release-note}}

Para aumentar a transparência e a visibilidade das atividades realizadas no sistema, você pode auditar a atividade do usuário em vários serviços e recursos na forma de logs de auditoria no Adobe Real-Time Customer Data Platform (CDP). Esses registros formam uma trilha de auditoria que pode ajudar na solução de problemas no Real-Time CDP Collaboration e ajudar sua empresa a cumprir com as políticas corporativas de gerenciamento de dados e os requisitos normativos.

Basicamente, um log de auditoria informa *quem* executou a ação *o que* e *quando*. Cada ação registrada em um log contém metadados que indicam o tipo de ação, a data e a hora, a ID do email do usuário que executou a ação e atributos adicionais relevantes ao tipo de ação.

Use a funcionalidade de logs de auditoria no Real-Time CDP Collaboration para rastrear atividades e alterações do usuário na plataforma. Esse recurso é integrado ao serviço de auditoria da Adobe Experience Platform e a interface do usuário dessa funcionalidade reside no Experience Platform.

![Tela de visão geral de alto nível da funcionalidade de logs de auditoria](/help/assets/setup/audit-logs/audit-logs-overview.png)

Para obter informações mais abrangentes sobre logs de auditoria, consulte a [documentação de Logs de auditoria do Adobe Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Acessar logs de auditoria

Você pode acessar logs de auditoria de duas maneiras, conforme descrito nas seções abaixo. Ambas as opções exibem uma lista de logs de auditoria que capturam várias atividades executadas na interface do usuário do Real-Time CDP Collaboration

### Acessar logs de auditoria na interface do usuário do Real-Time CDP Collaboration

1. Navegue até a guia **[!UICONTROL Minha atividade]** na interface do Real-Time CDP Collaboration.
2. Selecione o link Experience Platform no texto da interface na parte superior da página.

![Acessar logs de auditoria da interface do Real-Time CDP Collaboration](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Acessar logs de auditoria diretamente na interface do usuário do Experience Platform

1. Navegue até a interface do usuário do Adobe Experience Platform e selecione a seção **[!UICONTROL Auditorias]** no menu à esquerda. Entre em contato com os administradores de sistema de sua organização para obter as permissões necessárias se não conseguir visualizar logs de auditoria.

![Acessar logs de auditoria da interface do Experience Platform](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Exibir e usar logs de auditoria

Para exibir os logs de auditoria:

1. Navegue até a seção **[!UICONTROL Auditorias]** na interface do Adobe Experience Platform.
2. Use os filtros para restringir os logs com base em seus critérios.
3. Selecione uma entrada de log para exibir informações detalhadas, incluindo o carimbo de data e hora, a ID da solicitação, os detalhes do recurso e o status da ação.

![Log de auditoria detalhado](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Atividades capturadas

Os logs de auditoria capturam informações detalhadas sobre as atividades do usuário, incluindo:

* **ID de Usuário**: o identificador do usuário que executou a ação.
* **Ação**: o tipo de ação executada (por exemplo, criar, atualizar, excluir).
* **Recurso**: o recurso modificado ou criado.
* **Carimbo de data/hora**: a hora em que a ação foi executada.

Esses registros criam uma trilha abrangente de todas as atividades na instância do Real-Time CDP Collaboration, o que é útil para o controle de dados e a conformidade normativa. Leia mais sobre [gerenciamento de logs de auditoria na interface](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Filtrar logs de auditoria

A interface dos logs de auditoria fornece vários filtros para ajudar você a pesquisar logs específicos:

* **Categoria**: refere-se ao tipo de recurso (por exemplo: instância de colaboração, conexão, projeto).
* **Ação**: o tipo de ação executada (por exemplo: criar, excluir, atualizar).
* **ID da Solicitação**: um identificador exclusivo para a solicitação.
* **Email de Usuário**: o endereço de email do usuário que executou a ação.
* **Status**: o status da ação (por exemplo: permitido, negado).
* **Intervalo de datas**: o intervalo de datas para o qual você deseja exibir logs.

Leia mais sobre [filtrando logs de auditoria](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

### Uso de exemplos

Os logs de auditoria são gerados e exibidos na interface de auditorias do Experience Platform quando você executa ações na interface do Real-Time CDP Collaboration, como gerenciar públicos, estender convites de conexão, criar projetos e assim por diante. Por exemplo, as operações para criar ou atualizar partes de um projeto são capturadas conforme mostrado abaixo:

![Exemplo de logs de auditoria gerados ao criar e atualizar partes de um projeto.](/help/assets/setup/audit-logs/create-project-audits.png)

## Benefícios

Entenda alguns dos benefícios de usar logs de auditoria:

* **Governança de dados**: use logs de auditoria para garantir que todas as atividades na plataforma sejam rastreadas e auditáveis.
* **Conformidade Normativa**: o recurso fornece uma trilha de atividades do usuário para atender aos requisitos normativos.
* **Solução de problemas**: os logs de auditoria ajudam a identificar e resolver problemas, fornecendo logs detalhados das ações do usuário.

## Referência de categorias e ações

A tabela abaixo fornece uma referência de todas as categorias e ações do Real-Time CDP Collaboration.

![Categorias disponíveis destacadas nos logs de auditoria do Real-Time CDP Collaboration.](/help/assets/setup/audit-logs/available-categories.png)

| Categoria | Ações | Descrição |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Instância do Collaboration]** | criar, atualizar, excluir | Gerenciar contas da organização, incluindo criação, atualização e exclusão de organizações. Leia mais sobre [configurando organizações](/help/guide/setup/onboard-organization.md). |
| **[!UICONTROL Convite para Conexão com o Collaboration]** | criar, atualizar, excluir, aprovar, rejeitar | Gerencie convites de conexão, incluindo criação, atualização, exclusão, aprovação e rejeição de convites. Leia mais sobre [convites de conexão](/help/guide/connect/establishing-connections.md). |
| **[!UICONTROL Conexão Collaboration]** | criar, atualizar, excluir, aprovar, rejeitar, solicitar aprovação | Gerencie conexões de colaboração, incluindo criação, atualização, exclusão, aprovação, rejeição e solicitação de aprovação para conexões. |
| **[!UICONTROL Conexão de dados do Collaboration]** | criar, atualizar, excluir | Gerencie conexões de dados para colaboração a fim de importar e gerenciar públicos, incluindo criação, atualização e exclusão de conexões de dados. Leia mais sobre [gerenciamento de conexões de dados](/help/guide/setup/manage-data-connection.md). |
| **[!UICONTROL Entidade de Dados do Collaboration]** | criar, atualizar, excluir | Gerencie entidades de dados para colaboração, incluindo criação, atualização e exclusão de entidades de dados. As entidades de dados neste contexto se referem aos públicos-alvo. Leia mais sobre [importação e gerenciamento de públicos](/help/guide/setup/onboard-audiences.md). |
| **[!UICONTROL Projeto do Collaboration]** | criar, atualizar, excluir | Gerencie projetos dentro da colaboração, incluindo criação, atualização e exclusão de projetos. Leia mais sobre [gerenciamento de projetos](/help/guide/collaborate/manage-projects.md). |
| **[!UICONTROL Módulo Collaboration]** | criar, atualizar, excluir | Gerencie diferentes módulos em projetos de colaboração, incluindo a criação, atualização e exclusão de vários módulos na interface do usuário. Por exemplo, a capacidade de [compartilhar públicos](/help/guide/collaborate/share.md). |

{style="table-layout:auto"}

Ao aproveitar a funcionalidade de logs de auditoria, é possível manter um registro claro e detalhado de todas as atividades na instância do Real-Time CDP Collaboration, garantindo transparência e responsabilidade.
