---
title: Importar e gerenciar públicos
description: Saiba como importar e gerenciar públicos no Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 2c835ce72f09c450aa3467dc72980c9c627a0ab8
workflow-type: tm+mt
source-wordcount: '2666'
ht-degree: 21%

---

# Importar e gerenciar públicos

{{limited-availability-release-note}}

Os públicos-alvo são grupos específicos de usuários ou clientes segmentados com base em vários atributos. Isso permite que anunciantes e editores colaborem em marketing direcionado e experiências personalizadas para campanhas de publicidade mais eficazes.

Use esta página como local de destino para entender todas as métricas relevantes que você pode visualizar relacionadas aos seus públicos, bem como as etapas do fluxo de trabalho para importar um público para o Adobe Real-Time CDP Collaboration.

>[!TIP]
>
>Use as informações nesta tela para obter todas as informações necessárias sobre os públicos-alvo, e as [telas de descoberta e sobreposição](/help/guide/collaborate/discover.md) para obter informações sobre qual dos públicos-alvo funcionaria melhor para diferentes tipos de campanha em comparação com o inventário do editor.

>[!BEGINSHADEBOX]

O que você encontrará nesta página de documentação:

* [Importar públicos-alvo para a Real-Time CDP Collaboration](#import-audiences)
* [Exibir painel de públicos-alvo](#view-audiences-dashboard)
* [Exibir públicos-alvo individuais](#view-individual-audiences)

>[!ENDSHADEBOX]

## Importar públicos-alvo para a Real-Time CDP Collaboration {#import-audiences}

>[!IMPORTANT]
>
>Para importar públicos, seu usuário precisa ser atribuído a uma função que contém duas permissões de Gerenciamento de perfil - Exibir perfis e Exibir segmentos. Para obter informações sobre como atribuir as permissões necessárias, consulte o guia [importação de público-alvo](../permissions/overview.md#audience-importation).

Antes de compartilhar públicos com colaboradores e executar cálculos de sobreposição, os públicos precisam ser importados para o Real-Time CDP Collaboration. Para importar públicos, siga as etapas do fluxo de trabalho na seção abaixo.

![Meus públicos-alvo são exibidos antes da adição de qualquer público-alvo à organização.](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

Na guia **[!UICONTROL Meus públicos-alvo]**, selecione o símbolo de adição **+** e selecione **Público-alvo**.

### Selecionar conexão de dados {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Ações de marketing"
>abstract="<p>Use ações de marketing para controlar quais dados de público-alvo importar para colaboração na Real-Time CDP a partir da Experience Platform. A ação de marketing <strong>Colaboração de dados</strong> é compatível com os rótulos de uso de dados C4, C5 e C9. A ação de marketing <strong>Ciência de dados</strong> é compatível com o rótulo de uso de dados C9.</p> <p> <ul><li> Com a caixa de seleção <em>habilitada</em>, todos os dados marcados com os rótulos mencionados acima na Experience Platform serão excluídos e <strong>não</strong> serão enviados para a Real-Time CDP Collaboration.</li><li> Com a caixa de seleção <em>desabilitada</em>, não há restrição para dados da Experience Platform que possam ser importados para a Real-Time CDP Collaboration.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=pt-BR" text="Visão geral dos rótulos de uso de dados"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=pt-BR" text="Glossário de rótulos de uso de dados"

>[!IMPORTANT]
>
>Depois de se conectar à primeira conexão de dados e importar o primeiro público-alvo, você pode optar por importar vários públicos-alvo dessa conexão de dados existente. Nesse caso, o fluxo de trabalho levará você diretamente à etapa [selecionar público-alvo](#select-audience), já que todas as informações de pré-requisito das outras etapas serão importadas da conexão existente.

Uma conexão de dados é a fonte de dados da qual você está importando públicos para o Real-Time CDP Collaboration. Para a primeira versão do Real-Time CDP Collaboration, a única conexão de dados compatível é a Adobe Experience Platform.

Todas as configurações, como mapeamento de identidade ou agendamento, definidas para a conexão de dados são aplicadas a todos os públicos-alvo importados dessa conexão de dados.

>[!TIP]
>
>Há um fluxo de trabalho separado em que você sempre pode exibir e editar todas as conexões de dados adicionadas nesta etapa. Leia mais sobre [gerenciamento de conexões de dados](/help/guide/setup/manage-data-connection.md).

![Selecione a tela de origem do público-alvo que mostra as opções do AEP RTCDP, Arquivo CSV, Amazon S3 e Snowflake.](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### Selecionar fonte de dados

Nesta etapa, você escolherá a fonte dos dados do público-alvo. As fontes disponíveis incluem:

* **Adobe Experience Platform**: selecione esta opção para trazer seus públicos do Adobe Experience Platform Real-Time CDP.
* **Arquivo CSV** (versão futura): carregue um arquivo CSV contendo seus dados de público-alvo para assimilação rápida e direta de dados.
* **Amazon Web Services** (versão futura): conecte-se ao seu armazenamento Amazon S3 para importar dados de público diretamente dos seus buckets do S3.
* **Snowflake** (versão futura): use o data warehouse do Snowflake para obter dados de público-alvo facilmente.

#### Selecionar sandbox

Depois de selecionar **Adobe Experience Platform** como fonte de dados, você deve selecionar a sandbox que inclui os públicos que você vai importar.

![Selecionar sandbox para importar públicos](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

Selecione **[!UICONTROL Avançar]** depois de selecionar a sandbox desejada.

#### Política de governação e medidas de execução {#governance-policy-and-enforcement-actions}

Em seguida, verifique se as ações de marketing corretas estão definidas nos dados importados. Você também precisa fornecer consentimento para que os dados importados da Real-Time CDP sejam usados para colaboração de dados.

Use ações de marketing para controlar quais dados de público-alvo importar para colaboração na Real-Time CDP a partir da Experience Platform. A ação de marketing **Colaboração de dados** é compatível com os rótulos de uso de dados C4, C5 e C9. A ação de marketing **Ciência de dados** é compatível com o rótulo de uso de dados C9.

Leia mais sobre os [rótulos de uso de dados C4, C5 e C9](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Com a caixa de seleção *habilitada*, todos os dados marcados com os rótulos mencionados acima na Experience Platform serão excluídos e *não* serão enviados para a Real-Time CDP Collaboration.
* Com a caixa de seleção *desabilitada*, não há restrição para dados da Experience Platform que possam ser importados para a Real-Time CDP Collaboration.

Leia mais sobre os rótulos de uso de dados na documentação do Experience Platform:

* [Visão geral dos rótulos de uso de dados](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [Glossário de rótulos de uso de dados](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![Ações de marketing necessárias para colaboração de dados.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### Fornecer detalhes

Em seguida, forneça um nome e uma descrição para que você reconheça essa conexão de dados no futuro.

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### Mapear campos {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Campos de origem"
>abstract="Os campos de origem são namespaces de identidade e atributos de sua implementação existente da Real-Time CDP. É possível mapeá-los para campos de destino definidos na Real-Time CDP Collaboration."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Campos de destino"
>abstract="Os campos de destino correspondem às chaves de correspondência selecionadas ao integrar sua empresa. Atualmente, os emails com hash são as únicas chaves de correspondência compatíveis."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="Aplicar transformação"
>abstract="Ao importar campos *sem hash* da origem, use essa opção para que a Real-Time CDP Collaboration aplique hash e transforme os campos simples em campos com hash."

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

![Tela Mapear campos mostrando campos de origem mapeados para campos de destino.](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

Na etapa mapear campos, é possível selecionar como os campos de identidade dos perfis trazidos da conexão de dados devem mapear para as chaves de correspondência selecionadas na organização.

>[!TIP]
>
>Você pode mapear vários campos de origem para o mesmo campo de destino. Por exemplo, se você tiver endereços de email em dois campos separados no Experience Platform, poderá mapear ambos para o campo de destino **[!UICONTROL Email com hash]** como duas linhas separadas.

>[!BEGINSHADEBOX]

**[!UICONTROL Os campos do Source]** indicam como as identidades são referenciadas na fonte da qual você está importando dados.

**[!UICONTROL Os campos de destino]** indicam como as identidades são referenciadas no Real-Time CDP Collaboration. Os valores que você pode selecionar aqui correspondem às chaves de correspondência configuradas no fluxo de trabalho de integração da empresa.

Use a opção **[!UICONTROL Aplicar transformação]** ao importar campos *sem hash* da sua origem. Nesse caso, o Real-Time CDP Collaboration aplicará o hash e transformará os campos. O algoritmo de hash usado pelo Adobe é SHA256.

>[!ENDSHADEBOX]

Adicione quantos pares de mapeamento forem necessários e selecione **[!UICONTROL Avançar]** para prosseguir para a próxima etapa.

<!--

In this step, you can also add any identity crosswalks that you would like to use.

Identity crosswalks will be supported after the beta release.

#### Add identity crosswalk

Use identity crosswalks to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. 

TODO add GIF Identity crosswalks screen showing a list of available identity crosswalks with details.

Select **[!UICONTROL Add identity crosswalk]** to see a screen where you can choose from various identity crosswalks that you have previously [imported into Real-Time CDP Collaboration](/help/guide/setup/identity-crosswalk.md#import-crosswalk). Each entry includes details such as the table name, type, description, and creation date.

After selecting the desired crosswalk, use a source field join key to map to the crosswalk table join key. 

>[!NOTE]
>
>After selecting an identity crosswalk, the **[!UICONTROL Add identity crosswalk]** control is greyed out. 

For further reading about identity crosswalks, refer to the [glossary](/help/guide/glossary.md).

-->


<!-- will uncomment this part when Manage use cases part becomes available

### Manage use cases {#manage-use-cases}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_usecases"
>title="Use cases for identities"
>abstract="This control is disabled in the initial release of Real-Time CDP Collaboration"

![Manage use cases screen.](/help/assets/setup/add-manage-audiences/Step-manage-use-cases.png)

For every identity selected in the mapping step, select the use cases that you can use the identity for. Available use cases are: 

* Discover
* Share
* Activate
* Measure

Note that this control is disabled in the initial release of Real-Time CDP Collaboration.

After selecting the desired use cases for each identity, proceed to the next step. 

-->›

### Agendar {#schedule}

Agendar quando começar e terminar de preencher e atualizar os públicos. A associação de público será atualizada de acordo com este agendamento.

![Tela de agendamento mostrando datas de início e término para preencher os públicos.](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

Selecione a taxa de atualização para os públicos-alvo. As opções disponíveis estão entre taxas de atualização de um a seis dias.

>[!IMPORTANT]
>
>Ajustar a frequência de atualizações de público ajudará a gerenciar a [atividade de crédito de Gerenciamento de público-alvo](/help/guide/setup/my-activity.md#types-of-activities), que é calculada por atualização de associação de público-alvo. O impacto disso pode ser a disponibilização de dados menos atualizados para relatórios de descoberta de público-alvo e compartilhamento e ativação de público-alvo.

![Tela de agendamento mostrando intervalos de frequência diferentes para atualizar associação de público-alvo.](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>Após a data de término no intervalo de datas, todos os públicos-alvo importados dessa conexão de dados deixarão de ser atualizados. Para renovar a conexão, vá para [Gerenciar conexão de dados](/help/guide/setup/manage-data-connection.md) e defina uma nova data de término.

### Selecionar públicos-alvo {#select-audience}

Depois de selecionar a origem do público-alvo, você escolherá públicos-alvo específicos para incluir. Use as opções de pesquisa e filtro na página para localizar os públicos relevantes da fonte de dados selecionada.

![Tela Selecionar público-alvo mostrando uma lista de públicos-alvo disponíveis com caixas de seleção para selecioná-los.](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### Revisar

Revise todas as configurações e definições antes de finalizar a adição do público-alvo. Verifique se todos os detalhes estão corretos e selecione **[!UICONTROL Concluído]** para finalizar o processo.

## Exibir painel de públicos-alvo {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Identidades ausentes"
>abstract="A contagem de identidades estará disponível após a próxima atualização da conexão de dados após o agendamento configurado. A atualização inicial geralmente ocorre em 24 horas após a configuração da conexão de dados. Atualizações contínuas seguirão o agendamento configurado. "

Depois de importar públicos para o Real-Time CDP Collaboration, você pode obter informações sobre eles em uma visualização de painel. O modo de exibição padrão na página **[!UICONTROL Meus públicos-alvo]** exibe todos os públicos-alvo atualmente importados pela sua organização para a Real-Time CDP Collaboration.

![Página de visão geral dos públicos-alvo mostrando todos os públicos-alvo importados por um anunciante](/help/assets/setup/add-manage-audiences/audiences-overview.png)

Você pode exibir as seguintes informações relevantes sobre cada público-alvo:

| Item | Descrição |
|----------|---------|
| **[!UICONTROL Identidades]** | Indica o número de identidades presentes nesse público-alvo. Observe que, se o mesmo perfil tiver duas ou mais identidades, e essas identidades forem usadas como chaves de correspondência no projeto, o perfil aparecerá duas vezes na contagem. |
| **[!UICONTROL Status]** | Indica se a audiência está ativa e pode ser usada em projetos. Um status Pendente indica que o público-alvo acabou de ser importado e os membros do público-alvo ainda não foram preenchidos. Os públicos-alvo importados serão preenchidos com perfis após a próxima atualização da conexão de dados após o agendamento configurado. A atualização inicial geralmente ocorre em 24 horas após a configuração da conexão de dados                                         . |
| **[!UICONTROL Source]** | Indica a fonte de onde esse público-alvo foi importado. Na versão atual do Real-Time CDP Collaboration, o Adobe Experience Platform é a única fonte compatível. |
| **[!UICONTROL Conexão de dados]** | Mais informações detalhadas sobre de onde esse público-alvo foi importado. Por exemplo, ao importar públicos da origem do Experience Platform, as sandboxes individuais às quais sua organização tem acesso são consideradas as conexões de dados. |
| **[!UICONTROL Acesso à conexão]** | Define se esse público-alvo é público ou privado. Os públicos-alvo são detectáveis em relatórios de sobreposição e podem ser compartilhados com colaboradores. |
| **[!UICONTROL Criado]** | Indica quando esse público-alvo foi importado para o Real-Time CDP Collaboration. |
| **[!UICONTROL Última atualização]** | Indica a última data e hora em que qualquer aspecto desse público-alvo foi atualizado. |

Selecione **[!UICONTROL Gerenciar conexões de dados]** para exibir e editar todas as conexões de dados configuradas.
Selecione as reticências e **[!UICONTROL Excluir]** para remover o público.
Selecione as reticências e **[!UICONTROL Editar categorias]** para adicionar marcas de categoria diferentes ao público-alvo. Obtenha mais informações na seção [categorias](/#categories) abaixo.
Selecione o nome do público para inspecionar ou editar públicos individuais.

## Exibir públicos-alvo individuais {#view-individual-audiences}

A visualização do público-alvo revela mais informações sobre ele.

![Exibir e inspecionar público-alvo individual.](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

As métricas que você pode visualizar nessa tela estão descritas abaixo:

| Item | Descrição |
|----------|---------|
| **[!UICONTROL Status]** | Indica se a audiência está ativa e pode ser usada em projetos. |
| **[!UICONTROL Source]** | Indica a fonte de onde esse público-alvo foi importado. Na versão atual do Real-Time CDP Collaboration, o Adobe Experience Platform é a única fonte compatível. |
| **[!UICONTROL Conexão de dados]** | Mais informações detalhadas sobre de onde esse público-alvo foi importado. Por exemplo, ao importar públicos da origem do Experience Platform, as sandboxes individuais às quais sua organização tem acesso são consideradas as conexões de dados. |
| **[!UICONTROL Última atualização]** | Indica a última data e hora em que qualquer aspecto desse público-alvo foi atualizado. |
| **[!UICONTROL Última atualização por]** | Indica o usuário que atualizou esse público pela última vez. |
| **[!UICONTROL Criado]** | Indica quando esse público-alvo foi importado para o Real-Time CDP Collaboration. |
| **[!UICONTROL Criado por]** | Indica o usuário que importou o público-alvo para o Real-Time CDP Collaboration. |


Você pode usar mais dois controles na página para editar ou remover públicos:

* **[!UICONTROL Excluir]**: remover o público-alvo do inventário
* **[!UICONTROL Editar]**: edite os metadados do público-alvo como seu nome ou descrição.

![Exibir e inspecionar público-alvo individual.](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

Mais informações sobre o público estão disponíveis e parcialmente editáveis nos widgets abaixo:

![Exibir e inspecionar público-alvo individual.](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [Identidades](#identities)
* [Categorias](#categories)
* [Acesso à conexão](#connection-access)
* [Visibilidade de metadados](#metadata-visibility)

### Identidades {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identidades"
>abstract="Obtenha uma visualização detalhada das identidades que compõem esse público-alvo, bem como uma contagem total de perfis com as respectivas identidades."

Esta seção indica o número de perfis presentes no público com qualquer uma das identidades especificadas ao importar os públicos. A seção também contém um detalhamento de identidade para que você possa saber quais identidades compõem a maioria da população do público-alvo.

### Categorias {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Categorias"
>abstract="Adicione tags aos públicos-alvo para facilitar a organização, a filtragem e a recuperação. Você pode marcar um público-alvo com várias categorias e então usar essas tags de categoria para filtrar os públicos-alvo desejados em outras áreas do produto."

Para facilitar a organização, a filtragem e a recuperação de públicos-alvo, você pode marcar seus públicos-alvo. Você pode marcar um público com várias categorias e usar essas marcas de categoria para filtrar os públicos desejados na área de produto [descoberta](/help/guide/collaborate/discover.md), ao executar relatórios de sobreposição de público.

### Acesso à conexão {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Acesso à conexão"
>abstract="<p>Os públicos-alvo podem ser de três tipos: públicos, privados e personalizados.</p><p> Sua disponibilidade para uso em projetos com colaboradores difere com base na configuração de acesso à conexão. É sempre possível alterar o acesso à conexão de privado para público, mas não será permitido retornar à configuração anterior a partir do momento que um público-alvo for compartilhado com os colaboradores.</p>"

Selecione se o público-alvo deve ser privado para você ou utilizável e detectável em conexões. As três opções disponíveis são:

* **[!UICONTROL Público]**. Esses públicos-alvo estão disponíveis para uso em relatórios de sobreposição e para compartilhamento e ativação em conexões com qualquer colaborador.
* **[!UICONTROL Público-alvo]**. Estes públicos-alvo *não* estão disponíveis para uso em relatórios de sobreposição e para compartilhamento e ativação em conexões com qualquer colaborador. Embora não esteja disponível para os colaboradores visualizarem ou usarem, a população deste público-alvo ainda contribui para a população total na exibição **[!UICONTROL Todos os públicos-alvo]** na [seção de descobertas e sobreposições](/help/guide/collaborate/discover.md#compare-audiences). Altere a configuração para público ou personalizado para usar os públicos-alvo em conexões com colaboradores.
* **[!UICONTROL Público-alvo personalizado]**. Esses públicos-alvo estão disponíveis para uso em relatórios de sobreposição e para compartilhamento e ativação somente em conexões especificadas. Embora não esteja disponível para todos os colaboradores visualizarem ou usarem, a população deste público-alvo ainda contribui para a população total na exibição **[!UICONTROL Todos os públicos-alvo]** da seção [descobrir e sobrepor](/help/guide/collaborate/discover.md).

>[!IMPORTANT]
>
>Independentemente do status de acesso (público, privado ou personalizado), a população de qualquer público-alvo contribui para a população de **[!UICONTROL Todos os públicos-alvo]** na exibição de análise de sobreposição da Descoberta de público-alvo. <br> ![O público-alvo **Todos os públicos-alvo** gerados pelo sistema na análise de sobreposição da Descoberta de Público-alvo inclui os públicos-alvo com todos os status de acesso de conexão (público, privado, personalizado).](/help/assets/setup/add-manage-audiences/all-audiences-view.png "O público-alvo **Todos os públicos-alvo** gerado pelo sistema na análise de sobreposição **Descoberta de Público-alvo** inclui os públicos-alvo com todos os status de acesso de conexão (público, privado, personalizado)."){width="100" zoomable="yes"}

A disponibilidade do público-alvo para uso em projetos com colaboradores é diferente de acordo com a configuração de acesso à conexão. É sempre possível alterar o acesso à conexão de privado para público, mas não será permitido retornar à configuração anterior a partir do momento que um público-alvo for compartilhado com os colaboradores.

### Visibilidade de metadados {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Visibilidade de metadados"
>abstract="<p>Indica quais das informações de metadados de público-alvo estão visíveis para outras organizações antes de elas se conectarem com a sua organização. </p> <p> A **contagem de identidades** controla se o seu parceiro pode exibir contagens de identidades dos seus públicos-alvo ao visualizar relatórios de sobreposição na guia de descoberta. A **% de sobreposição de público-alvo** controla se os colaboradores podem descobrir as porcentagens de sobreposição entre os públicos-alvo deles e os seus."

>[!NOTE]
>
>Se o colaborador tiver todos os públicos definidos como privados, a exibição **[!UICONTROL Públicos relevantes]** nos insights do público-alvo estará em branco. [Leia mais](/help/guide/collaborate/discover.md#relevant-audiences).

Indica qual das informações de metadados de público-alvo é visível para outras organizações antes que elas se conectem com a organização ou em diferentes visualizações de projeto.

**[!UICONTROL Mostrar contagem de identidades]**: esta configuração controla se o parceiro pode exibir contagens de identidades para os públicos-alvo ao [exibir relatórios de sobreposição na guia de descoberta](/help/guide/collaborate/discover.md#discover-overlaps).

![Imagens lado a lado com a opção mostrar contagem de identidades desmarcada e selecionada.](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL Mostrar sobreposição de público-alvo %]**: quando definido como verdadeiro, os colaboradores podem [descobrir porcentagens de sobreposição](/help/guide/collaborate/discover.md#compare-audiences) entre seus públicos-alvo e o público que pertence a você. Por exemplo, na gravação abaixo, o público-alvo `agora-advertiser-aud3` tem essa configuração definida como verdadeira e um colaborador pode visualizar porcentagens de sobreposição com esse público-alvo. A audiência `agora-advertiser-aud1` tem essa configuração definida como falsa, portanto, o colaborador não pode exibir porcentagens de sobreposição.

![Percentual de sobreposição de público-alvo para dois públicos-alvo diferentes.](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## Próximas etapas

Depois de importar públicos, use a seção [Conectar](/help/guide/connect/establishing-connections.md) para descobrir editores para se conectar e começar a colaborar em projetos.
