---
title: Notas de versão mais recentes do Real-Time CDP Collaboration
description: Seguir as versões mais recentes do Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
TQID: https://experienceleague.adobe.com/re4oFblCLiZpspWIS7D4EEYNh36EDhULEOd2-ccXH28
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1461
ht-degree: 2%

---

# Notas de versão mais recentes do Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Última atualização**: janeiro de 2026.

Essas notas de versão abordam a funcionalidade lançada no Adobe Real-Time CDP Collaboration. As versões do Collaboration operam em um modelo de entrega contínua, que permite uma cadência de lançamento mensal aproximada. Essas notas de versão são atualizadas com frequência. Portanto, verifique-as regularmente.

## Janeiro de 2026 {#january-2026}

O Real-Time CDP Collaboration agora é compatível com o upload de arquivos CSV como um novo método para fornecer públicos-alvo, bem como novas chaves de correspondência móvel (IDFA e GAID) para melhorar a correspondência e a medição de públicos-alvo.

**Recursos novos ou atualizados**

| Recurso | Descrição |
| ------- | ----------- |
| Upload de CSV para origem de público-alvo | Faça upload de arquivos CSV para públicos-alvo de origem na Collaboration diretamente da interface do usuário. Ideal para a integração de dados primários para projetos de colaboração de curto prazo. Para obter mais informações, consulte o [guia de fornecimento de carregamento de arquivo CSV para público-alvo](../setup/upload-csv-audience-sourcing.md). |
| Suporte à chave de correspondência móvel | O Collaboration agora é compatível com chaves de correspondência móvel, incluindo IDFA e GAID, para correspondência e medição de público-alvo. Essas chaves de correspondência são selecionadas durante a configuração da conta e podem ser usadas ao definir configurações de conexão para novas conexões e em workflows de colaboração downstream. Consulte o [Guia de configuração de chaves de correspondência](../setup/onboard-account.md#set-up-match-keys) para obter mais detalhes. |

{style="table-layout:auto"}

## Dezembro de 2025 {#december-2025}

O Real-Time CDP Collaboration agora está disponível para clientes na **Europa, Oriente Médio e África (EMEA)**. Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate nessas regiões.

## Agosto de 2025 {#august-2025}

O Real-Time CDP Collaboration agora está disponível para clientes no **Canadá**. Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate nessas regiões.

* O Collaboration agora oferece suporte às [chaves de correspondência](../setup/onboard-account.md#supported-match-keys) a seguir:
   * Email com hash
   * Número de telefone com hash
   * ID do CRM
   * ID de fidelidade
   * IPv4 com hash
   * ID do AdFixus
* Agora há várias chaves de correspondência disponíveis no Collaboration, o que permite expandir o tamanho do público e melhorar as taxas de correspondência. Várias chaves de correspondência podem ser usadas ao fornecer públicos, estabelecer conexões e ativar públicos. Para saber mais sobre como usar várias chaves de correspondência, leia os [guias Configurar chaves de correspondência](../setup/onboard-account.md) e [públicos-alvo de origem](../setup/onboard-audiences.md#map-fields).

>[!IMPORTANT]
>
>Ao ativar públicos-alvo em que várias chaves de correspondência são usadas, se uma (ou mais) chave de correspondência não tiver sobreposições, contagem de público-alvo ou ficar abaixo do limite, toda a ativação falhará. Verifique se os públicos-alvo têm sobreposição suficiente e se atendem ao limite mínimo de 1000 IDs em todas as chaves de correspondência antes da ativação.

* O destino do Adobe Experience Platform agora é compatível com a ativação de públicos-alvo com várias chaves de correspondência. Além disso, agora você pode usar uma chave vinculada ao configurar o mapeamento do destino para especificar qual chave de correspondência é enviada durante a ativação. Para saber mais, leia o [guia de destino do Experience Platform](../destinations/experience-platform.md#linked-keys).
* Agora os colaboradores podem editar vários públicos-alvo de uma só vez. Agora você pode editar metadados de público-alvo, acesso à conexão, nomes, descrições e categorias para vários públicos-alvo usando a ferramenta de edição em massa. Para saber mais sobre edição de públicos, leia o guia [gerenciar públicos-alvo](../setup/onboard-audiences.md#edit-audiences).

## Julho de 2025 {#july-2025}

A Real-time CDP Collaboration agora oferece suporte à colaboração de marca para marca. Os colaboradores agora podem formar conexões, independentemente de serem um anunciante ou editor. Isso permite oportunidades de colaboração mais flexíveis e permite que as marcas aproveitem os dados e insights umas das outras. Para saber mais sobre as diferenças entre a colaboração de marca para marca e de anunciante para editor, leia o guia [padrões de colaboração](../overview/collaboration-patterns.md).

* Os colaboradores agora podem se conectar usando [convites para conexão privada](../connect/establishing-connections.md#private-connection-invites). Compartilhe o código de conexão exclusivo de sua conta com um colaborador que pode usá-lo para se conectar diretamente com você. Este é um recurso principal da colaboração de marca para marca, permitindo que os colaboradores estabeleçam conexões além dos anunciantes que exploram o diretório **[!UICONTROL Descobrir colaboradores]**.
* [Destinos de autoatendimento](../setup/manage-destinations.md) agora estão disponíveis para anunciantes e editores.
* A ativação de público agora está disponível para ambos os colaboradores em uma conexão, independentemente de sua [função de conta](../overview/roles.md). As configurações de ativação de público-alvo são definidas ao [estabelecer conexões](../connect/establishing-connections.md#configure-connection-settings), permitindo que você especifique qual colaborador pode ativar públicos-alvo. Para saber mais sobre a ativação de público, leia o guia [ativar públicos-alvo](../collaborate/activate.md).
* O caso de uso **[!UICONTROL Ativar]** foi reconfigurado para oferecer suporte à colaboração de marca para marca. A guia **[!UICONTROL Ativar]** em um projeto agora exibe os públicos que foram enviados para o colaborador e os públicos que foram ativados para o destino pelo colaborador. Para saber mais, leia o guia [ativar públicos-alvo](../collaborate/activate.md). <br> ![The Activate dashboard with the Audiences sent to and Audiences activated sections.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* Audience index scores are now available in the **[!UICONTROL Discover]** tab of a project. The audience index score is a measure of how well an audience matches your collaborator&#39;s audience. This score is calculated based on on underlying audience counts &amp; overlaps. To learn more about audience index scores, read the [audience index score](../collaborate/discover.md#audience-index-score) guide.

## Maio de 2025 {#may-2025}

* Real-Time CDP Collaboration is now available to customers in **Australia** and **New Zealand**. Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate nessas regiões.
* Real-Time CDP Collaboration now offers [self-serve destinations](../setup/manage-destinations.md) through the **[!UICONTROL My destinations]** tab in the **[!UICONTROL Setup]** section. Destinations allow you to activate audiences in third-party platforms, such as advertising networks or data management platforms, to reach your customers across various channels. Currently, only Adobe Experience Platform destinations are supported. Se você estiver interessado em configurar um destino diferente, entre em contato com o representante da Adobe. To learn more about destinations, read the [destinations overview](../destinations/overview.md) guide.
   * Destinations also adds support to view Collaboration audiences in the [Adobe Experience Platform audience portal](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* You can now edit the audience refresh frequency for existing data connections in Collaboration. Currently, you can choose to refresh your audiences daily or every two to six days. To learn more about how to edit the audience refresh frequency, read the [manage data connections](../setup/manage-data-connection.md#scheduling) guide.
* Credit splits between collaborators are now set for each use case selected within the connection. You can set different credit consumption rules for each use case to better control how your credits are used. To learn more about about the credit split funtionality, read the [connection settings](../connect/establishing-connections.md#connection-settings) guide. To learn more about how credits are consumed, read the [credit activity types](../setup/my-activity.md#types-of-activities) guide. <br> ![Connection settings screen showing the credit split functionality.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Publishers can now set advertiser names and IDs before accepting the connection settings from an advertiser. Publishers can set names and IDs that align with their internal systems, which can be different from the advertiser&#39;s names and IDs. To learn more about adding advertiser names and IDs, read the [connection settings](../connect/establishing-connections.md#connection-settings.md) guide. <br> ![Connection settings screen showing the publisher setting advertiser names and IDs.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## Abril de 2025 {#april-2025}

* Uma nova coluna **[!UICONTROL Entradas Processadas]** foi adicionada à tabela de atividade de consumo de crédito. Essa coluna exibe o número total de entradas (por exemplo, IDs ou linhas) processadas para cada atividade. [Leia mais](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Coluna processada de entradas realçada na exibição Minha atividade.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Uma nova opção de email de contato foi adicionada à criação da conta. Isso ajuda os colaboradores do parceiro a contatarem você, conforme necessário, durante o processo de conexão. [Leia mais](../setup/onboard-account.md).

## Março de 2025 {#march-2025}

* Ao [fornecer públicos-alvo](/help/guide/setup/onboard-audiences.md) para o Collaboration, agora é possível definir uma frequência de atualização de público-alvo de **a cada um a seis dias** para gerenciar melhor a [atividade de crédito de Gerenciamento de público-alvo](/help/guide/setup/my-activity.md#types-of-activities). Para obter mais informações, leia o guia [gerenciar públicos-alvo](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences). <br> ![A tela Agendar mostra intervalos de frequência diferentes para atualizar a associação de público-alvo.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Tela de agendamento mostrando intervalos de frequência diferentes para atualizar associação de público-alvo."){width="250" align="center" zoomable="yes"}
* Ao estabelecer uma conexão com um colaborador, agora é possível selecionar **casos de uso** predefinidos. O caso de uso selecionado determina quais seções do projeto e funcionalidades do produto ficam disponíveis. Para obter mais informações, leia o guia [gerenciar projetos](/help/guide/collaborate/manage-projects.md#project-use-cases).
   * *A medição* habilita a seção de projeto **Medida**.
   * A *descoberta de público-alvo* habilita a seção de projeto **Descoberta**.
   * *A ativação de público* habilita as **Ativar** seções de projeto <br>
* Agora você pode excluir conexões com colaboradores com os quais não deseja mais trabalhar. Para saber como excluir conexões, leia o guia [excluindo conexões](/help/guide/connect/establishing-connections.md#delete-connections).

## Fevereiro de 2025 {#february-2025}

O Adobe Real-Time CDP Collaboration, criado especificamente para permitir que anunciantes e editores descubram, ativem e meçam públicos-alvo de alto valor sem cookies de terceiros, agora está disponível de modo geral nos Estados Unidos.

### Introdução

1. **Configuração do Access**: os administradores do sistema configuram permissões de acesso para usuários. Para saber mais sobre como configurar permissões de acesso, leia o [guia de gerenciamento de acesso do usuário](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access).
2. **Conectar-se às Fontes de Dados**: públicos-alvo da Source a serem usados na Collaboration. Para começar a fornecer públicos-alvo, leia o guia [fonte e gerenciar públicos-alvo](/help/guide/setup/onboard-audiences.md).
3. **Estabelecer Conexões**: comece a colaborar com anunciantes ou editores confiáveis. Para saber mais sobre como formar conexões, leia o guia [estabelecendo conexões](/help/guide/connect/establishing-connections.md).
4. **Descobrir e ativar**: crie projetos para identificar públicos-alvo valiosos a serem ativados em campanhas. Para saber mais sobre como criar projetos, leia o guia [gerenciar projetos](/help/guide/collaborate/manage-projects.md).

### Disponibilidade

* No momento, o Adobe Real-Time CDP Collaboration está disponível somente para clientes dos EUA.
* Ele fica disponível automaticamente para clientes do Adobe Real-Time CDP Prime e do Ultimate

Para obter mais informações, leia:

* [Visão geral do Collaboration](/help/guide/home.md)
* [Fluxo de trabalho de ponta a ponta](/help/guide/overview/end-to-end-workflow.md)
* [Visão geral de permissões](/help/guide/permissions/overview.md)
