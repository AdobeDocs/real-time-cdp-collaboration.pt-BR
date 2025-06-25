---
title: Início rápido de integração do Real-Time CDP Collaboration
description: Saiba como integrar sua organização ao Real-Time CDP Collaboration, incluindo a configuração de funções e organizações, o provisionamento de público-alvo, a ativação e a medição. Este guia ajuda anunciantes e editores a definir as configurações de colaboração e começar a usar públicos-alvo compartilhados de forma segura e eficiente.
audience: admin, publisher, advertiser
source-git-commit: 4435788917dd82cb127525e054f7f09803e1dcdf
workflow-type: tm+mt
source-wordcount: '1595'
ht-degree: 0%

---

# Início rápido da integração do Real-Time CDP Collaboration

Comece a usar o Real-Time Customer Data Platform (CDP) Collaboration configurando sua organização, provisionando públicos e habilitando a ativação e a medição com foco em privacidade.

## Pré-requisitos

Antes de começar, verifique se você tem o seguinte:

- Uma licença ativa do Real-Time CDP Collaboration.
- [Acesso de administrador de sistema ou de produto ao Adobe Experience Platform](./permissions/overview.md#use-cases).
- [Acesso provisionado para usuários finais](./permissions/manage-user-access.md).
- [Funções criadas para sua organização e atribuídas a usuários](./permissions/manage-roles.md).
- Acesso aos ativos de marca, como nome, logotipo e banner da sua organização.
- Uma [estratégia de chave de correspondência definida](./setup/onboard-organization.md#set-up-match-keys) (no momento, o email com hash é a única chave de correspondência com suporte).
- (Opcional) Acesse uma origem na nuvem compatível (Amazon S3 ou Snowflake) se não estiver usando o Experience Platform como destino.

## Etapa 1: concluir configuração baseada em função {#complete-role-based-setup}

>[!NOTE]
>
>Essa etapa se aplica a anunciantes e editores.

As funções de acesso da sua organização determinam o que os usuários podem ver e fazer no Real-Time CDP Collaboration. Antes de continuar, verifique se as permissões baseadas em função estão configuradas corretamente para garantir o acesso e a visibilidade apropriados na plataforma.

**Recursos:**

- [Documentação de acesso do usuário](./permissions/manage-user-access.md)
- [Documentação de configuração de função](./permissions/manage-roles.md)


Assista a este vídeo para saber como atribuir acesso e permissões de produto ao Collaboration usando a interface do usuário do Admin Console e do Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## Etapa 2: configurar sua organização da Real-Time CDP Collaboration {#set-up-your-organization}

>[!NOTE]
>
>Essa etapa se aplica a anunciantes e editores.

Antes de adicionar públicos, é necessário configurar sua organização no Collaboration. Isso controla como sua organização aparece e se comporta na interface.

Se você não tiver acesso de administrador ao Experience Platform, entre em contato com o administrador da organização para obter ajuda para concluir essa configuração.

Defina a função da sua organização na Collaboration, forneça ativos de marca e configure chaves de correspondência para alinhar públicos-alvo em todas as conexões. Em seguida, conclua as etapas abaixo para finalizar a configuração e preparar sua organização para se envolver com suas conexões.

>[!NOTE]
>
>Você pode criar um ou mais colaboradores (como anunciantes ou editores) durante a configuração. Determinados campos, como ativos de marca e email de contato, podem ser atualizados posteriormente no espaço de trabalho **[!UICONTROL Configurações]**. As teclas correspondentes podem ser removidas no nível do projeto, mas não adicionadas. Portanto, planeje-as cuidadosamente.

- **Atribuir uma função** - Determina se sua organização atua como anunciante, editor ou ambos. Sua função define quais recursos de colaboração você tem, como iniciar o compartilhamento de público-alvo (anunciante) ou disponibilizar públicos-alvo (editor). Para saber mais sobre como as funções afetam o fluxo de trabalho de colaboração, consulte o [Guia completo do fluxo de trabalho](./end-to-end-workflow.md).
- **Ativos de marca** - Adicione o seguinte à sua conta:
   - Nome da marca (máximo de 100 caracteres)
   - Descrição da marca (máximo de 1.000 caracteres)
   - Logotipo da marca (SVG &lt;20KB, idealmente quadrado)
   - Banner da marca (JPG 2688x1536 ou semelhante)
- **Email de contato** - Forneça um email comercial para que os colaboradores usem depois que uma conexão for estabelecida.

  >[!NOTE]
  >
  >Se você estiver criando uma conta de editor e quiser que o seja exibido publicamente no catálogo de conexões da Collaboration, entre em contato com o representante de conta da Adobe. As contas do editor exigem um banner de marca personalizado (JPG 2688x1536); esse arquivo pode ser compartilhado diretamente com o representante.

- **Configurar chaves de correspondência** - Selecione os identificadores usados para correspondência de público-alvo (atualmente, o email com hash é a única chave de correspondência com suporte).

Depois que sua organização for criada e suas chaves de correspondência e identidade visual forem configuradas, sua organização estará pronta para começar a provisionar públicos e ativar dados.

Para saber mais sobre a configuração inicial da organização, incluindo como definir funções, carregar ativos de marca e configurar chaves de correspondência, consulte o [documento de configuração inicial da organização](./setup/onboard-organization.md#initial-organization-setup){target="_blank"}.

Assista a uma apresentação passo a passo da configuração do anunciante, incluindo criação de conta, marca e configuração principal de correspondência.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## Etapa 3: públicos-alvo da Source (do Experience Platform ou de uma fonte na nuvem) {#source-audiences}

Escolha um ou ambos os armazenamentos de dados a seguir para originar públicos-alvo. Use a interface do usuário do Collaboration ou coordene com a Adobe para provisionar públicos-alvo em um formato com preservação da privacidade.

### Opção A: Source do Experience Platform

[Use a interface do usuário de destinos do Collaboration para vincular uma sandbox que contenha públicos](./setup/onboard-audiences.md). Use esse método de autoatendimento para fazer referência a segmentos de público-alvo existentes na sua instância do Experience Platform.

### Opção B: Source do Snowflake ou Amazon S3

Para configurar uma fonte de nuvem (por exemplo, [!DNL AWS S3] ou [!DNL Snowflake]), prepare os dados do público-alvo usando a seguinte [PDF de Especificação de Público-Alvo](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf). Depois de concluir, ou em caso de dúvidas, entre em contato com o representante de conta da Adobe para finalizar a configuração. Este método não é de autoatendimento e requer a assistência da Adobe.

>[!IMPORTANT]
>
>Os arquivos de público-alvo baseados em nuvem devem seguir o esquema necessário descrito na PDF de especificação de público-alvo. Os arquivos devem incluir identificadores com hash (SHA256 em letras minúsculas), campos de metadados obrigatórios como `segment_name` e `activation_id` e usar formatos compatíveis como CSV ou Parquet. O Adobe não normaliza dados antes da ativação. O TTL é aplicado com base na duração do público-alvo.
>
>Todos os públicos-alvo no arquivo carregado são totalmente originários nesse estágio. O acesso a organizações parceiras específicas é provisionado separadamente por meio da interface do usuário do Collaboration.

### Provisionar públicos-alvo

Configure como os públicos-alvo são preparados, combinados e controlados para uso em conexões.

- **Selecionar públicos-alvo** *(somente Experience Platform)* - Escolha segmentos de público-alvo com identificadores compatíveis.
- **Mapear chaves de correspondência** - Alinhar campos de público-alvo com as chaves de correspondência configuradas.
- **Aplicar transformações** - Hash valores de texto sem formatação (por exemplo, email), se necessário.
- **Atualizações de agendamento** - Defina a frequência de atualização (por exemplo, diariamente).
- **Definir configurações de consentimento** - Determine quais perfis estão qualificados para serem incluídos em conexões selecionando um modo de consentimento: aceitação, recusa ou nenhum.

>[!NOTE]
>
>Você pode adicionar ou remover públicos e atualizar o agendamento de atualização diretamente na interface do usuário do Collaboration. Para alterar outras configurações, como chaves de correspondência ou modo de consentimento, você deve excluir e recriar a conexão de dados.

>[!IMPORTANT]
>
>**Número máximo de públicos-alvo por função de colaborador:**
>
>- **Os anunciantes** podem provisionar até 25 públicos-alvo.
>- **Os editores** podem provisionar até 250 públicos-alvo (cada um com no mínimo 5.000 IDs).

>[!IMPORTANT]
>
>**Corresponder requisitos de chave:**
>
>Todas as chaves de correspondência devem ser **cortadas**, **em minúsculas** e **SHA256-com hash**.\
>Se você fornecer valores com hash que usam caracteres em maiúsculas, o Collaboration os converterá automaticamente em minúsculas.\
>Se sua origem contiver **identificadores de texto sem formatação**, use a opção **[!UICONTROL Aplicar transformação]** na interface para aplicar o hash. Essa opção só está disponível ao fornecer públicos-alvo do Experience Platform e não tem suporte para fontes baseadas em nuvem.
>
>Para obter mais informações, consulte a seção [mapear campos](./setup/onboard-audiences.md#map-fields) do guia de importação e gerenciamento de públicos.

Para ver uma apresentação completa de como fazer referência a públicos-alvo usando a interface do usuário do Collaboration, assista ao vídeo de demonstração Referência de público-alvo da Collaboration abaixo.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

Como alternativa, consulte o documento sobre [como disponibilizar públicos-alvo no Real-Time CDP Collaboration](https://experienceleague.adobe.com/pt-br/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#import-audiences).

## Etapa 4: ativar públicos-alvo (para Experience Platform ou um destino de nuvem) {#activate-audiences}

>[!NOTE]
>
>Essa etapa se aplica a anunciantes e editores.

Use a interface do usuário do Collaboration para ativar públicos-alvo para sua instância do Experience Platform ou um destino de nuvem.

### Opção A: Ativar para o Experience Platform

Conclua as etapas a seguir descritas no guia [Configurar o Adobe Experience Platform como destino](https://experienceleague.adobe.com/pt-br/docs/real-time-cdp-collaboration/using/destinations/experience-platform).

- **Criar um destino** - Use a interface do usuário para configurar um destino do Experience Platform (nível de sandbox).
- **Mapear chaves de correspondência** - Selecione o identificador (por exemplo, `hashedEmail`).
- **Definir TTL** - Definir expiração (1-30 dias).
- **Verificar no Audience Portal** - Depois que um colaborador enviar um público-alvo para você, verifique se ele aparece no Audience Portal sob a origem &quot;[!UICONTROL Real-Time CDP Collaboration].&quot;

### Opção B: Ativar para nuvem

Para ativar públicos-alvo para um destino de nuvem (como [!DNL AWS S3] ou [!DNL Snowflake]), entre em contato com o representante de conta da Adobe para iniciar o processo de configuração. Você precisará fornecer detalhes de destino, como caminho do arquivo, credenciais e formato de arquivo esperado. Durante a instalação, você também deve especificar uma chave de correspondência (por exemplo, `hashedEmail`) e definir o TTL desejado e a cadência de atualização. Quando a configuração for concluída, a Adobe fornecerá o destino e garantirá que os dados sejam entregues corretamente.

Os dados de público-alvo enviados para um destino de nuvem seguem um esquema predefinido. Para obter uma descrição detalhada dos campos e formatos necessários, baixe o [Guia do Collaboration Audience Activation](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

### Principais diferenças

A lista a seguir destaca as diferenças entre as opções de ativação do Experience Platform e da nuvem:

- As ativações para o Experience Platform são totalmente de autoatendimento e visíveis no Portal de público-alvo.
- Os destinos em nuvem exigem coordenação do Adobe e não estão visíveis na interface do usuário.

## Etapa 5: configurar medição (opcional) {#set-up-measurement}

>[!AVAILABILITY]
>
>Este recurso está na **beta** e está disponível exclusivamente para clientes no programa de Disponibilidade Limitada. Entre em contato com seu representante da Adobe para solicitar acesso.

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Medida]** só estará disponível se o caso de uso **[!UICONTROL Medida]** tiver sido habilitado [durante o processo de conexão](./connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./collaborate/manage-projects.md#project-use-cases).

O Collaboration oferece vários relatórios para analisar o alcance, a frequência e a eficácia da campanha. Embora o espaço de trabalho **[!UICONTROL Medida]** esteja disponível na interface do usuário, a funcionalidade completa de relatórios pode exigir a habilitação do back-end.

Para saber como exibir e interpretar relatórios de medição, consulte o [Guia de medição](./collaborate/measure.md). Ele abrange atribuição, métricas de resumo da campanha e painéis, como curvas de alcance e distribuição de frequência.

<!-- Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."
### Configure measurement workflow

Collaboration supports two measurement workflows:

- **Attribution using Adobe Experience Platform datasets**
- **Campaign summary using only partner-provided data**

Choose the appropriate workflow below based on your campaign measurement goals.

#### Option A: Attribution using Experience Platform datasets

Use this workflow to measure conversion activity using datasets stored in Experience Platform.

1. **Create a measurement data connection**
   - Select the dataset that contains your conversion events.
   - Map identity fields from your dataset to the match keys used in Collaboration.
   - Manage consent and governance settings.
   - Define one or more conversion events to measure.
   - Review and confirm your setup.

2. **Run a measurement report**
   - Go to the **[!UICONTROL Measure]** workspace within the associated project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Attribution]** as the report type.
   - Select the defined conversion event(s).
   - Submit the report. It will run on the specified date and populate within 24 hours.

#### Option B: Campaign summary using partner-provided data

Use this workflow to generate campaign summary insights based on advertiser-supplied identifiers (for example, campaign ID).

1. **Set up the connection**
   - In the connection settings, ensure **[!UICONTROL Measurement]** is selected as a use case.
   - Create a project under the connection with **[!UICONTROL Measurement]** as an activity.

2. **Provide campaign context**
   - Input required campaign identifiers (for example, **Campaign ID**) for the partner to reference.
   - Align with your partner on campaign scope and reporting timeline.

3. **Run a measurement report**
   - Navigate to the **[!UICONTROL Measure]** workspace within the project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Campaign summary]** as the report type.
   - Submit the report. It will run on the selected date and populate within 24 hours. -->

## Verificação

Após a ativação, verifique se os públicos-alvo foram entregues ou disponibilizados no destino apropriado.

- Verifique se os públicos-alvo aparecem no Portal de público-alvo (para ativação do Experience Platform).
- Confirme a entrega bem-sucedida na nuvem por meio de logs de destino externos ou confirmação.

## Etapa 6: conectar-se com colaboradores {#connect-with-collaborators}

Com a configuração e o provisionamento de dados concluídos, sua organização agora está pronta para se conectar com colaboradores, enviando ou aceitando convites e enviando configurações de projeto para aprovação. Esse processo de conexão envolve enviar ou receber convites, revisar e enviar configurações de conexão (como casos de uso e consumo de crédito) e confirmar o relacionamento.

Use o espaço de trabalho **[!UICONTROL Conectar]** no menu de navegação esquerdo da interface do usuário do Collaboration para procurar editores disponíveis (os anunciantes não podem ser procurados no momento). Para obter uma visão geral desse fluxo, consulte o [Guia de Conectar com anunciantes ou editores](./connect/establishing-connections.md){target="_blank"}. Para uma apresentação visual do processo de conexão, incluindo a navegação de colaboradores e o gerenciamento das configurações de conexão, assista ao [vídeo de configuração da conta do anunciante](https://experienceleague.adobe.com/pt-br/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}.

## Próximas etapas

Agora você concluiu a integração e configurou a organização para colaboração segura. Em seguida, explore os seguintes recursos para aprofundar sua compreensão da ativação, medição e governança de dados:

- [Documentação do fluxo de trabalho de ativação de público-alvo](./collaborate/activate.md)
- [Casos de uso de medição](./collaborate/measure.md)
- [Práticas recomendadas de governança do Collaboration](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
