---
title: Notas de versão mais recentes do Real-Time CDP Collaboration
description: Seguir as versões mais recentes do Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 9e8371c36b58c2b3065e63396be43ebd2c52576f
workflow-type: tm+mt
source-wordcount: '1263'
ht-degree: 2%

---

# Notas de versão mais recentes do Real-Time CDP Collaboration

{{limited-availability-release-note}}

**Última atualização**: dezembro de 2025.

Essas notas de versão abordam a funcionalidade lançada no Adobe Real-Time CDP Collaboration. As versões do Collaboration operam em um modelo de entrega contínua, que permite uma cadência de lançamento mensal aproximada. Essas notas de versão são atualizadas com frequência. Portanto, verifique-as regularmente.

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
>Ao ativar públicos-alvo onde várias chaves de correspondência são usadas, se uma (ou mais) chave de correspondência não tiver sobreposições, nenhuma contagem de público-alvo ou ficar abaixo do limite, toda a ativação falhará. Verifique se os públicos-alvo têm sobreposição suficiente e se atendem ao limite mínimo de 1000 IDs em todas as chaves de correspondência antes da ativação.

* O destino do Adobe Experience Platform agora é compatível com a ativação de públicos-alvo com várias chaves de correspondência. Além disso, agora você pode usar uma chave vinculada ao configurar o mapeamento do destino para especificar qual chave de correspondência é enviada durante a ativação. Para saber mais, leia o [guia de destino do Experience Platform](../destinations/experience-platform.md#linked-keys).
* Agora os colaboradores podem editar vários públicos-alvo de uma só vez. Agora você pode editar metadados de público-alvo, acesso à conexão, nomes, descrições e categorias para vários públicos-alvo usando a ferramenta de edição em massa. Para saber mais sobre edição de públicos, leia o guia [gerenciar públicos-alvo](../setup/onboard-audiences.md#edit-audiences).

## Julho de 2025 {#july-2025}

A Real-time CDP Collaboration agora oferece suporte à colaboração de marca para marca. Os colaboradores agora podem formar conexões, independentemente de serem um anunciante ou editor. Isso permite oportunidades de colaboração mais flexíveis e permite que as marcas aproveitem os dados e insights umas das outras. Para saber mais sobre as diferenças entre a colaboração de marca para marca e de anunciante para editor, leia o guia [padrões de colaboração](../overview/collaboration-patterns.md).

* Os colaboradores agora podem se conectar usando [convites para conexão privada](../connect/establishing-connections.md#private-connection-invites). Compartilhe o código de conexão exclusivo de sua conta com um colaborador que pode usá-lo para se conectar diretamente com você. Este é um recurso principal da colaboração de marca para marca, permitindo que os colaboradores estabeleçam conexões além dos anunciantes que exploram o diretório **[!UICONTROL Descobrir colaboradores]**.
* [Destinos de autoatendimento](../setup/manage-destinations.md) agora estão disponíveis para anunciantes e editores.
* A ativação de público agora está disponível para ambos os colaboradores em uma conexão, independentemente de sua [função de conta](../overview/roles.md). As configurações de ativação de público-alvo são definidas ao [estabelecer conexões](../connect/establishing-connections.md#configure-connection-settings), permitindo que você especifique qual colaborador pode ativar públicos-alvo. Para saber mais sobre a ativação de público, leia o guia [ativar públicos-alvo](../collaborate/activate.md).
* O caso de uso **[!UICONTROL Ativar]** foi reconfigurado para oferecer suporte à colaboração de marca para marca. A guia **[!UICONTROL Ativar]** em um projeto agora exibe os públicos que foram enviados para o colaborador e os públicos que foram ativados para o destino pelo colaborador. Para saber mais, leia o guia [ativar públicos-alvo](../collaborate/activate.md). <br> ![O painel Ativar com as seções Públicos-alvo enviados para e Públicos-alvo ativadas.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* As pontuações do índice de público-alvo agora estão disponíveis na guia **[!UICONTROL Descubra]** de um projeto. A pontuação do índice de público-alvo é uma medida do desempenho de um público-alvo que corresponde ao público-alvo de seu colaborador. Essa pontuação é calculada com base nas contagens e sobreposições subjacentes do público-alvo. Para saber mais sobre as pontuações do índice de público-alvo, leia o guia [pontuação do índice de público-alvo](../collaborate/discover.md#audience-index-score).

## Maio de 2025 {#may-2025}

* O Real-Time CDP Collaboration agora está disponível para clientes na **Austrália** e na **Nova Zelândia**. Ele fica disponível automaticamente para clientes do Real-Time CDP Prime e do Ultimate nessas regiões.
* O Real-Time CDP Collaboration agora oferece [destinos de autoatendimento](../setup/manage-destinations.md) por meio da guia **[!UICONTROL Meus destinos]** na seção **[!UICONTROL Configuração]**. Os destinos permitem ativar públicos-alvo em plataformas de terceiros, como redes de publicidade ou plataformas de gerenciamento de dados, para alcançar seus clientes em vários canais. No momento, somente os destinos do Adobe Experience Platform são compatíveis. Se você estiver interessado em configurar um destino diferente, entre em contato com o representante da Adobe. Para saber mais sobre destinos, leia o guia [visão geral dos destinos](../destinations/overview.md).
   * Destinos também adiciona suporte para exibir públicos da Collaboration no [portal de público-alvo da Adobe Experience Platform](https://experienceleague.adobe.com/pt-br/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences).
* Agora você pode editar a frequência de atualização do público-alvo para conexões de dados existentes no Collaboration. Atualmente, você pode optar por atualizar os públicos-alvo diariamente ou a cada dois ou seis dias. Para saber mais sobre como editar a frequência de atualização do público-alvo, leia o guia [gerenciar conexões de dados](../setup/manage-data-connection.md#scheduling).
* As divisões de crédito entre colaboradores agora são definidas para cada caso de uso selecionado na conexão. Você pode definir diferentes regras de consumo de crédito para cada caso de uso para controlar melhor como seus créditos são usados. Para saber mais sobre a funcionalidade de divisão de crédito, leia o guia [configurações de conexão](../connect/establishing-connections.md#connection-settings). Para saber mais sobre como os créditos são consumidos, leia o guia [tipos de atividade de crédito](../setup/my-activity.md#types-of-activities). <br> ![Tela de configurações de conexão mostrando a funcionalidade de divisão de crédito.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Agora, os editores podem definir nomes e IDs de anunciante antes de aceitar as configurações de conexão de um anunciante. Os editores podem definir nomes e IDs que se alinham a seus sistemas internos, que podem ser diferentes dos nomes e IDs do anunciante. Para saber mais sobre como adicionar nomes e IDs de anunciante, leia o guia [configurações de conexão](../connect/establishing-connections.md#connection-settings.md). <br> ![Tela de configurações de conexão mostrando o publicador definindo nomes e IDs de anunciante.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## Abril de 2025 {#april-2025}

* Uma nova coluna **[!UICONTROL Entradas Processadas]** foi adicionada à tabela de atividade de consumo de crédito. Essa coluna exibe o número total de entradas (por exemplo, IDs ou linhas) processadas para cada atividade. [Leia mais](/help/guide/setup/my-activity.md#inputs-processed). <br> ![Coluna processada de entradas realçada na exibição Minha atividade.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Uma nova opção de email de contato foi adicionada à criação da conta. Isso ajuda os colaboradores do parceiro a contatarem você, conforme necessário, durante o processo de conexão. [Leia mais](../setup/onboard-account.md).

## Março de 2025 {#march-2025}

* Ao [fornecer públicos-alvo](/help/guide/setup/onboard-audiences.md) para o Collaboration, agora é possível definir uma frequência de atualização de público-alvo de **a cada um a seis dias** para gerenciar melhor a [atividade de crédito de Gerenciamento de público-alvo](/help/guide/setup/my-activity.md#types-of-activities). Para obter mais informações, leia o guia [gerenciar públicos-alvo](https://experienceleague.adobe.com/pt-br/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences). <br> ![A tela Agendar mostra intervalos de frequência diferentes para atualizar a associação de público-alvo.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "Tela de agendamento mostrando intervalos de frequência diferentes para atualizar associação de público-alvo."){width="250" align="center" zoomable="yes"}
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
