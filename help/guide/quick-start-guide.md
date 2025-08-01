---
title: Guia de início rápido do Real-Time CDP Collaboration
description: Saiba como integrar sua organização ao Real-Time CDP Collaboration, incluindo a configuração de funções e organizações, fornecimento de público-alvo, ativação e medição. Este guia ajuda os colaboradores a definir configurações de conexão para começar a usar seus públicos de forma segura e eficiente.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
source-git-commit: d460cb12b43b6c250a5fb491c1efc223c53abb23
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 0%

---

# Guia de início rápido do Real-Time CDP Collaboration

{{limited-availability-release-note}}

Comece a usar o Real-Time CDP Collaboration configurando sua organização, fornecendo públicos-alvo e habilitando a ativação e a medição com foco na privacidade.

## Pré-requisitos

Antes de começar, verifique se você tem o seguinte:

- Uma licença ativa do Real-Time CDP Collaboration.
- [Acesso de administrador de sistema ou de produto ao Adobe Experience Platform](./permissions/overview.md).
- [Acesso provisionado para usuários finais](./permissions/manage-user-access.md).
- [Funções criadas para sua organização e atribuídas a usuários](./permissions/manage-roles.md).
- Acesso aos ativos de marca, como nome, logotipo e banner da sua organização.
- Uma [estratégia de chave de correspondência definida](./setup/onboard-account.md#set-up-match-keys) (no momento, o email com hash é a única chave de correspondência com suporte).
- (Opcional) Acesse uma fonte de nuvem compatível (Amazon S3 ou Snowflake) se você não estiver usando o Experience Platform para gerenciamento de público-alvo.

## Etapa 1: concluir configuração baseada em função {#complete-role-based-setup}

As funções de acesso da sua organização determinam o que os usuários podem ver e fazer no Collaboration. Antes de continuar, verifique se as permissões baseadas em função estão configuradas corretamente para garantir o acesso e a visibilidade apropriados na plataforma.

**Recursos:**

- [Documentação de acesso do usuário](./permissions/manage-user-access.md)
- [Documentação de configuração de função](./permissions/manage-roles.md)


Assista a este vídeo para saber como atribuir acesso e permissões de produto ao Collaboration usando o Admin Console e o Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## Etapa 2: configurar a conta do Collaboration {#set-up-your-account}

Antes de fornecer públicos, você deve configurar sua conta no Collaboration. Isso controla como você aparece e a que você tem acesso na interface do.

Se você não tiver o acesso necessário, consulte a etapa 1 ou entre em contato com o administrador da organização para obter ajuda para concluir essa configuração.

Defina a função da sua conta no Collaboration, forneça ativos de marca e configure chaves de correspondência para alinhar públicos-alvo em todas as conexões.

>[!NOTE]
>
>É possível criar uma ou mais contas (como anunciante e editor) durante a configuração. Determinados campos, como ativos de marca e email de contato, podem ser atualizados posteriormente no espaço de trabalho **[!UICONTROL Configurações]**.

- **Atribuir uma função** - Determina se sua conta é um anunciante ou um editor. Sua função define quais recursos você tem no Collaboration. Para saber mais sobre como as funções afetam o fluxo de trabalho de colaboração, consulte o guia [funções](./overview/roles.md).
- **Ativos de marca** - Adicione o seguinte à sua conta:
   - Nome da conta (máximo de 100 caracteres)
   - Descrição (máximo de 1.000 caracteres)
   - Logotipo (SVG &lt;20KB, idealmente quadrado)

>[!NOTE]
>
>Se você estiver criando uma conta de editor e quiser que o seja exibido publicamente no catálogo de conexões da Collaboration, entre em contato com o representante de conta da Adobe. As contas do editor exigem um banner de marca personalizado (JPG 2688x1536); esse arquivo pode ser compartilhado diretamente com o representante.

- **Email de contato** - Forneça um email comercial para que os colaboradores usem depois que uma conexão for estabelecida.
- **Configurar chaves de correspondência** - Selecione os identificadores usados para correspondência de público-alvo (atualmente, o email com hash é a única chave de correspondência com suporte).

Para saber mais sobre a configuração inicial da conta, incluindo como definir funções, carregar ativos de marca e configurar chaves de correspondência, consulte o guia [configuração inicial da conta](./setup/onboard-account.md#initial-account-setup){target="_blank"}.

Assista a este vídeo para obter uma apresentação passo a passo da configuração de um anunciante, incluindo criação de conta, marca e configuração principal de correspondência.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## Etapa 3: públicos-alvo da Source (do Experience Platform ou de uma fonte na nuvem) {#source-audiences}

Depois que sua conta for criada e suas chaves de identidade visual e correspondência forem configuradas, você estará pronto para começar a fornecer públicos-alvo. Escolha um dos seguintes métodos de seleção de fornecedor com base no armazenamento de dados e nas necessidades comerciais.

### Opção A: Source do Experience Platform

[Use o Collaboration para vincular uma sandbox que contém públicos](./setup/onboard-audiences.md). Use esse método de autoatendimento para fazer referência a segmentos de público-alvo existentes na sua instância do Experience Platform.

#### Configurar públicos

Configure como os públicos-alvo são preparados, combinados e controlados para uso em conexões.

- **Selecionar públicos-alvo** *(somente Experience Platform)* - Escolha segmentos de público-alvo com identificadores compatíveis.
- **Mapear chaves de correspondência** - Alinhar campos de público-alvo com as chaves de correspondência configuradas.
- **Aplicar transformações** - Hash valores de texto sem formatação (por exemplo, email), se necessário.
- **Atualizações de agendamento** - Defina a frequência de atualização (por exemplo, diariamente).
- **Definir configurações de consentimento** - Determine quais perfis estão qualificados para serem incluídos em conexões selecionando um modo de consentimento: aceitação, recusa ou nenhum.

>[!NOTE]
>
>Você pode adicionar ou remover públicos e atualizar o agendamento de atualização diretamente no Collaboration. Para alterar outras configurações, como chaves de correspondência ou modo de consentimento, você deve excluir e recriar a conexão de dados.

>[!IMPORTANT]
>
>**Número máximo de públicos-alvo por função de colaborador:**
>
>- **Anunciantes** podem ter até 25 públicos-alvo.
>- **Os editores** podem ter até 250 públicos-alvo (cada um com no mínimo 5.000 IDs).

>[!IMPORTANT]
>
>**Corresponder requisitos de chave:**
>
>Todas as chaves de correspondência devem ser **cortadas**, **em minúsculas** e **SHA256-com hash**.\
>Se você fornecer valores com hash que usam caracteres em maiúsculas, o Collaboration os converterá automaticamente em minúsculas.\
>Se sua origem contiver **identificadores de texto sem formatação**, use a opção **[!UICONTROL Aplicar transformação]** para aplicar o hash. Essa opção só está disponível ao fornecer públicos-alvo do Experience Platform e não tem suporte para fontes baseadas em nuvem.
>
>Para obter mais informações, consulte a seção [mapear campos](./setup/onboard-audiences.md#map-fields) do guia de origem e gerenciar públicos.

Para ver uma apresentação completa de como fornecer públicos-alvo usando o Collaboration, assista ao vídeo abaixo.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

Como alternativa, consulte o documento sobre [origem de públicos-alvo no Collaboration](./setup/onboard-audiences.md#source-and-manage-audiences).

### Opção B: Source do Snowflake ou Amazon S3

Para configurar uma fonte de nuvem (por exemplo, [!DNL AWS S3] ou [!DNL Snowflake]), prepare os dados do público-alvo usando a seguinte [PDF de Especificação de Público-Alvo](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf). Depois de concluir, ou em caso de dúvidas, entre em contato com o representante de conta da Adobe para finalizar a configuração. Este método não é de autoatendimento e requer a assistência da Adobe.

>[!IMPORTANT]
>
>Os arquivos de público-alvo baseados em nuvem devem seguir o esquema necessário descrito na PDF de especificação de público-alvo. Os arquivos devem incluir identificadores com hash (SHA256 em letras minúsculas), campos de metadados obrigatórios como `segment_name` e `activation_id` e usar formatos compatíveis como CSV ou Parquet. O Adobe não normaliza dados antes da ativação. O TTL é aplicado com base na duração do público-alvo.
>
>Todos os públicos-alvo no arquivo carregado são totalmente originários nesse estágio. A [configuração de visibilidade de público-alvo](/help/guide/setup/onboard-audiences.md#metadata-visibility) determina se seus colaboradores podem ver seu público-alvo e é gerenciada por meio da interface do usuário do Collaboration.

## Etapa 4: ativar públicos-alvo (para Experience Platform ou um destino de nuvem) {#activate-audiences}

Em seguida, ative os públicos-alvo para sua instância do Experience Platform ou para um destino de nuvem.

### Opção A: Ativar para o Experience Platform

Conclua as etapas a seguir descritas no guia [configurar o Adobe Experience Platform como destino](/help/guide/destinations/experience-platform.md).

- **Criar um destino** - Use a interface do usuário para configurar um destino do Experience Platform (nível de sandbox).
- **Mapear chaves de correspondência** - Selecione o identificador (por exemplo, `hashedEmail`).
- **Definir TTL** - Definir expiração (1-30 dias).
- **Verificar no Audience Portal** - Depois que um colaborador enviar um público-alvo para você, verifique se ele aparece no Audience Portal sob a origem &quot;[!UICONTROL Real-Time CDP Collaboration].&quot;

### Opção B: Ativar para nuvem

Para configurar um destino de nuvem (por exemplo, [!DNL AWS S3] ou [!DNL Snowflake]), entre em contato com o representante de conta da Adobe para iniciar o processo de configuração. Dependendo do destino da nuvem, você precisará fornecer detalhes de destino da nuvem, como caminho do arquivo, credenciais, localizadores de conta etc. Depois que as informações necessárias forem fornecidas, o Adobe definirá a configuração do destino da nuvem.

Os dados de público-alvo enviados para um destino de nuvem seguem um esquema predefinido. Para obter uma descrição detalhada dos campos e formatos necessários, baixe o [Guia do Collaboration Audience Activation](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

## Etapa 5: configurar medição (opcional) {#set-up-measurement}

>[!AVAILABILITY]
>
>Este recurso está na **beta** e está disponível exclusivamente para clientes no programa de Disponibilidade Limitada. Entre em contato com seu representante da Adobe para solicitar acesso.

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Medida]** só estará disponível se o caso de uso **[!UICONTROL Medida]** tiver sido habilitado [durante o processo de conexão](./connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./collaborate/manage-projects.md#project-use-cases).

O Collaboration oferece vários relatórios para analisar o alcance, a frequência e a eficácia da campanha. Embora o espaço de trabalho **[!UICONTROL Medida]** esteja disponível na interface do usuário, a funcionalidade completa de relatórios pode exigir a habilitação do back-end.

Para saber como exibir e interpretar relatórios de medição, consulte o [Guia de medição](./collaborate/measure.md). Ele abrange atribuição, métricas de resumo da campanha e painéis, como curvas de alcance e distribuição de frequência.

<!-- 
Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."

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
   - Submit the report. It will run on the selected date and populate within 24 hours. 
-->

## Etapa 6: conectar-se com colaboradores {#connect-with-collaborators}

Com a configuração concluída, sua organização agora está pronta para se conectar com colaboradores, enviando ou aceitando convites e enviando configurações de projeto para aprovação. Esse processo de conexão envolve enviar ou receber convites, revisar e enviar configurações de conexão (como casos de uso e consumo de crédito) e confirmar a conexão.

Como anunciante, use o espaço de trabalho **[!UICONTROL Conectar]** no menu de navegação esquerdo para procurar editores disponíveis. Como alternativa, os colaboradores podem se conectar diretamente através de [convites para conexão privada](./connect/establishing-connections.md#private-connection-invite){target="_blank"}.

>[!NOTE]
>
>Atualmente, somente anunciantes podem navegar pelos editores. Os editores não podem procurar ou iniciar conexões com anunciantes.

Para obter uma visão geral desse fluxo, consulte o [guia de estabelecimento de conexões](./connect/establishing-connections.md){target="_blank"}. Para uma apresentação visual do processo de conexão, incluindo a navegação de colaboradores e o gerenciamento das configurações de conexão, assista ao [vídeo de configuração da conta do anunciante](https://experienceleague.adobe.com/pt-br/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}.

## Próximas etapas

Agora você concluiu a configuração inicial e configurou sua organização para colaboração segura. Em seguida, explore os seguintes recursos para aprofundar sua compreensão da ativação, medição e governança de dados:

- [Documentação do fluxo de trabalho de ativação de público-alvo](./collaborate/activate.md)
- [Casos de uso de medição](./collaborate/measure.md)
- [Práticas recomendadas de governança do Collaboration](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
