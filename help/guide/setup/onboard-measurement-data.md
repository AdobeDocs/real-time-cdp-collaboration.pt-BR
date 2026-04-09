---
title: Adicionar e gerenciar dados de medição
description: Saiba como adicionar dados de medição ao Adobe Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 739d31b9-3f00-477d-b6be-995c7767c6ca
source-git-commit: 42bbd17878701cfaf2cba170a9471cf5c7285796
workflow-type: tm+mt
source-wordcount: '1918'
ht-degree: 5%

---

# Adicionar e gerenciar dados de medição {#add-and-manage-measurement-data}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_onboard_measurement_data"
>title="Saiba mais"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_data_target_fields"
>title="Campos de destino"
>abstract="Espaço reservado para campos de destino de medição."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_data_source_fields"
>title="Campos de origem"
>abstract="Espaço reservado para campos de origem de medição."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_measurement_mapping_source_fields"
>title="Mapear campos da origem"
>abstract="Espaço reservado para o mapeamento de medição dos campos de origem."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_measurement_mapping_target_fields"
>title="Mapear campos de origem"
>abstract="Espaço reservado para o mapeamento de medição dos campos de destino."

{{limited-availability-release-note}}

Este documento descreve as etapas para adicionar dados de medição da campanha ao Adobe Real-Time CDP Collaboration. Os editores podem trabalhar com as equipes do Adobe para carregar dados de medição da campanha. Depois que os dados forem carregados e processados, tanto o editor quanto o anunciante poderão exibir [relatórios de medição de campanha](/help/guide/collaborate/measure.md) abrangentes.

## Adicionar dados de medição {#add-measurement-data}

Como anunciante, você pode fazer upload de seus dados de medição que contêm eventos de conversão para o Collaboration para usar em relatórios de medição de campanha. Os dados de conversão normalmente incluem campos como identificadores de usuário (por exemplo, email com hash ou IDs de dispositivo), carimbo de data e hora do evento de conversão e detalhes específicos do evento de conversão, como compra ou inscrição.

Para originar dados de medição, navegue até a guia **[!UICONTROL Meus dados de medição]** no espaço de trabalho **[!UICONTROL Configuração]**. Selecione o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Dados de medição]**.

Se esses forem seus primeiros dados de medição, você também poderá selecionar a opção **[!UICONTROL Adicionar]**.

![Guia Meus dados de medição com as opções Adicionar e Dados de medição realçadas.](../../assets/setup/add-manage-measurement-data/add-measurement-data.png){zoomable="yes"}

A tela **[!UICONTROL Adicionar dados de medição]** é exibida, exibindo um resumo das etapas para a origem dos dados de medição. Selecione **[!UICONTROL Iniciar integração]**.

![A tela Adicionar dados de medição exibindo um resumo das etapas dos dados de medição de origem e a opção Iniciar integração realçada.](../../assets/setup/add-manage-measurement-data/add-measurement-data-screen.png){zoomable="yes"}

### Conexão de dados e detalhes {#data-connection-and-details}

Nesta etapa, é necessário configurar a conexão de dados e especificar os detalhes dos dados de medição.

#### Selecionar tipo de dados de medição {#select-measurement-data-type}

O tipo de dados de medição define o tipo de eventos que você traz para a medição da campanha. Atualmente, dados de conversão é o tipo compatível.

Selecione **[!UICONTROL Dados de conversão]** como o tipo de dados de medição, seguido de **[!UICONTROL Próximo]**.

![A etapa Detalhes e conexão de dados que destaca o tipo de dados de medição e a opção Próximo.](../../assets/setup/add-manage-measurement-data/select-measurement-data-type.png){zoomable="yes"}

#### Selecionar conexão de dados {#select-data-connection}

Uma conexão de dados é a origem de onde você origina os dados de medição no Collaboration. Depois de estabelecer sua conexão de dados inicial e originar seu primeiro conjunto de dados de medição, você pode continuar fornecendo dados de medição adicionais usando a mesma conexão de dados.

Para adicionar uma conexão de dados, selecione **[!UICONTROL Adicionar nova conexão de dados]** e **[!UICONTROL Avançar]**.

![A etapa Conexão e detalhes de dados que destaca a opção Adicionar uma nova conexão de dados e a opção Avançar.](../../assets/setup/add-manage-measurement-data/select-measurement-data-connection.png){zoomable="yes"}

#### Selecionar fonte de dados {#select-data-source}

Em seguida, escolha a origem da conexão de dados. No momento, o Adobe Experience Platform é a única fonte de dados compatível.

Selecione sua fonte de dados e, em seguida, selecione **[!UICONTROL Próximo]**.

![A etapa Detalhes e conexão de dados destacando a opção Adobe Experience Platform e a opção Avançar.](../../assets/setup/add-manage-measurement-data/select-measurement-data-source.png){zoomable="yes"}

#### Selecionar sandbox {#select-sandbox}

Selecione a sandbox que inclui os dados de medição que você deseja usar para os relatórios de medição da campanha do Collaboration. Escolha a sandbox na lista de sandboxes disponíveis e selecione **[!UICONTROL Avançar]**.

![A etapa Detalhes e conexão de dados que destaca a sandbox de produção e a opção Avançar.](../../assets/setup/add-manage-measurement-data/select-sandbox.png){zoomable="yes"}

#### Selecionar conjunto de dados de medição {#select-measurement-dataset}

Uma lista de conjuntos de dados na sandbox selecionada é exibida. Selecione um conjunto de dados como seus dados de medição e selecione **[!UICONTROL Próximo]**. Você pode usar a opção Pesquisar para filtrar e encontrar o conjunto de dados preferido.

![A etapa Detalhes e conexão de dados destacando a opção Pesquisar, o Conjunto de Dados de Exemplo do Evento e a opção Próximo.](../../assets/setup/add-manage-measurement-data/select-measurement-dataset.png){zoomable="yes"}

#### Fornecer nome e detalhes {#provide-name-and-details}

Em seguida, forneça um nome e uma descrição para sua conexão de dados. Essas informações ajudarão você a identificar a conexão de dados posteriormente.

![A etapa Detalhes e conexão de dados com a opção para fornecer um nome e uma descrição.](../../assets/setup/add-manage-measurement-data/data-connection-name-details.png){zoomable="yes"}

### Mapeamento {#mapping}

A próxima etapa é mapear campos dos dados de medição para os campos de destino correspondentes usados no Collaboration. Você também pode optar por enriquecer seu conjunto de dados de evento com atributos do Perfil de cliente em tempo real mapeando chaves de junção e usar esses atributos para detalhar os relatórios de medição.

#### Enriquecer dados do evento {#enrich-event-data}

Para enriquecer os dados do evento, selecione a opção **[!UICONTROL Chave de junção do campo do Source]**.

![A tela Mapeamento com a opção de chave de junção de campo do Source está realçada.](../../assets/setup/add-manage-measurement-data/select-source-field-join-key.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL Chave de ingresso do campo do Source]**, escolha o campo de origem, seguido por **[!UICONTROL Selecionar]**.

![A caixa de diálogo da chave de ingresso do campo do Source realçando o campo do Source e a opção Avançar.](../../assets/setup/add-manage-measurement-data/source-field-join-key-dialog.png){zoomable="yes"}

Em seguida, selecione a opção **[!UICONTROL Chave de ingresso do perfil]**. Na caixa de diálogo **[!UICONTROL Chave de ingresso do perfil]**, selecione o campo de perfil na lista. Você pode usar a opção Search para localizar o campo desejado. Em seguida, escolha **[!UICONTROL Selecionar]** para confirmar.

![A caixa de diálogo da chave de ingresso do Perfil destacando a chave de Pesquisa, o campo de perfil selecionado e a opção Avançar.](../../assets/setup/add-manage-measurement-data/profile-join-key-dialog.png){zoomable="yes"}

#### Mapeamento de campos {#mapping-fields}

Para começar a mapear campos de origem dos dados de medição para os campos de destino no Collaboration, selecione o campo de origem vazio na tela **[!UICONTROL Mapeamento]**.

![A tela Mapeamento com o campo de origem vazio realçado.](../../assets/setup/add-manage-measurement-data/mapping-screen.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Selecionar campo de origem]** é exibida, exibindo uma lista de campos de origem disponíveis agrupados em opções como **[!UICONTROL Namespace de identidade]** e **[!UICONTROL Esquema de evento]**. Você pode usar a opção de pesquisa para filtrar e localizar o campo de origem na lista.

Escolha o campo de origem desejado, seguido por **[!UICONTROL Selecionar]**.

![A caixa de diálogo Selecionar campo de origem destacando o campo de origem Emails e a opção Selecionar.](../../assets/setup/add-manage-measurement-data/select-source-field-dialog.png){zoomable="yes"}

Em seguida, use o menu suspenso para mapear o campo de origem selecionado para um campo de destino apropriado. Todos os campos de destino disponíveis são as [chaves de correspondência configuradas para sua conta do Collaborator](./onboard-account.md#set-up-match-keys).

![O menu suspenso que exibe todos os campos de destino disponíveis para mapear com o campo de origem selecionado.](../../assets/setup/add-manage-measurement-data/select-target-field-dropdown.png){zoomable="yes"}

É possível adicionar ou remover linhas de mapeamento, conforme necessário. Se você precisar mapear um campo de origem sem hash para um campo de destino com hash (por exemplo, mapear um email de texto sem formatação para [!UICONTROL Email com hash]), use a opção **[!UICONTROL Aplicar transformação]** para aplicar o hash necessário.

Quando terminar, revise os campos mapeados e as chaves de junção se o enriquecimento estiver ativado. Em seguida, selecione **[!UICONTROL Próximo]**.

![A tela Mapeamento mostrando os campos mapeados, chaves de junção (quando o enriquecimento está habilitado) e a opção Avançar realçada.](../../assets/setup/add-manage-measurement-data/review-mapping.png){zoomable="yes"}

### Gerenciar consentimento {#manage-consent}

Antes de continuar, você deve reconhecer que o uso de dados no Collaboration está em conformidade com as políticas de governança de dados da Real-Time CDP. Todos os dados devem ser pré-filtrados de acordo com os requisitos de consentimento ou com as políticas de consentimento personalizadas aplicáveis, portanto, não é necessário nenhum processamento adicional.

Para confirmar sua confirmação, selecione **[!UICONTROL Avançar]**.

![A tela Gerenciar consentimento que requer confirmação com a opção Avançar foi realçada.](../../assets/setup/add-manage-measurement-data/manage-consent.png){zoomable="yes"}

Se você [habilitar o enriquecimento do perfil durante a etapa de mapeamento](#enrich-event-data), poderá configurar políticas de consentimento a partir de uma lista de opções predefinidas. Isso inclui:

* **Ações de marketing**: use essas ações de marketing para controlar quais dados de público-alvo trazer para a Collaboration da Experience Platform.
* **Regras de consentimento**: selecione as regras de consentimento a serem aplicadas aos dados que estão sendo originados na Collaboration.
* **Público-alvo**: use o filtro de público-alvo para incluir ou excluir perfis de público-alvo para consentimento.


>[!NOTE]
>
>**[!UICONTROL O Data Collaboration]** oferece suporte aos rótulos de uso de dados C4, C5 e C9, enquanto o **[!UICONTROL Data Science]** oferece suporte apenas a C9. Leia mais sobre os rótulos de uso de dados na documentação do Experience Platform:
>
>* [Visão geral dos rótulos de uso de dados](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/overview){target="_blank"}
>* [Glossário](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/reference){target="_blank"}

Selecione as configurações preferenciais e, em seguida, selecione **[!UICONTROL Avançar]**.

![A tela Gerenciar consentimento mostrando as opções de configuração de consentimento quando o enriquecimento do perfil está habilitado, com a opção Avançar realçada.](../../assets/setup/add-manage-measurement-data/manage-consent-configuration-options.png){zoomable="yes"}

Antes de continuar, você precisa confirmar e aceitar os termos na caixa de diálogo **[!UICONTROL Política de governança e ações de imposição]**. Marque a caixa de seleção, seguida de **[!UICONTROL OK]**.

![A caixa de diálogo Política de governança e ações de imposição mostrando a caixa de seleção e a opção OK destacadas.](../../assets/setup/add-manage-measurement-data/governance-policy-enforcement-actions-dialog.png){zoomable="yes"}

#### Filtro de público-alvo {#audience-filter}

Para incluir ou excluir determinados perfis de público-alvo para consentimento, use o menu suspenso **[!UICONTROL Filtro de público-alvo]**. Após selecionar esse filtro, a interface será atualizada para exibir a opção **[!UICONTROL Procurar públicos-alvo]**. Selecione **[!UICONTROL Procurar públicos]**.

![A tela Gerenciar consentimento mostrando a opção Procurar públicos-alvo depois que o filtro de público-alvo é selecionado.](../../assets/setup/add-manage-measurement-data/browse-audiences.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Selecionar públicos-alvo]** é exibida. Escolha um público da lista, seguido por **[!UICONTROL Selecionar]**.

![A caixa de diálogo Selecionar públicos-alvo destacando o público-alvo selecionado e a opção Selecionar.](../../assets/setup/add-manage-measurement-data/select-audiences-dialog.png){zoomable="yes"}

O público-alvo escolhido agora é exibido, com a opção de removê-lo, se necessário. Examine suas configurações de consentimento e selecione **[!UICONTROL Avançar]**.

![A tela Gerenciar consentimento destacando o público selecionado para consentimento e a opção Avançar.](../../assets/setup/add-manage-measurement-data/audience-for-consent.png){zoomable="yes"}

### Adicionar evento de conversão {#add-conversion-event}

Em seguida, defina os eventos de conversão nos quais você deseja medir o impacto de suas campanhas, por exemplo, visitas de site, registros ou compras concluídas. Você pode especificar até **3** eventos de conversão distintos para medição.

Forneça o nome do evento de conversão e use o menu suspenso para selecionar o tipo de conversão.

![A tela Adicionar evento de conversão destacando o menu suspenso do tipo de conversão foi expandida.](../../assets/setup/add-manage-measurement-data/conversion-type-dropdown.png){zoomable="yes"}

Você pode inserir um valor para a conversão ou deixá-lo vazio se não quiser atribuir um valor neste momento.

![A tela Adicionar evento de conversão destacando a opção de valor de Conversão.](../../assets/setup/add-manage-measurement-data/conversion-value.png){zoomable="yes"}

Em seguida, você precisa especificar a chave de duplicação para indicar quais linhas no conjunto de dados do evento pertencem ao mesmo evento de conversão subjacente (por exemplo, o mesmo carimbo de data e hora durante um processo de inscrição). Isso impede a contagem da mesma conversão várias vezes nos relatórios de medição. Para fazer isso, selecione **[!UICONTROL Chave de duplicação]**. Na caixa de diálogo **[!UICONTROL Chave de duplicação]**, localize e escolha a chave, seguida por **[!UICONTROL Selecionar]**.

![A caixa de diálogo Chave de Duplicação mostrando a chave selecionada e a opção Selecionar.](../../assets/setup/add-manage-measurement-data/duplication-key-dialog.png){zoomable="yes"}

Depois de especificar a chave de duplicação, você pode adicionar até **5** condições para incluir somente linhas relevantes do conjunto de dados do evento para a conversão. Escolha aplicar todas ou qualquer uma dessas condições.

Selecione **[!UICONTROL Adicionar condição]** e selecione a opção de condição.

![A tela Adicionar evento de conversão realçando a opção de condição após selecionar a opção Adicionar condição.](../../assets/setup/add-manage-measurement-data/add-condition.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL Selecionar campo de origem]**, localize e escolha um campo de origem para a regra de condição, seguido por **[!UICONTROL Selecionar]**.

![A caixa de diálogo Selecionar campo de origem destacando o campo Tipo de Evento e a opção Selecionar.](../../assets/setup/add-manage-measurement-data/select-condition-field.png){zoomable="yes"}

Use o menu suspenso para selecionar um operador lógico e, em seguida, insira o valor da regra de configuração.

![A tela Adicionar evento de conversão destacando a lista suspensa do operador lógico e a opção Valor.](../../assets/setup/add-manage-measurement-data/logic-operator-dropdown.png){zoomable="yes"}

Para adicionar outro evento de conversão, selecione **[!UICONTROL Adicionar conversão]**. Você pode incluir até **3** eventos de conversão no total. Depois de concluído, revise as configurações de conversão e selecione **[!UICONTROL Próximo]**.

![A tela Adicionar evento de conversão mostrando as configurações do evento de conversão e a opção Avançar foram realçadas.](../../assets/setup/add-manage-measurement-data/add-conversion-event.png){zoomable="yes"}

### Revisar {#review}

A tela **[!UICONTROL Revisão]** é exibida com um resumo das configurações de dados de medição. Revise e verifique se todas as informações estão corretas. Se precisar alterar qualquer seção, use a opção **[!UICONTROL Editar]**.

Finalmente, selecione **[!UICONTROL Concluir]** para concluir a adição dos dados de medição.

![A tela Revisão mostrando um resumo das configurações de dados de medição e a opção Concluído realçada.](../../assets/setup/add-manage-measurement-data/review-measurement-data.png){zoomable="yes"}

Uma caixa de diálogo de confirmação confirma que os dados de medição foram criados com êxito. Você pode ver os novos eventos de conversão configurados com seus dados de medição no espaço de trabalho **[!UICONTROL Meus dados de medição]**.

![Meu espaço de trabalho de dados de medição mostrando uma lista de eventos de conversão configurados a partir dos dados de medição.](../../assets/setup/add-manage-measurement-data/conversion-event-list.png){zoomable="yes"}

Quando estiver na exibição de grade ou tabela, selecione um item de linha ou a opção **[!UICONTROL Exibir conversão]** em um cartão de evento para ter uma visão geral de um evento de conversão específico. Ele exibe o status do evento, a origem e o nome da conexão de dados, juntamente com painéis detalhados para:

* **[!UICONTROL Detalhes da conversão]**: exibe informações importantes sobre a conversão, incluindo seu tipo, a chave de duplicação usada para identificar eventos exclusivos e o valor de conversão atribuído (se especificado).
* **[!UICONTROL Condições]**: exibe as regras de condição aplicadas a este evento de conversão.

![A tela Visão Geral exibindo os detalhes de um evento de conversão.](../../assets/setup/add-manage-measurement-data/conversion-event-overview.png){zoomable="yes"}

## Próximas etapas {#next-steps}

Você concluiu a origem dos dados de medição no Collaboration. Como anunciante, agora você pode criar relatórios de atribuição para explorar como suas campanhas geram conversões e avaliam o impacto geral. Se você for um editor, solicite que seu colaborador gere um relatório de Atribuição para suas campanhas. Para obter instruções detalhadas, consulte o guia [Criar relatório de atribuição](../collaborate/measure.md#create-attribution-report).
