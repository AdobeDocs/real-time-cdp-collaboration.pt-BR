---
title: Configurar [!DNL Google Cloud Storage] para fornecimento de exposição de anúncios
description: Saiba como conectar um bucket do [!DNL Google Cloud Storage] como uma fonte de log de anúncios de autoatendimento para exposições de anúncios na medição do Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 02f344c9fcfff20c84c2e92b5aa4647829dd5d2f
workflow-type: tm+mt
source-wordcount: '1712'
ht-degree: 2%
---

# Configurar [!DNL Google Cloud Storage] para fornecimento de exposição de anúncios

Conecte seu bucket do [!DNL Google Cloud Storage] (GCS) ao Adobe Real-Time CDP Collaboration para obter dados de exposição de publicidade (log de anúncios) para medição.

O módulo de Medição no Real-Time CDP Collaboration conecta os dados de conversão do anunciante aos logs de exposição dos anúncios do editor para fornecer relatórios de campanha centrados em privacidade. Isso adiciona um caminho sem código e de autoatendimento para anunciantes e editores. Você pode incluir os logs de exposição (impressão) dos anúncios que já mantém no [!DNL Google Cloud Storage] na Medição para atribuição, sem uma dependência do Adobe Experience Platform. Você conecta um bucket, confirma se os dados detectados correspondem ao esquema de log de anúncios esperado pela Avaliação e conclui o processo em minutos.

Os dados não são obtidos no momento da conexão. A origem é disparada quando você executa um relatório de medição. Para minimizar o armazenamento, a Adobe exclui automaticamente os registros de anúncios de origem após um período de retenção de sete dias.

As regras de governança e de tratamento de dados para logs de anúncios originados de [!DNL Google Cloud Storage] correspondem às regras que se aplicam aos dados originados no Adobe Experience Platform.

>[!NOTE]
>
>Este guia aborda o fornecimento de anunciantes e editores **logs de anúncios** (exposições de anúncios) do armazenamento na nuvem. A obtenção de dados de conversão do armazenamento na nuvem será adicionada em breve.

## Pré-requisitos {#prerequisites}

Conclua todos os itens desta seção antes de iniciar o fluxo de trabalho de configuração. Antes de seguir este guia, você deve ter concluído a integração e a configuração da [conta](./onboard-account.md).

### Acesso e permissões do GCS {#gcs-access-permissions}

Você ou o administrador do [!DNL Google Cloud] deve conceder ao Adobe acesso somente leitura ao seu bucket de GCS antes de iniciar o assistente. Para obter instruções passo a passo, consulte [Configurar permissões do Google Cloud Storage](#setup-gcs-permissions).


### Preparar os dados do registro de anúncios {#prepare-adlog-data}

Seus arquivos de log de anúncios devem estar em conformidade com o [esquema de log de anúncios](#ad-log-schema) antes do início do fornecimento. Os principais requisitos incluem:

* **Formato de arquivo:** somente CSV.
* **Cabeçalhos de coluna canônicos:** Os arquivos devem usar os cabeçalhos de coluna canônicos definidos no [esquema de log de anúncios](#ad-log-schema). Esta versão não oferece suporte ao remapeamento por coluna ou ao mapeamento de esquema automatizado.
* **Campos obrigatórios:** todos os campos obrigatórios devem estar presentes, juntamente com pelo menos uma chave de correspondência.
* **Hash de chave de correspondência:** valores de hash de chave de correspondência devem ser SHA-256 hexadecimal em minúsculas.
* **Consistência de coluna:** todos os arquivos no caminho configurado devem compartilhar um layout de coluna idêntico.
* **Subpastas:** os arquivos devem ficar diretamente no caminho especificado. O Collaboration não percorre subpastas.

## Conectar logs de anúncios no assistente {#connect-adlogs}

Use as etapas a seguir para conectar seus logs de anúncio do GCS de dentro do Collaboration.

1. No espaço de trabalho **[!UICONTROL Configuração]**, selecione **[!UICONTROL Meus dados de medição]**, selecione o ícone adicionar e escolha **[!UICONTROL Dados de medição]**.

   ![O espaço de trabalho de Instalação na guia Meus dados de medição, mostrando o ícone de adição e a opção Dados de medição no menu.](../../assets/setup/gcs-adlog-sourcing/add-measurement-data-entry-point.png){zoomable="yes"}

2. No fluxo de trabalho **[!UICONTROL Adicionar dados de medição]**, selecione **[!UICONTROL Exposições da Advertising]** como seu tipo de dados de medição e selecione **[!UICONTROL Avançar]**.

   ![O fluxo de trabalho Adicionar dados de medição que mostra a seleção do tipo de dados de medição, com Exposições Advertising selecionadas.](../../assets/setup/gcs-adlog-sourcing/select-adlog-data-type.png){zoomable="yes"}

3. Para importar os dados de medição, selecione **[!UICONTROL Adicionar nova conexão de dados]** e **[!UICONTROL Avançar]**.

   ![O fluxo de trabalho Adicionar dados de medição mostrando a etapa de seleção da conexão de dados, com a opção Adicionar uma nova conexão de dados selecionada.](../../assets/setup/gcs-adlog-sourcing/add-new-data-connection.png){zoomable="yes"}

4. Escolha a fonte de dados para sua nova conexão de dados: **[!UICONTROL Google Cloud Storage]**. Selecione **[!UICONTROL Próximo]**.

   ![O fluxo de trabalho Adicionar dados de medição que mostra a etapa de seleção da fonte de dados, com as opções Google Cloud Storage, Azure Blob Storage, Azure Data Lake Storage Gen 2 e Google Cloud Storage selecionadas.](../../assets/setup/gcs-adlog-sourcing/gcs-adlog-source-selection.png){zoomable="yes"}

5. O assistente **[!UICONTROL Adicionar conexão de dados]** é aberto. Na etapa **[!UICONTROL Conectar o Google Cloud Storage]**, forneça o **[!UICONTROL Bucket]** e o **[!UICONTROL Path]** onde seus arquivos de log de anúncios residem. Ambos os campos são obrigatórios e todos os arquivos no caminho configurado são tratados como um conjunto de dados.

   ![O assistente para Adicionar conexão de dados na etapa Conectar Armazenamento em Nuvem da Google, mostrando os campos Bucket e Path necessários.](../../assets/setup/gcs-adlog-sourcing/gcs-adlog-connection-details.png){zoomable="yes"}

6. Na etapa **[!UICONTROL Nome e descrição]**, forneça um **[!UICONTROL Nome da conexão de dados]** necessário e uma **[!UICONTROL Descrição]** opcional para a conexão de dados.

   ![A etapa Nome e Descrição, mostrando os campos Nome e Descrição da conexão de dados.](../../assets/setup/gcs-adlog-sourcing/gcs-adlog-name-description.png){zoomable="yes"}

7. Na etapa **[!UICONTROL Mapear campos]**, visualize as colunas detectadas para confirmar se o assistente leu os arquivos corretos e revise o [esquema de log de anúncios](#ad-log-schema), que lista todos os campos que a medição entende, quais campos são obrigatórios versus opcionais e quais colunas detectadas são reconhecidas como chaves de identidade/correspondência. Esta etapa é uma validação somente leitura: o sistema confirma que os cabeçalhos obrigatórios estão presentes e bloqueia se um campo obrigatório estiver ausente. Não há remapeamento por coluna nesta versão.

   ![A etapa Mapear campos mostrando a visualização das colunas detectadas e a revisão do esquema do log de anúncios.](../../assets/setup/gcs-adlog-sourcing/gcs-adlog-map-fields.png){zoomable="yes"}

8. Na etapa **[!UICONTROL Revisar]**, revise e conclua. A conexão aparece na área de dados de medição com seu status, que permanece **pendente** até que o primeiro relatório de medição execute os dados das fontes de dados.

## Como funciona o fornecimento de log de anúncio {#how-it-works}

O fornecimento de log de anúncio de [!DNL Google Cloud Storage] espelha o fluxo de alto nível usado para fornecimento de público:

1. **Conexão de armazenamento na nuvem:** você configura o acesso somente leitura a um compartimento que armazena seus logs de anúncios.
2. **Revisão e validação de esquema:** o sistema valida seus arquivos em relação ao esquema de log de anúncios (verificações de pasta, arquivo e cabeçalho necessário; somente leitura).
3. **Mapeamento de campos:** os campos de identidade de origem são mapeados automaticamente para campos canônicos com base nos nomes de coluna canônicos. Não há remapeamento manual.
4. **Assimilação e normalização:** eventos são normalizados para uma linha por exposição. A origem do log de anúncio é iniciada quando você executa um relatório de medição.

### Esquema de log de anúncios (formato CSV canônico) {#ad-log-schema}

Os campos obrigatórios devem estar presentes e pelo menos um campo marcado como **Chave de Junção (um dos obrigatórios)** na tabela a seguir também deve estar presente. Os valores de hash de chave correspondentes são SHA-256 hexadecimal em minúsculas.

| Campo | Tipo de dados | Obrigatório | Descrição |
| --- | --- | --- | --- |
| `EVENT_DATETIME` | String (ISO 8601) | Obrigatório | Carimbo de data e hora do evento |
| `EVENT_ID` | String | Opcional | Identificador exclusivo do evento |
| `EVENT_TYPE` | String (enumeração) | Obrigatório | Tipo de evento. Um de `{impression, click}` |
| `HASHED_EMAIL_SHA_256` | Cadeia de caracteres (hexadecimal de 64 caracteres) | Chave de associação (uma das necessárias) | SHA-256 hexadecimal minúsculo do email |
| `HASHED_IPV4_SHA_256` | Cadeia de caracteres (hexadecimal de 64 caracteres) | Chave de associação (uma das necessárias) | SHA-256 hexadecimal em minúsculas de IPv4 |
| `DEVICE_ID` | Cadeia de caracteres (hexadecimal de 64 caracteres) | Chave de associação (uma das necessárias) | ID de anúncio do dispositivo |
| `DEVICE_ID_TYPE` | String (enumeração) | Opcional | Um de `{idfa, gaid, aaid, rida, afai, msai, vida, lgudid, tifa}` |
| `ECID` | Cadeia de caracteres (hexadecimal de 64 caracteres) | Chave de associação (uma das necessárias) | ECID baseado em Demdex |
| `CUSTOM_ID` | String | Opcional | ID persistente de editor/parceiro (por exemplo, PPID, RampID, Core ID) |
| `ADVERTISER_ID` | String | Obrigatório | Identificador exclusivo do anunciante |
| `ADVERTISER_NAME` | String | Opcional | Anunciante/nome da marca |
| `CAMPAIGN_ID` | String | Obrigatório | Identificador de campanha específico da plataforma |
| `CAMPAIGN_NAME` | String | Opcional | Nome de campanha legível |
| `PLACEMENT_ID` | String | Obrigatório | Identificador exclusivo do posicionamento |
| `PLACEMENT_NAME` | String | Opcional | Nome do posicionamento descritivo |
| `CREATIVE_ID` | String | Opcional | Identificador exclusivo do criativo do anúncio |
| `CREATIVE_NAME` | String | Opcional | Nome criativo legível |
| `AUDIENCE_ID` | String | Opcional | Identificador de segmento de público |
| `AUDIENCE_NAME` | String | Opcional | Nome de público legível |
| `DEVICE_TYPE` | String (enumeração) | Opcional | Um de `{mobile, desktop, tablet, ctv, dooh, car, in_store, other}` |
| `AD_FORMAT` | String (enumeração) | Opcional | Um de `{display, video, native, audio, search, commerce, dooh, other}` |
| `SITE_NAME` | String | Opcional | Propriedade de rede/site/aplicativo/editor em que ocorreu a impressão |
| `TEST_GROUP` | String | Opcional | Agrupamento para estudos de elevação, teste/controle, grupos de controle |
| `CUSTOM_DIM` | String | Opcional | Dimensão adicional do editor |

{style="table-layout:auto"}

>[!NOTE]
>
>`MATCH_KEY_TYPE` está incluído como um campo opcional no esquema para que, com o tempo, vários tipos de ID possam ser aceitos em paralelo e a origem da chave de correspondência (email, telefone ou CRM) possa ser preservada sem romper o contrato v1.

### Requisitos de validação (v1) {#validation-requirements}

O sistema valida e registra os dados de origem antes de você concluir o fluxo de trabalho de configuração. Verificações de validação:

* A pasta de origem deve conter pelo menos um arquivo.
* Os arquivos não podem estar vazios.
* Os cabeçalhos de esquema obrigatórios devem estar presentes.
* Campos de esquema opcionais podem ser omitidos.
* Os arquivos que contêm apenas os campos obrigatórios são válidos.

As falhas de validação impedem que você continue. O sistema **não** valida tipos de dados, valores de campo, integridade de registro, qualidade de dados ou mapeamento de esquema automatizado. A validação está limitada às verificações de pasta, arquivo e cabeçalho necessárias para esta versão inicial.

## Limitações conhecidas {#known-limitations}

Esteja ciente das seguintes restrições ao configurar e usar o [!DNL Google Cloud Storage] ad log sourcing:

* **Somente logs de anúncios:** Essa conexão origina logs de anúncios de anunciantes ou editores (exposições de anúncios). Os dados de conversão ainda não são suportados.
* **Fontes com suporte:** [!DNL Google Cloud Storage] e [!DNL Azure Data Lake Storage] ou [!DNL Azure Blob Storage].
* **Formato de arquivo:** somente CSV.
* **Cabeçalhos canônicos necessários:** Não há remapeamento por coluna e nenhum mapeamento inteligente/automatizado nesta versão. Seus arquivos devem usar os nomes de coluna canônicos.
* **Nenhuma validação de valor/tipo:** Somente os cabeçalhos de coluna necessários são validados. Inicialmente, pode não haver linhas de dados.
* **Não editar uma conexão após a criação:** Qualquer alteração, incluindo a alteração das chaves de correspondência ativas, requer a criação de uma nova conexão.
* **Um layout por caminho:** Todos os arquivos no caminho devem compartilhar um layout de coluna idêntico. Layouts mistos podem causar falhas de fornecimento parcial.
* **Subpastas não percorridas:** os arquivos devem ficar localizados diretamente no caminho especificado.
* **Nenhum agendamento ou retrospectiva na configuração:** A fonte de log de anúncios começa quando você executa um relatório de medição. Defina o período de retrospectiva ao configurar o relatório.
* **Uma conexão de dados de log de anúncios:** Configure apenas uma conexão de dados de log de anúncios por vez. Os relatórios de medição usam automaticamente a conexão configurada.

## Solução de problemas {#troubleshooting}

* **A conexão mostra dados pendentes / sem dados:** Isso é esperado até que o primeiro relatório de medição seja executado. Nenhum dado é originado no momento da conexão.
* **&quot;Nenhum dado encontrado&quot; na etapa de origem:** A pasta está vazia. Adicione arquivos antes de continuar.
* **A visualização não mostra nenhuma coluna:** O arquivo está presente, mas vazio (sem cabeçalhos ou conteúdo).
* **Não é possível obter validação passada:** Um cabeçalho de coluna obrigatório está ausente. Confirme se os campos obrigatórios e pelo menos uma chave de correspondência estão presentes, usando nomes canônicos.
* **Colunas não reconhecidas:** Nomes de colunas não canônicas não são selecionados como campos conhecidos. Renomeie-os para o formato canônico; não há remapeamento nesta versão.
* **A origem falha após a configuração:** Confirme se o acesso de leitura do Adobe ao bucket não foi alterado e se os arquivos ainda existem no caminho configurado no formato canônico.
* **Intervalo de datas do relatório não totalmente coberto:** Lembre-se da expiração automática de dados de 7 dias. Logs com mais de 7 dias podem não estar disponíveis para o intervalo solicitado.

## Configurar [!DNL Google Cloud Storage] permissões {#setup-gcs-permissions}

Para permitir que o Adobe leia a partir do seu bucket de GCS, crie uma função IAM personalizada com as seguintes permissões:

| Permissão | Finalidade |
| ------------- | --------------- |
| `storage.buckets.get` | Metadados do bucket de leitura. |
| `storage.objects.get` | Ler dados e metadados do objeto. |
| `storage.objects.list` | Listar objetos em um bucket. |

{style="table-layout:auto"}

Conceda essa função personalizada à Conta de Serviço do Adobe Google de sua região (NA, EMEA ou Austrália). A conclusão desta configuração requer privilégios de **Administrador da Conta da Google Cloud**.

## Considerações sobre atualização ou migração {#upgrade-migration}

* Os clientes que antes eram integrados por meio da Experience Platform ou da configuração assistida pela Adobe podem migrar para o caminho de armazenamento na nuvem de autoatendimento. Os relatórios e fluxos de medição existentes permanecem inalterados.
* As chaves de correspondência presentes nos arquivos de log de anúncios devem ser habilitadas para a conta do Collaboration, assim como no fornecimento de público-alvo.
* As regras de governança e manuseio de dados correspondem aos dados obtidos do Experience Platform.

## Próximas etapas {#next-steps}

Depois que a origem for concluída, os logs de anúncios estarão disponíveis para os relatórios de medição.

Para outros métodos de fornecimento de exposição de anúncios, consulte [Configurar armazenamento do Azure para fornecimento de exposição de anúncios](./configure-azure-adlog-sourcing.md).
