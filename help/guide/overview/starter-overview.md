---
title: Visão geral do RTCDP Collaboration Starter
description: Saiba como o Adobe Real-Time CDP Collaboration Starter ajuda a expandir e aprimorar a colaboração centrada na privacidade com um parceiro licenciado sem exigir sua própria licença completa da Real-Time CDP.
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: c759496b528ed6c1e173f1ca1f1469da572c85df
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 3%

---

# Visão geral do Adobe Real-Time CDP Collaboration [!DNL Starter]

Use o Adobe Real-Time CDP Collaboration [!DNL Starter] para colaborar com um parceiro licenciado em projetos de dados centrados na privacidade. Não é necessário ter sua própria licença da Collaboration para participar.

Seu parceiro licenciado o convida para a Collaboration e usa seus créditos para financiar fluxos de trabalho conjuntos, tanto em padrões de anunciante para editor quanto de marca para marca. Para saber mais sobre esses padrões e como eles funcionam, leia os guias [padrões de colaboração](./collaboration-patterns.md) e [fluxo de trabalho completo](./end-to-end-workflow.md).

Como usuário convidado [!DNL Starter], você pode:

* Integrar e gerenciar dados de colaboração em uma conta do [!DNL Starter].
* Source e manter públicos-alvo para uso em projetos conjuntos.
* Obtenha insights sobre as sobreposições de público-alvo com seu parceiro para oferecer suporte ao direcionamento eficaz e à medição de campanha.
* Ative públicos e compartilhe-os com seu parceiro para ativação e envolvimento conjuntos de campanhas.

## Pré-requisitos {#prerequisites}

Para começar a usar o Collaboration [!DNL Starter], verifique se sua organização e seu parceiro licenciado estão localizados na mesma região. Você deve ser convidado por um parceiro que possua uma licença do Real-Time CDP Prime, Ultimate ou Collaboration.

Para iniciar o convite, forneça as seguintes informações ao seu parceiro licenciado:

* Nome do contato
* Email de contato
* Empresa
* Função (Anunciante/Editor): Anunciante
* Setor

Depois que você receber e aceitar o convite, sua organização deverá revisar e assinar uma Ordem de Venda sem custo com a Adobe para acessar o Collaboration [!DNL Starter]. Para obter mais detalhes sobre o processo de convite, consulte o guia [convidando um colaborador para a Collaboration [!DNL Starter]](../connect/establishing-connections.md#invite-collaborator).

## Medidas de proteção {#guardrails}

Leia a tabela a seguir para entender as medidas de proteção principais que se aplicam à sua conta do [!DNL Starter]. Isso inclui limites na origem do público-alvo, volume de dados, frequência de atualização, sobreposições de público-alvo e recursos de ativação.

| Grade de Proteção | Descrição |
|----------| ------------|
| Fonte do público-alvo | Você pode trazer dados de público-alvo para a Collaboration com **[!DNL Amazon S3]** como fonte. Para obter instruções passo a passo, consulte [como configurar [!DNL Amazon S3] para fornecimento de público-alvo](../setup/configure-aws-s3-audience-sourcing.md). |
| Público-alvo | Sua conta [!DNL Starter] tem direito a no máximo:<ul><li>10 públicos-alvo originados de um bucket de [!DNL AWS S3]</li><li>50 milhões de identidades totais (calculadas pelo número de linhas nos dados do público-alvo)</li><li>1 atualização por público a cada 6 dias</li></ul> |
| Sobreposições de público-alvo e insights | Não há limite de uso para a frequência com que você pode executar sobreposições de público-alvo e insights entre seus públicos-alvo. Saiba como [descobrir sobreposições e comparar públicos](../collaborate/discover.md). |
| Activation | Como usuário do [!DNL Starter], você pode ativar e compartilhar públicos somente com o parceiro que convidou você. A configuração de destinos para plataformas externas não está disponível. Saiba mais sobre [como ativar seus públicos-alvo](../collaborate/activate.md). |

{style="table-layout:auto"}

## Introdução {#getting-started}

Depois que você [aceitar seu convite e concordar com os termos](../connect/establishing-connections.md#accept-invitation-sign-terms), faça logon no [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"} com suas credenciais. Antes de usar o Collaboration, sua conta deve receber o acesso e as funções apropriadas.

Use este fluxo de trabalho para configurar sua conta do [!DNL Starter] e começar a colaborar com seu parceiro.

### Configurar o acesso do administrador {#setup-admin-access}

Primeiro, use o espaço de trabalho **Acesso de Administrador** para conceder a si mesmo o acesso necessário. Isso garante que você tenha direitos administrativos e acesso de usuário aos produtos da Experience Platform. Para obter etapas detalhadas sobre como configurar o acesso inicial, consulte as [instruções de acesso de administrador](../setup/starter-admin-access.md).

Depois de concluído, você deverá ver as **[!UICONTROL Permissões]**, **[!UICONTROL Experience Platform]** e **[!UICONTROL Real-Time CDP Collaboration]** na seção de **[!UICONTROL Acesso rápido]** da sua página inicial do [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}.

![O espaço de trabalho do Adobe Experience Cloud que mostra as Permissões, o Experience Platform e o Real-Time CDP Collaboration após a instalação de acesso do administrador do produto.](/help/assets/overview/starter/setup-admin-access.png){zoomable="yes"}

Para obter mais detalhes sobre funções de acesso e diferentes produtos da Adobe Experience Cloud, leia a [visão geral do controle de acesso](../permissions/overview.md).

### Configurar permissões {#configure-permissions}

Agora que você tem privilégios de administrador, pode atribuir funções e permissões a si mesmo e a outros usuários em sua organização. Esta etapa é necessária antes de acessar o Real-Time CDP Collaboration ou permitir que outros possam usá-lo. Para obter instruções detalhadas, consulte [como configurar permissões](../setup/starter-permission-controls.md). Para obter mais informações sobre as diferentes funções e permissões disponíveis no Collaboration, consulte a documentação de [gerenciar funções](../permissions/manage-roles.md).

Depois que as funções e permissões forem atribuídas, confirme se você pode acessar o Collaboration. Navegue até [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"} e selecione **[!UICONTROL Real-Time CDP Collaboration]** na seção **[!UICONTROL Acesso rápido]**. Isso abre o espaço de trabalho **[!UICONTROL Adobe Real-Time CDP Collaboration]**, onde você pode começar a usar os recursos do Collaboration.

### Configurar conexões {#set-up-connections}

Em seguida, siga as etapas nos guias a seguir para configurar a conexão e começar a colaborar com seu parceiro:

* [Configurar sua conta do Collaboration](../setup/onboard-account.md)
* [Estabeleça uma conexão com seu colaborador convidado](../connect/overview.md)
* [Crie um novo projeto e comece a colaborar com seu parceiro](../collaborate/overview.md)

### Entender o uso de crédito {#understand-credit-usage}

Todas as atividades [!DNL Starter] do Collaboration usam créditos. No entanto, como usuário convidado, não é necessário comprar ou gerenciar esses créditos. O colaborador que convidou você cobre todo o uso de crédito associado às suas atividades. Para saber mais, consulte o uso e o consumo de crédito [na documentação do Collaboration [!DNL Starter]](../setup/starter-credit-usage.md).

## Próximas etapas {#next-steps}

Agora você concluiu a configuração inicial e configurou sua organização para colaboração segura. Em seguida, explore os seguintes recursos para saber mais sobre o fornecimento de público-alvo e diferentes casos de uso de projetos no Collaboration:

* [Source e gerenciar públicos](../setup/onboard-audiences.md)
* [Casos de uso de projetos](../collaborate/overview.md#project-use-cases):
   * [Descubra sobreposições e compare públicos](../collaborate/discover.md)
   * [Ativar públicos-alvo](../collaborate/activate.md)
   * [Meça o desempenho da campanha](../collaborate/measure.md)
