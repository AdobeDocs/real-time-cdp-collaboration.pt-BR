---
title: Source e gerenciar públicos
description: Saiba como fornecer e gerenciar públicos-alvo no Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 2f2a128f1591ac864d2ebef09c58ecc93bed8d98
workflow-type: tm+mt
source-wordcount: '2985'
ht-degree: 19%

---

# Source e gerenciar públicos

{{limited-availability-release-note}}

Os públicos-alvo são grupos específicos de usuários ou clientes segmentados com base em vários atributos. Eles permitem que os colaboradores trabalhem em conjunto em marketing direcionado e experiências personalizadas para campanhas publicitárias mais eficazes. Este guia aborda como originar públicos-alvo na Real-Time CDP Collaboration, exibir o painel de públicos-alvo e gerenciar públicos-alvo individuais.

>[!BEGINSHADEBOX]

O que você encontrará nesta página de documentação:

* [Públicos-alvo da Source na Collaboration](#source-audiences)
* [Exibir painel de públicos-alvo](#view-audiences-dashboard)
* [Exibir públicos-alvo individuais](#view-individual-audiences)

>[!ENDSHADEBOX]

## Públicos-alvo da Source na Collaboration {#source-audiences}

>[!IMPORTANT]
>
>Para públicos de origem, seu usuário precisa ser atribuído a uma função que contém duas permissões de Gerenciamento de Perfil - **[!UICONTROL Exibir Perfis]** e **[!UICONTROL Exibir Segmentos]**. Para obter informações sobre como atribuir as permissões necessárias, consulte o guia [fornecimento de público-alvo](../permissions/overview.md#audience-sourcing) em permissões.

Antes de ativar públicos-alvo com colaboradores e executar cálculos de sobreposição, os públicos-alvo precisam ser originados na Collaboration. Para direcionar públicos-alvo, siga as etapas do fluxo de trabalho na seção abaixo.

Na guia **[!UICONTROL Meus públicos-alvo]** do espaço de trabalho **[!UICONTROL Configuração]**, selecione o ícone adicionar (![ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Público-alvo]**. Se este for seu primeiro público-alvo, você também poderá selecionar a opção **[!UICONTROL Adicionar]**.

![Meu espaço de trabalho de públicos-alvo com a opção Adicionar e a opção Públicos-alvo realçadas.](/help/assets/setup/add-manage-audiences/add-audiences.png)

### Selecionar conexão de dados {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Ações de marketing"
>abstract="<p>Use ações de marketing para controlar quais dados de público-alvo importar para colaboração na Real-Time CDP a partir da Experience Platform. A ação de marketing <strong>Colaboração de dados</strong> é compatível com os rótulos de uso de dados C4, C5 e C9. A ação de marketing <strong>Ciência de dados</strong> é compatível com o rótulo de uso de dados C9.</p> <p> <ul><li> Com a caixa de seleção <em>habilitada</em>, todos os dados marcados com os rótulos mencionados acima na Experience Platform serão excluídos e <strong>não</strong> serão enviados para a Real-Time CDP Collaboration.</li><li> Com a caixa de seleção <em>desabilitada</em>, não há restrição para dados da Experience Platform que possam ser importados para a Real-Time CDP Collaboration.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=pt-BR" text="Visão geral dos rótulos de uso de dados"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=pt-BR" text="Glossário de rótulos de uso de dados"

>[!IMPORTANT]
>
>Depois de estabelecer para sua primeira conexão de dados e importar o primeiro público-alvo, você pode importar vários públicos-alvo da conexão de dados existente. Ao adicionar públicos-alvo adicionais, você começará pela etapa [selecionar público-alvo](#select-audiences), pois a conexão de dados já foi estabelecida.

Uma conexão de dados é a fonte de dados da qual você está fornecendo públicos-alvo. No momento, a única conexão de dados compatível é a Adobe Experience Platform.

Todas as configurações, como o agendamento definido para a conexão de dados, são aplicadas a todos os públicos-alvo provenientes dessa conexão de dados.

>[!TIP]
>
>Há um fluxo de trabalho separado em que você pode visualizar e editar suas conexões de dados. Para obter mais informações, siga o guia [gerenciando conexões de dados](/help/guide/setup/manage-data-connection.md).

Para começar a adicionar sua conexão de dados, selecione **[!UICONTROL Adicionar nova conexão de dados]** e clique em **[!UICONTROL Avançar]**.

![O espaço de trabalho Adicionar públicos-alvo com a opção Adicionar uma nova conexão de dados foi realçado.](/help/assets/setup/add-manage-audiences/add-data-connection.png)

#### Selecionar fonte de dados

Em seguida, escolha a origem da conexão de dados. As fontes disponíveis incluem:

* **Adobe Experience Platform**: selecione esta opção para trazer seus públicos do Adobe Experience Platform.
* **Arquivo CSV** (versão futura): carregue um arquivo CSV contendo seus dados de público-alvo para assimilação rápida e direta de dados.
* **Amazon Web Services** (versão futura): conecte-se ao seu armazenamento Amazon S3 para obter dados de público-alvo diretamente dos seus buckets do S3.
* **Snowflake** (versão futura): use o data warehouse do Snowflake para obter dados de público-alvo facilmente.
* **Google Cloud Platform** (versão futura): conecte-se ao Google Cloud Storage para obter dados de público-alvo diretamente dos seus buckets do GCS.

Selecione sua fonte de dados e selecione **[!UICONTROL Avançar]**.

![O espaço de trabalho Adicionar públicos-alvo com a opção Adobe Experience Platform está realçado.](/help/assets/setup/add-manage-audiences/select-data-connection-source.png)

#### Selecionar sandbox

Após selecionar a fonte de dados, é necessário selecionar a sandbox que inclui os públicos-alvo que você deseja usar na Collaboration. Selecione a sandbox na lista de sandboxes disponíveis e selecione **[!UICONTROL Avançar]**

![O espaço de trabalho Adicionar públicos-alvo com uma sandbox selecionada.](/help/assets/setup/add-manage-audiences/select-sandbox.png)

#### Política de governança e medidas de aplicação {#governance-policy-and-enforcement-actions}

Em seguida, verifique se as ações de marketing corretas estão definidas nos dados fornecidos. Você também precisa fornecer consentimento para que os dados obtidos do Experience Platform sejam usados para colaboração de dados.

Use ações de marketing para controlar quais dados de público-alvo trazer para o Collaboration a partir do Experience Platform. A ação de marketing **[!UICONTROL Colaboração de dados]** é compatível com os rótulos de uso de dados C4, C5 e C9. A ação de marketing **[!UICONTROL Ciência de dados]** é compatível com o rótulo de uso de dados C9.

Leia mais sobre os [rótulos de uso de dados C4, C5 e C9](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Quando a caixa de seleção estiver ***habilitada***, todos os dados rotulados no Experience Platform conforme descrito acima serão excluídos e **não** serão trazidos para o Collaboration.
* Com a caixa de seleção ***desabilitada***, não há restrição nos dados obtidos do Experience Platform.

Leia mais sobre os rótulos de uso de dados na documentação do Experience Platform:

* [Visão geral dos rótulos de uso de dados](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [Glossário de rótulos de uso de dados](https://experienceleague.adobe.com/pt-br/docs/experience-platform/data-governance/labels/reference){target="_blank"}

Além disso, selecione suas regras de consentimento a serem aplicadas aos dados que estão sendo originados na Collaboration.

![O espaço de trabalho Adicionar públicos-alvo na seção Política de governança e ações de imposição.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

Depois de selecionar as ações de marketing e as regras de consentimento, selecione **[!UICONTROL Avançar]** para prosseguir para a próxima etapa. Uma caixa de diálogo de confirmação será exibida, solicitando que você aceite os termos. Marque a caixa de seleção e selecione **[!UICONTROL OK]** para confirmar.

![Caixa de diálogo Política de governança e ações de aplicação com a caixa de seleção e a opção OK realçadas.](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png)

### Forneça detalhes

Em seguida, forneça um nome e uma descrição para sua conexão de dados. Essas informações ajudarão você a identificar a conexão de dados posteriormente.

![O espaço de trabalho Adicionar públicos-alvo com a opção para fornecer um nome e uma descrição.](/help/assets/setup/add-manage-audiences/data-connection-details.png)

### Mapear campos {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Campos de origem"
>abstract="Os campos de origem são namespaces de identidade e atributos da implementação da Experience Platform. É possível mapeá-los para campos de destino definidos em Collaboration."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Campos de destino"
>abstract="Atualmente, os emails com hash são as únicas chaves de correspondência compatíveis."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="Aplicar transformação"
>abstract="Ao importar campos *sem hash*, use essa opção para que a Collaboration aplique hash e transforme os campos simples em campos com hash."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="Namespaces de identidade"
>abstract="Selecione um namespace de identidade nos namespaces de identidade padrão e personalizados disponíveis em sua organização da Experience Platform."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html?lang=pt-BR#standard" text="Namespaces padrão e de identidade na Experience Platform"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="Atributos do perfil"
>abstract="Selecione atributos do esquema de união para a classe Perfil na Experience Platform. Essa exibição mostra atributos que estão presentes no esquema de união e pertencem à classe Perfil individual XDM."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html?lang=pt-BR" text="Esquema de união na Experience Platform"

Em seguida, você selecionará campos de origem para mapear para campos de destino no Collaboration.

![O espaço de trabalho Adicionar públicos-alvo com a opção para mapear campos de origem para campos de destino.](/help/assets/setup/add-manage-audiences/add-map-fields.png)

>[!TIP]
>
>Você pode mapear vários campos de origem para o mesmo campo de destino. Por exemplo, se você tiver endereços de email em dois campos separados no Experience Platform, poderá mapear cada um desses para o campo de destino **[!UICONTROL Email com hash]** como duas linhas separadas.

>[!BEGINSHADEBOX]

**[!UICONTROL Os campos do Source]** são namespaces de identidade e atributos da Experience Platform. Essas são as identidades existentes na plataforma da qual você está fornecendo dados. Os campos do Source são mapeados para os campos de destino definidos no Collaboration.

**[!UICONTROL Os campos de destino]** indicam como as identidades são referenciadas no Collaboration. Atualmente, os emails com hash são as únicas chaves de correspondência compatíveis.

Use a opção **[!UICONTROL Aplicar transformação]** ao importar campos *sem hash* da sua origem. Nesse caso, o Collaboration aplicará o hash e transformará os campos. O algoritmo de hash usado pelo Adobe é SHA256.

>[!ENDSHADEBOX]

Selecione o campo de origem vazio ao lado do campo de destino. A caixa de diálogo **[!UICONTROL Selecionar campo de origem]** será exibida. Selecione entre as opções **[!UICONTROL Namespaces de identidade]** e **[!UICONTROL Atributos do perfil]** para localizar o campo de origem desejado e selecione o campo na lista. Também é possível usar a opção de pesquisa para localizar o campo desejado.

![A caixa de diálogo Selecionar campo de origem com as opções de email exibidas.](/help/assets/setup/add-manage-audiences/select-source-field.png)

Para lidar com vários campos de email, mapeie o campo de origem de email sem hash usando **[!UICONTROL Aplicar transformação]**.

![O espaço de trabalho Adicionar públicos-alvo com os campos de origem de email mapeados para o campo de destino, com a opção Aplicar transformação ativada para um campo.](/help/assets/setup/add-manage-audiences/apply-transformation.png)

Continue adicionando pares de mapeamento conforme necessário e selecione **[!UICONTROL Avançar]**.

### Agendar {#schedule}

Em seguida, programe quando começar e terminar de preencher os públicos. O público será atualizado de acordo com este agendamento.

![O espaço de trabalho Adicionar público-alvo com as opções de agendamento exibidas.](/help/assets/setup/add-manage-audiences/audience-scheduling.png)

>[!IMPORTANT]
>
>Ajustar a frequência de atualizações de público ajudará a gerenciar a [atividade de crédito de Gerenciamento de público-alvo](/help/guide/setup/my-activity.md#types-of-activities), que é calculada por atualização de público-alvo. Selecionar uma frequência mais alta pode afetar a atualização dos dados disponíveis para os relatórios de descoberta de público-alvo e a ativação de público-alvo.

Selecione a frequência de atualização do público na lista suspensa **[!UICONTROL Frequência]**.

![O espaço de trabalho Adicionar agendamento de públicos-alvo com a lista suspensa de Frequência aberta.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png)

Em seguida, selecione o **[!UICONTROL Intervalo de datas]**. A data de início é a data em que o público-alvo começará a preencher com perfis, e a data de término é quando o público-alvo parará de ser atualizado.

![A opção Adicionar espaço de trabalho de agendamento de públicos-alvo com o intervalo de datas é exibida.](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png)

>[!IMPORTANT]
>
>Após a data de término no intervalo de datas, todos os públicos-alvo provenientes dessa conexão de dados deixarão de ser atualizados. Para renovar a conexão, siga o guia [gerenciar conexão de dados](/help/guide/setup/manage-data-connection.md).

### Selecionar públicos-alvo {#select-audiences}

Depois de selecionar a origem do público-alvo, você escolherá públicos-alvo específicos para incluir. Use as opções de pesquisa e filtro para localizar os públicos relevantes da sua fonte de dados. Selecione os públicos desejados e clique em **[!UICONTROL Avançar]**.

![O espaço de trabalho Adicionar públicos-alvo com uma lista de públicos-alvo disponíveis.](/help/assets/setup/add-manage-audiences/select-audience.png)

### Revisar

Revise todas as configurações e definições antes de finalizar a adição do público-alvo. Verifique se todos os detalhes estão corretos e selecione **[!UICONTROL Concluído]** para concluir a criação da conexão de dados.

![O espaço de trabalho Adicionar públicos-alvo com todas as configurações selecionadas foi exibido.](/help/assets/setup/add-manage-audiences/review-connection.png)

## Exibir painel de públicos-alvo {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Identidades ausentes"
>abstract="A contagem de identidades estará disponível após a próxima atualização da conexão de dados, de acordo com o agendamento configurado. A atualização inicial geralmente ocorre em 24 horas após a configuração da conexão de dados. Atualizações contínuas seguirão o cronograma configurado."

Depois de fornecer os públicos-alvo, o espaço de trabalho **[!UICONTROL Meus públicos-alvo]** exibe todos os públicos-alvo originados no Collaboration no momento.

Cada público-alvo contém uma visão geral das seguintes informações:

| Item | Descrição |
|----------|---------|
| **[!UICONTROL Identidades]** | Indica o número de identidades presentes nesse público-alvo. Observe que, se o mesmo perfil tiver duas ou mais identidades, e essas identidades forem usadas como chaves de correspondência no projeto, o perfil aparecerá duas vezes na contagem. |
| **[!UICONTROL Status]** | Indica se a audiência está ativa e pode ser usada em projetos. Um status **[!UICONTROL Pendente]** indica que o público-alvo acabou de ser originado e as identidades ainda não foram preenchidas. Os públicos-alvo fornecidos serão preenchidos com perfis após a atualização inicial, que geralmente ocorre em 24 horas após a configuração da conexão de dados. |
| **[!UICONTROL Source]** | Indica de onde o público-alvo foi originado. Na versão atual do Collaboration, o Experience Platform é a única fonte compatível. |
| **[!UICONTROL Conexão de dados]** | A conexão de dados da qual o público-alvo tem origem. Você pode selecionar o nome para exibir a conexão de dados. |
| **[!UICONTROL Acesso à conexão]** | Define se o público é privado ou público. Os públicos-alvo são detectáveis em relatórios de sobreposição e podem ser ativados em um projeto. |
| **[!UICONTROL Criado]** | Indica quando o público-alvo foi originado inicialmente na Collaboration. |
| **[!UICONTROL Última atualização]** | Indica a última data e hora em que o público-alvo foi atualizado no Collaboration. Não se refere a quando o público-alvo foi atualizado pela última vez, mas sim quando a configuração ou os metadados do público-alvo foram alterados pela última vez. |

![O espaço de trabalho Meu público-alvo mostrando todos os públicos-alvo originados.](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

Para executar ações rápidas em um público, selecione as reticências **...** ao lado do nome do público. As opções disponíveis são as seguintes:

* **[!UICONTROL Editar categorias]** permite adicionar diferentes marcas de categoria ao público-alvo. Para obter mais informações, consulte a seção [categorias](#categories) abaixo.
* **[!UICONTROL Excluir]** excluirá o público da conexão de dados.

![O espaço de trabalho Meus públicos-alvo com o menu de reticências é aberto, e as opções Editar categorias e Excluir são realçadas.](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png)

## Exibir públicos-alvo individuais {#view-individual-audiences}

Para exibir mais informações e editar configurações para um público individual, selecione o público no espaço de trabalho **[!UICONTROL Meus públicos]**. O espaço de trabalho de público-alvo exibe informações detalhadas sobre o público-alvo selecionado, incluindo seus detalhes, identidades, categorias, acesso à conexão e configurações de visibilidade de metadados.

### Detalhes do público-alvo

As seguintes informações são exibidas para cada público individual:

| Item | Descrição |
|----------|---------|
| **[!UICONTROL Status]** | Indica se a audiência está ativa e pode ser usada em projetos. |
| **[!UICONTROL Source]** | Indica de onde o público-alvo foi originado. Na versão atual do Collaboration, o Experience Platform é a única fonte compatível. |
| **[!UICONTROL Conexão de dados]** | A conexão de dados da qual o público-alvo tem origem. |
| **[!UICONTROL Última atualização]** | Indica a última data e hora em que o público-alvo foi atualizado no Collaboration. Não se refere a quando o público-alvo foi atualizado pela última vez, mas sim quando a configuração ou os metadados do público-alvo foram alterados pela última vez |
| **[!UICONTROL Última atualização por]** | Indica o usuário que atualizou o público pela última vez. |
| **[!UICONTROL Criado]** | Indica quando o público-alvo foi originado inicialmente na Collaboration. |
| **[!UICONTROL Criado por]** | Indica o usuário que originou o público no Collaboration. |

![Espaço de trabalho de um público-alvo individual.](/help/assets/setup/add-manage-audiences/audience-details.png)

Além disso, os seguintes controles estão disponíveis no espaço de trabalho do público-alvo:

* **[!UICONTROL Excluir]**: remova o público-alvo de sua conexão de dados.
* **[!UICONTROL Editar]**: edite o nome ou a descrição do público-alvo.

![Um espaço de trabalho de público-alvo individual com a opção Editar e Excluir realçada.](/help/assets/setup/add-manage-audiences/audience-details-edit-delete.png)

Em seguida, você pode atualizar as seguintes seções no espaço de trabalho do público-alvo:

* [Identidades](#identities)
* [Categorias](#categories)
* [Acesso à conexão](#connection-access)
* [Visibilidade de metadados](#metadata-visibility)

### Identidades {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identidades"
>abstract="Uma visualização detalhada das identidades que compõem esse público-alvo, bem como uma contagem total de perfis com as respectivas identidades."

A seção **[!UICONTROL Identidades]** indica o número de perfis presentes no público com qualquer uma das identidades que você selecionou ao fornecer o público. A seção também contém um detalhamento de identidade para que você possa saber quais identidades compõem a maioria da população do público-alvo.

![A seção Identidades do espaço de trabalho de um público-alvo individual.](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

### Categorias {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Categorias"
>abstract="Adicione tags aos públicos-alvo para facilitar a organização, a filtragem e a recuperação. Você pode marcar um público-alvo com várias categorias e então usar essas tags de categoria para filtrar os públicos-alvo desejados em outras áreas do produto."

Para facilitar a organização, a filtragem e a recuperação de públicos-alvo, você pode marcar seus públicos-alvo. Você pode marcar um público com várias categorias e usar essas marcas de categoria para filtrar os públicos desejados na área de produto [descoberta](/help/guide/collaborate/discover.md), ao executar relatórios de sobreposição de público.

Para adicionar categorias, selecione a opção **[!UICONTROL Editar]** na seção **[!UICONTROL Categorias]**.

![A seção Categorias do espaço de trabalho de um público-alvo individual.](/help/assets/setup/add-manage-audiences/audience-details-categories.png)

A caixa de diálogo **[!UICONTROL Categorias]** será exibida, permitindo que você selecione as categorias que deseja adicionar ao público-alvo. Para selecionar uma categoria individual, marque a caixa de seleção ao lado do nome da categoria.

![A caixa de diálogo Categorias exibida com as categorias disponíveis.](/help/assets/setup/add-manage-audiences/audience-details-categories-select.png)

### Acesso à conexão {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Acesso à conexão"
>abstract="<p>Os públicos-alvo podem ser de três tipos: públicos, privados e personalizados.</p><p> Sua disponibilidade para uso em projetos com colaboradores difere com base na configuração de acesso à conexão. É sempre possível alterar o acesso à conexão de privado para público, mas não será permitido reverter essa configuração a partir do momento que um público-alvo for ativado com colaboradores.</p>"

A disponibilidade de um público-alvo para uso em projetos com colaboradores é diferente com base na configuração de acesso à conexão. Na seção **[!UICONTROL Acesso à conexão]**, você pode selecionar se o público-alvo deve ser privado ou público. Os públicos-alvo públicos-alvo são utilizáveis e detectáveis em conexões.

Para atualizar o acesso à conexão do público-alvo, selecione a opção **[!UICONTROL Editar]** na seção **[!UICONTROL Acesso à conexão]**.

![A seção Acesso à conexão do espaço de trabalho de um público-alvo individual.](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png)

A caixa de diálogo **[!UICONTROL Acesso à conexão]** é exibida, com três opções de acesso à conexão disponíveis:

* **[!UICONTROL Público-alvo]**. Estes públicos-alvo *não* estão disponíveis para uso em relatórios de sobreposição ou para ativação em conexões com qualquer colaborador. Embora os públicos-alvo não estejam disponíveis para os colaboradores visualizarem ou usarem, a população dos públicos-alvo ainda contribui para a população total na exibição **[!UICONTROL Todos os públicos-alvo]** da [seção Comparar públicos-alvo](/help/guide/collaborate/discover.md#compare-audiences). Altere a configuração para público ou personalizado para usar os públicos-alvo em conexões com colaboradores.
* **[!UICONTROL Público]**. Esses públicos-alvo estão disponíveis para uso em relatórios de sobreposição e para ativação em conexões com qualquer colaborador.
* **[!UICONTROL Público-alvo personalizado]**. Esses públicos-alvo estão disponíveis para uso em relatórios de sobreposição e para ativação somente em conexões especificadas. Embora os públicos-alvo não estejam disponíveis para os colaboradores visualizarem ou usarem, a população dos públicos-alvo ainda contribui para a população total na exibição **[!UICONTROL Todos os públicos-alvo]** da [seção Comparar públicos-alvo](/help/guide/collaborate/discover.md#compare-audiences).

Selecione a opção de acesso de conexão desejada e selecione **[!UICONTROL Salvar]** para aplicar as alterações.

![A caixa de diálogo Acesso à conexão com as opções disponíveis foi exibida.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

>[!IMPORTANT]
>
>Independentemente do status de acesso (público, privado ou personalizado), a população de qualquer público-alvo contribui para a população **[!UICONTROL Todos os públicos-alvo]** na seção **[!UICONTROL Comparar públicos-alvo]** em um projeto.

A disponibilidade do público-alvo para uso em projetos com colaboradores é diferente de acordo com a configuração de acesso à conexão. Você sempre pode alterar o acesso à conexão de privado para público, mas não pode alterar essa configuração novamente depois que um público-alvo for ativado.

### Visibilidade de metadados {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Visibilidade de metadados"
>abstract="<p>Indica quais metadados de público-alvo estão visíveis para outros colaboradores antes que se conectem com você ou em visualizações de projeto.</p> <p> A **Contagem de identidades** controla se o seu colaborador pode exibir contagens de identidades dos seus públicos-alvo ao visualizar relatórios de sobreposição na guia de descoberta.</p><p> A **% de sobreposição de público-alvo** controla se os colaboradores podem descobrir as porcentagens de sobreposição entre os públicos-alvo deles e os seus.</p><p> O **[!UICONTROL Índice de público-alvo]** controla se os colaboradores podem exibir o índice de público-alvo em um projeto. Essa funcionalidade só está disponível quando você tem três ou mais públicos-alvo ativos.</p> <br> Para que as configurações de visibilidade de metadados entrem em vigor, o público-alvo precisa ter sido definido como público ou personalizado."

>[!NOTE]
>
>Se o colaborador tiver todos os públicos definidos como privados, a seção **[!UICONTROL Públicos relevantes]** de um projeto no espaço de trabalho **[!UICONTROL Descobrir]** ficará em branco. Para obter mais informações, leia o guia [descoberta](/help/guide/collaborate/discover.md#relevant-audiences).

A visibilidade dos metadados indica a visibilidade dos metadados de um público-alvo para outros colaboradores antes que eles se conectem com você ou em diferentes visualizações de projeto. Para atualizar a visibilidade de metadados do público, selecione a opção **[!UICONTROL Editar]** na seção **[!UICONTROL Visibilidade de metadados]**.

![A seção Visibilidade de metadados do espaço de trabalho de um público-alvo individual.](/help/assets/setup/add-manage-audiences/audience-details-metadata.png)

A caixa de diálogo **[!UICONTROL Visibilidade de metadados]** é exibida, permitindo definir as configurações de visibilidade para o público-alvo. Há duas configurações de visibilidade de metadados que você pode configurar para cada público:

**[!UICONTROL Mostrar contagem de identidades]**: esta configuração controla se seu colaborador pode exibir contagens de identidades para seus públicos ao [exibir relatórios de sobreposição na guia de descoberta](/help/guide/collaborate/discover.md#discover-overlaps) em um projeto.

**[!UICONTROL Mostrar sobreposição de público-alvo %]**: esta configuração controla se os colaboradores podem [descobrir porcentagens de sobreposição](/help/guide/collaborate/discover.md#compare-audiences) entre seus públicos-alvo e os seus públicos-alvo.

**[!UICONTROL Índice de público-alvo]**: quando definido como verdadeiro, seus colaboradores podem exibir o [índice de público-alvo](/help/guide/collaborate/discover.md#audience-index-score) em um projeto. Essa funcionalidade só está disponível quando você tem três ou mais públicos-alvo ativos.

>[!NOTE]
>
>Para que as configurações de visibilidade de metadados entrem em vigor, o público-alvo deve ser definido como público ou personalizado.

![A caixa de diálogo de visibilidade de Metadados com as opções disponíveis foi exibida.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

## Próximas etapas

Depois de fornecer públicos-alvo, é hora de descobrir editores para [conectar](/help/guide/connect/establishing-connections.md) com a para colaborar em projetos.
