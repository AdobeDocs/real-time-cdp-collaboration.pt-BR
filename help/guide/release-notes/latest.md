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
source-git-commit: 7affd3abf7a10019503825cb20d9be1ad4000603
workflow-type: tm+mt
source-wordcount: 1903
ht-degree: 3%

---

# Notas de versão mais recentes do Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Última atualização**: abril de 2026.

Essas notas de versão abordam a funcionalidade lançada no Adobe Real-Time CDP Collaboration. As versões do Collaboration operam em um modelo de entrega contínua, que permite uma cadência de lançamento mensal aproximada. Essas notas de versão são atualizadas com frequência. Portanto, verifique-as regularmente.

## Abril de 2026 {#april-2026}

Agora novos recursos estão disponíveis no Real-Time CDP Collaboration. Isso inclui o Collaboration [!DNL Starter] para convidar parceiros, a fonte de público ampliada de [!DNL Snowflake] e [!DNL Google Cloud Storage], o suporte para [!DNL Demdex ID (ECID)] como chave de correspondência e duas novas funções de colaborador: Agência e Parceiro de dados.

**Recursos novos ou atualizados**

| Recurso | Descrição |
| ------- | ----------- |
| Real-Time CDP Collaboration [!DNL Starter] | Agora você pode convidar parceiros que não têm uma licença da Collaboration para colaborar com você por meio do Collaboration [!DNL Starter]. Os parceiros convidados podem fornecer públicos-alvo, descobrir sobreposições e ativar públicos-alvo na conexão compartilhada. Consulte a [visão geral [!DNL Starter] do Collaboration](../overview/starter-overview.md) para começar. |
| Fornecimento de público de autoatendimento de [!DNL Snowflake] e [!DNL Google Cloud Storage] | Agora você pode originar públicos originais diretamente do seu bucket do [!DNL Snowflake Secure Data Share] ou do [!DNL Google Cloud Storage] para o Collaboration. Para obter instruções de configuração, consulte os guias a seguir: <ul><li>[Configurar [!DNL Snowflake] para fornecimento de público-alvo](../setup/configure-snowflake-audience-sourcing.md) </li><li> [Configurar [!DNL Google Cloud Storage] para fornecimento de público-alvo](../setup/configure-gcs-audience-sourcing.md) </li></ul> |
| [!DNL Demdex ID] chave correspondente | Agora há suporte para [!DNL Demdex ID] (ECID) como uma chave de correspondência para identidades anônimas baseadas em cookies entre plataformas. Isso melhora a precisão da sobreposição de público-alvo sem depender de dados de usuários autenticados. Consulte [chaves de correspondência com suporte](../setup/onboard-account.md#supported-match-keys) para obter detalhes. |
| Novas funções de colaborador | A Collaboration agora oferece suporte a duas funções adicionais de colaborador, incluindo **Agência** e **Parceiro de dados**. Essas funções expandem como organizações diferentes podem participar e trabalhar juntas na plataforma. Saiba mais sobre: <ul><li>[Funções de conta do colaborador](../overview/roles.md)</li><li>[Padrões do Collaboration](../overview/collaboration-patterns.md)</li><li>[Fluxo de trabalho de ponta a ponta](../overview/end-to-end-workflow.md)</li></ul> |

{style="table-layout:auto"}

## Março de 2026 {#march-2026}

Agora é possível gerar relatórios de medição de campanha e gerenciar dados de medição no Real-Time CDP Collaboration.

**Recursos novos ou atualizados**

| Recurso | Descrição |
| ------- | ----------- |
| Disponibilidade geral de medição | Os relatórios de medição agora estão disponíveis no Collaboration. Agora você pode inserir IDs de campanha associadas a campanhas de marketing como editor, originar dados de conversão como anunciante e gerar dois tipos de relatórios: **Resumo da campanha** para resultados gerais da campanha e **Atribuição** para insights de eficácia da campanha. Para começar, consulte os guias a seguir: <ul><li>[IDs da campanha de entrada](../collaborate/manage-projects.md#manage-campaign-id)</li><li>[dados de conversão do Source](../setup/onboard-measurement-data.md)</li><li>[Criar e exibir relatórios de medição](../collaborate/measure.md)</li></ul> |
| Gerenciamento do ciclo de vida de medição | O Collaboration também oferece suporte ao gerenciamento de medição:<ul><li> Agora os anunciantes podem editar ou excluir conexões de dados de medição e eventos de conversão associados para garantir uma análise de campanha precisa e atualizada. Para obter mais detalhes, consulte [Gerenciar conexão de dados de medição](../setup/manage-measurement-data-connection.md) e [Gerenciar eventos de conversão](../setup/onboard-measurement-data.md#edit-measurement-data).</li><li>Você também pode editar ou excluir relatórios de medição agendados diretamente da guia **[!UICONTROL Medida]** em qualquer projeto de colaboração. Isso está disponível para todos os usuários. Consulte o [guia de gerenciamento de relatórios de medição](../collaborate/measure.md) para obter mais detalhes.</li></ul> |

{style="table-layout:auto"}

## Fevereiro de 2026 {#february-2026}

O Real-Time CDP Collaboration agora oferece suporte à edição de configurações de conexão de dados e conexão existentes diretamente na interface.

**Recurso novo ou atualizado**

| Recurso | Descrição |
| ------- | ----------- |
| Editar configurações de conexão | Agora, os proprietários de uma conexão podem atualizar casos de uso, chaves de correspondência, permissões de ativação e divisões de crédito após o estabelecimento de uma conexão. Consulte [Editar conexão](../connect/manage-connections.md#edit-connection) para obter instruções passo a passo. |
| Editar conexões de dados | Atualize as chaves de correspondência e as configurações de agendamento para suas conexões de dados existentes diretamente no Collaboration. Consulte [Editar conexão de dados](../setup/manage-data-connection.md#edit-data-connection) para obter instruções passo a passo. |

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
* O caso de uso **[!UICONTROL Ativar]** foi reconfigurado para oferecer suporte à colaboração de marca para marca. A guia **[!UICONTROL Ativar]** em um projeto agora exibe os públicos que foram enviados para o colaborador e os públicos que foram ativados para o destino pelo colaborador. Para saber mais, leia o guia [ativar públicos-alvo](../collaborate/activate.md). <br> ![O painel Ativar com as seções Públicos-alvo enviados para e Públicos-alvo ativadas.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* As pontuações do índice de público-alvo agora estão disponíveis na guia **[!UICONTROL Descubra]** de um projeto. A pontuação do índice de público-alvo é uma medida do desempenho de um público-alvo que corresponde ao público-alvo de seu colaborador. Essa pontuação é calculada com base em contagem de público-alvo e sobreposições subjacentes. Para saber mais sobre as pontuações do índice de público-alvo, leia o guia [pontuação do índice de público-alvo](../collaborate/discover.md#audience-index-score).

## Maio de 2025 {#may-2025}

* O Real-Time CDP Collaboration agora está disponível para clientes na **Austrália** e na **Nova Zelândia**. Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate nessas regiões.
* O Real-Time CDP Collaboration agora oferece [destinos de autoatendimento](../setup/manage-destinations.md) por meio da guia **[!UICONTROL Meus destinos]** na seção **[!UICONTROL Configuração]**. Os destinos permitem ativar públicos-alvo em plataformas de terceiros, como redes de publicidade ou plataformas de gerenciamento de dados, para alcançar seus clientes em vários canais. No momento, somente os destinos do Adobe Experience Platform são compatíveis. Se você estiver interessado em configurar um destino diferente, entre em contato com o representante da Adobe. Para saber mais sobre destinos, leia o guia [visão geral dos destinos](../destinations/overview.md).
   * Destinos também adiciona suporte para exibir públicos da Collaboration no [portal de público-alvo da Adobe Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* Agora você pode editar a frequência de atualização do público-alvo para conexões de dados existentes no Collaboration. Atualmente, você pode optar por atualizar os públicos-alvo diariamente ou a cada dois ou seis dias. Para saber mais sobre como editar a frequência de atualização do público-alvo, leia o guia [gerenciar conexões de dados](../setup/manage-data-connection.md#scheduling).
* As divisões de crédito entre colaboradores agora são definidas para cada caso de uso selecionado na conexão. Você pode definir diferentes regras de consumo de crédito para cada caso de uso para controlar melhor como seus créditos são usados. Para saber mais sobre a funcionalidade de divisão de crédito, leia o guia [configurações de conexão](../connect/establishing-connections.md#connection-settings). Para saber mais sobre como os créditos são consumidos, leia o guia [tipos de atividade de crédito](../setup/my-activity.md#types-of-activities). <br> ![Tela de configurações de conexão mostrando a funcionalidade de divisão de crédito.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Agora, os editores podem definir nomes e IDs de anunciante antes de aceitar as configurações de conexão de um anunciante. Os editores podem definir nomes e IDs que se alinham a seus sistemas internos, que podem ser diferentes dos nomes e IDs do anunciante. Para saber mais sobre como adicionar nomes e IDs de anunciante, leia o guia [configurações de conexão](../connect/establishing-connections.md#connection-settings.md). <br> ![Tela de configurações de conexão mostrando o publicador definindo nomes e IDs de anunciante.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

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
