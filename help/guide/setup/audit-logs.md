---
title: Logs de auditoria
description: Saiba como usar a funcionalidade Logs de auditoria no Real-Time CDP Collaboration para rastrear atividades e alterações do usuário.
audience: admin
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Logs de auditoria

{{limited-availability-release-note}}

Para aumentar a transparência e a visibilidade das atividades realizadas no sistema, você pode auditar a atividade do usuário em vários serviços e recursos na forma de logs de auditoria no Adobe Experience Platform. Esses registros formam uma trilha de auditoria que pode ajudar na solução de problemas no Adobe Real-Time CDP Collaboration e ajudar sua empresa a cumprir com as políticas corporativas de gerenciamento de dados e os requisitos normativos.

Basicamente, um log de auditoria informa *quem* executou a ação *o que* e *quando*. Cada ação registrada em um log contém metadados que indicam o tipo de ação, a data e a hora, a ID do email do usuário que executou a ação e atributos adicionais relevantes ao tipo de ação.

Use a funcionalidade de logs de auditoria no Collaboration para rastrear atividades e alterações do usuário na plataforma. Esse recurso é integrado ao serviço de auditoria da Experience Platform e a interface do usuário dessa funcionalidade reside no Experience Platform.

![Tela de visão geral de alto nível da funcionalidade de logs de auditoria.](/help/assets/setup/audit-logs/audit-logs-overview.png)

Para obter informações mais abrangentes sobre logs de auditoria, consulte a [documentação sobre logs de auditoria da Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Acessar logs de auditoria

Você pode acessar logs de auditoria de duas maneiras, conforme descrito nas seções abaixo. Ambas as opções exibem uma lista de logs de auditoria que capturam várias atividades realizadas no Collaboration.

### Acessar logs de auditoria na interface do usuário do Collaboration

1. Navegue até a guia **[!UICONTROL Minha Atividade]** no espaço de trabalho **[!UICONTROL Configuração]** do Collaboration.
2. Selecione o link Experience Platform no texto na parte superior da página.

![Acesse logs de auditoria na guia Minha atividade no Collaboration.](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Acessar logs de auditoria diretamente na interface do usuário do Experience Platform

1. Navegue até [Experience Platform](https://platform.adobe.com/) e selecione a seção **[!UICONTROL Auditorias]** no menu à esquerda. Entre em contato com os administradores de sistema de sua organização para obter as permissões necessárias se não conseguir visualizar logs de auditoria.

![Acessar logs de auditoria do Experience Platform.](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

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

Esses registros criam uma trilha abrangente de todas as atividades na instância do Collaboration, o que é útil para o controle de dados e a conformidade normativa. Leia mais sobre [gerenciamento de logs de auditoria na interface](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Filtrar logs de auditoria {#filter-audit-logs}

A interface dos logs de auditoria fornece vários filtros para ajudar você a pesquisar logs específicos:

* **Categoria**: o tipo de recurso no qual a ação foi executada, como Instância do Collaboration ou Convite para Conexão do Collaboration.
* **Ação**: o tipo de ação executada. As ações disponíveis dependem da categoria selecionada. Por exemplo, as ações para a Instância do Collaboration incluem criar, atualizar e excluir.
* **ID da Solicitação**: um identificador exclusivo para a solicitação.
* **Usuário**: o endereço de email do usuário que executou a ação.
* **Status**: o status da ação, como permitir ou negar.
* **Intervalo de datas**: o intervalo de datas para o qual você deseja exibir logs.

Leia mais sobre [filtrando logs de auditoria](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

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
| **[!UICONTROL Entidade de Dados do Collaboration]** | criar, atualizar, excluir | Gerencie entidades de dados para o Collaboration, incluindo criação, atualização e exclusão de entidades de dados. As entidades de dados neste contexto se referem aos públicos-alvo. Para obter mais informações, leia o [guia de fornecimento e gerenciamento de públicos-alvo](/help/guide/setup/onboard-audiences.md). |
| **[!UICONTROL Projeto do Collaboration]** | criar, atualizar, excluir | Gerenciar projetos no Collaboration, incluindo criação, atualização e exclusão de projetos. Para obter mais informações, leia o guia [gerenciamento de projetos](/help/guide/collaborate/manage-projects.md). |
| **[!UICONTROL Módulo Collaboration]** | criar, atualizar, excluir | Gerencie diferentes módulos em projetos, incluindo a criação, atualização e exclusão de vários módulos na interface do usuário. Por exemplo, a capacidade de [ativar públicos-alvo](/help/guide/collaborate/activate.md). |

{style="table-layout:auto"}

Ao aproveitar a funcionalidade de logs de auditoria, você pode manter um registro claro e detalhado de todas as atividades no Collaboration, garantindo a transparência e a responsabilidade.
