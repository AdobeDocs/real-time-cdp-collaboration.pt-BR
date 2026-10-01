---
title: Ativar públicos-alvo
description: Saiba como enviar públicos-alvo e ativar automática ou manualmente os públicos-alvo recebidos para destinos no Adobe Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
    internal-label: Use cases
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: df0c7fe0d09203a02a192931135abaa1715e593f
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 1%
---
# Ativar públicos-alvo

Use a guia **[!UICONTROL Ativar]** em um projeto para enviar públicos-alvo para o colaborador, revisar públicos-alvo recebidos do colaborador e ativar públicos-alvo recebidos para entrega em um destino configurado. A ativação pode ser criada automaticamente quando o público-alvo é recebido ou manualmente pelo colaborador destinatário. Para configurar e gerenciar destinos do espaço de trabalho de nível superior **[!UICONTROL Ativação]**, consulte a [visão geral de destinos](../destinations/overview.md).

>[!IMPORTANT]
>
>A guia **[!UICONTROL Ativar]** só estará disponível se o caso de uso **Ativação de público-alvo** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte [Gerenciar projetos](./manage-projects.md#project-use-cases).

Use a [guia Descobrir](./discover.md) para identificar os públicos-alvo que melhor correspondem à sua campanha e, em seguida, envie-os ao seu colaborador.

Se o receptor definir um destino de ativação automática nas configurações de conexão, o remetente selecionará um agendamento de ativação ao enviar o público-alvo. O destino é somente leitura para o remetente. Quando o público é recebido, o público é ativado automaticamente para o destino configurado do destinatário no agendamento de ativação do remetente. Para obter instruções de configuração de conexão, consulte [Configurar um destino de ativação automática](../connect/manage-connections.md#configure-auto-activation-destination).

Se o receptor não tiver configurado um destino de ativação automática, o envio e a ativação permanecerão ações separadas. O envio fornece ao destinatário acesso a um público-alvo, e o destinatário seleciona um destino e agenda ao ativá-lo manualmente. Somente destinos pré-configurados podem ser selecionados para ativação em um projeto. Para obter instruções de configuração de destino, consulte [Gerenciar destinos](../destinations/manage-destinations.md).

As seções e ações disponíveis para você dependem se a sua organização está enviando ou recebendo públicos-alvo no projeto. A guia **[!UICONTROL Ativar]** contém as seguintes seções:

| Seção | Descrição |
|---|---|
| **[!UICONTROL Públicos enviados para [colaborador]]** | Públicos enviados ao seu colaborador. |
| **[!UICONTROL Públicos-alvo recebidos]** | Públicos-alvo que seu colaborador enviou para você e que estão disponíveis para ativação. |
| **[!UICONTROL Públicos ativados]** | Públicos-alvo recebidos com ativações criadas automática ou manualmente. |

![A guia Ativar no nível do projeto com contagens resumidas nas seções Principais e expandidas Públicos-alvo enviados, Públicos-alvo recebidos e Públicos-alvo ativados. Cada seção exibe contagens de status e uma tabela de detalhes do público-alvo.](/help/assets/collaborate/activate/activate-dashboard.png){zoomable="yes"}

## Pré-requisitos {#prerequisites}

Antes de enviar ou ativar públicos, verifique se:

- Os públicos-alvo são originados e disponibilizados para envio. Para obter mais informações, consulte [Source e gerenciar públicos](../setup/onboard-audiences.md).
- Os públicos-alvo atendem ao limite mínimo de 1.000 sobreposições de identidade necessárias para envio e ativação.
- Os públicos-alvo são configurados com as chaves de correspondência necessárias ao usar públicos-alvo de várias chaves de correspondência.
- Pelo menos um destino está configurado se você precisar ativar os públicos-alvo recebidos. Para obter mais informações, consulte a [visão geral sobre destinos](../destinations/overview.md).
- Para a ativação automática, o receptor possui um destino ativo e o selecionou como o [destino da ativação automática](../connect/manage-connections.md#configure-auto-activation-destination) da conexão.

## Enviar públicos-alvo {#send-audiences}

Envie um público-alvo para conceder acesso ao colaborador. Após enviar o público-alvo, ele será exibido na seção **[!UICONTROL Públicos-alvo enviados para o [colaborador]]** e na seção **[!UICONTROL Públicos-alvo recebidos]** do seu colaborador.

Navegue até **[!UICONTROL Colaborar]**, abra um projeto e selecione a guia **[!UICONTROL Ativar]**.

Na seção **[!UICONTROL Públicos enviados para [colaborador]]**, selecione o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)). Se nenhum público-alvo tiver sido enviado, selecione **[!UICONTROL Enviar público-alvo]** na exibição vazia.

![A guia Ativar no nível do projeto quando nenhum público-alvo for enviado. A mensagem de exibição vazia explica que você não enviou um público-alvo e exibe um botão Enviar público-alvo.](/help/assets/collaborate/activate/activate-new-audiences.png){zoomable="yes"}

O fluxo de trabalho **[!UICONTROL Enviar públicos-alvo]** é aberto. Use o seletor de público para encontrar um público ou selecione **[!UICONTROL Procurar públicos]** para comparar os públicos disponíveis.

>[!IMPORTANT]
>
>Somente públicos-alvo com mais de 1000 identidades sobrepostas estão disponíveis para ativação. Se as sobreposições de público-alvo estiverem próximas ao limite de identidade de 1000, a ativação poderá falhar.

![O fluxo de trabalho Enviar públicos-alvo com um seletor de público-alvo e um botão Procurar públicos-alvo. O fluxo de trabalho permite que o remetente escolha um público-alvo antes de definir as chaves de correspondência e acessar as configurações.](/help/assets/collaborate/activate/audience-activation.png){zoomable="yes"}

Na caixa de diálogo **[!UICONTROL Procurar públicos-alvo]**, revise a **[!UICONTROL Contagem de identidades]**, **[!UICONTROL Identidades sobrepostas]** e **[!UICONTROL Sobreposição %]** para cada público-alvo.

![A caixa de diálogo Procurar públicos-alvo listando os públicos-alvo disponíveis com sua contagem de identidades, contagem de identidades sobrepostas e porcentagem de sobreposição.](/help/assets/collaborate/activate/browse-audiences.png){zoomable="yes"}

>[!IMPORTANT]
>
>Se um público-alvo usar várias chaves de correspondência, cada chave de correspondência selecionada deverá atingir o limite de sobreposição necessário. Use a [guia Descobrir](./discover.md) para confirmar se o público-alvo atende aos requisitos de sobreposição antes de enviá-lo.

Selecione o público que deseja enviar e selecione **[!UICONTROL Salvar]**.

O público selecionado aparece no fluxo de trabalho com sua identidade e informações de sobreposição.

![O fluxo de trabalho Enviar públicos-alvo com um público-alvo selecionado mostrando sua contagem de identidades, contagem de identidades sobrepostas, porcentagem de sobreposição, chaves de correspondência e a opção Editar chaves de correspondência.](/help/assets/collaborate/activate/audience-selected.png){zoomable="yes"}

### Editar chaves de correspondência {#edit-match-keys}

Use as chaves de correspondência configuradas para a conexão do colaborador ou remova qualquer chave de correspondência que não se aplique ao público-alvo.

Selecione **[!UICONTROL Editar chaves de correspondência]** no público selecionado.

![O público selecionado no fluxo de trabalho Enviar públicos-alvo com a opção Editar chaves de correspondência realçada.](/help/assets/collaborate/activate/edit-match-keys.png){zoomable="yes"}

A caixa de diálogo **[!UICONTROL Editar chaves de correspondência]** é exibida. Desative todas as chaves de correspondência que você não deseja usar e selecione **[!UICONTROL Salvar]**.

>[!NOTE]
>
>Pelo menos uma chave de correspondência deve permanecer selecionada.

![A caixa de diálogo Editar chaves de correspondência com controles de alternância para as chaves de correspondência disponíveis por meio da conexão do colaborador e um botão Salvar.](/help/assets/collaborate/activate/edit-match-keys-selection.png){zoomable="yes"}

### Configurar o acesso do público {#configure-audience-access}

Configure como o público-alvo é enviado e por quanto tempo seu colaborador pode acessá-lo.

Use o controle **[!UICONTROL Duração do acesso]** para selecionar uma das seguintes opções:

- **[!UICONTROL Enviar agora (único)]**: enviar o público-alvo uma vez. O colaborador destinatário pode ativá-lo uma vez.
- **[!UICONTROL Agendar envio de público recorrente]**: atualize o público durante um período de acesso especificado. Use o controle **[!UICONTROL Intervalo de datas]** para selecionar as datas inicial e final.

![A etapa Duração do acesso no fluxo de trabalho Enviar públicos-alvo com opções para enviar o público-alvo uma vez ou agendar o envio de um público-alvo recorrente. A opção recorrente exibe controles de data para definir o período de acesso.](/help/assets/collaborate/activate/activation-frequency.png)

### Escolha uma programação de ativação automática {#auto-activation-schedule}

Se o colaborador tiver configurado um destino de ativação automática para a conexão, a seção **[!UICONTROL Ativação]** indicará que a **[!UICONTROL Ativação automática]** está habilitada. O destino selecionado pelo receptor é mostrado como somente leitura. Como remetente, use a **[!UICONTROL Frequência]** para escolher quando a ativação será executada:

- **[!UICONTROL Ativar agora (único)]**: execute a ativação uma vez quando o público-alvo for recebido.
- **[!UICONTROL Agendar ativação de público-alvo única]**: execute a ativação uma vez na data e hora futuras que você selecionar.
- **[!UICONTROL Agendar ativação recorrente]**: execute a ativação no agendamento configurado durante o intervalo de datas selecionado.

![O fluxo de trabalho Enviar públicos-alvo com a Ativação automática habilitada e o menu Frequência mostrando opções de ativação imediatas, futuras, únicas e recorrentes.](/help/assets/collaborate/activate/choose-auto-activation-schedule.png){zoomable="yes"}

Para uma ativação recorrente, configure o agendamento de ativação, a hora de início e o intervalo de datas. A ativação automática oferece suporte a agendamentos imediatos, futuros únicos ou recorrentes; não é necessário realizar a ativação recorrente.

![O fluxo de trabalho Enviar públicos-alvo configurado com um agendamento de ativação recorrente diária, hora de início e intervalo de datas.](/help/assets/collaborate/activate/configure-recurring-auto-activation.png){zoomable="yes"}

Quando as configurações de público-alvo e acesso forem concluídas, selecione **[!UICONTROL Enviar]**.

O público aparece na sua seção **[!UICONTROL Públicos enviados para o [colaborador]]**. Seu colaborador pode revisá-lo na seção **[!UICONTROL Públicos-alvo recebidos]**. Se a ativação automática estiver ativada, o Collaboration também criará a ativação para o receptor e a ativação será executada de acordo com o agendamento selecionado.

## Exibir públicos-alvo enviados {#view-sent-audiences}

Use a seção **[!UICONTROL Públicos enviados para o [colaborador]]** para analisar os públicos enviados e monitorar seu status de acesso atual.

Cada público-alvo enviado exibe as seguintes informações:

| Coluna | Descrição |
|---|---|
| **[!UICONTROL Nome do público-alvo]** | O nome do público-alvo enviado. |
| **[!UICONTROL Status]** | O status de acesso atual do público-alvo. |
| **[!UICONTROL Contagem de identidades]** | O número de identidades no público-alvo. |
| **[!UICONTROL Identidades sobrepostas]** | O número de identidades que se sobrepõem ao inventário do colaborador. |
| **[!UICONTROL Criado]** | A data e a hora em que o público-alvo foi enviado pela primeira vez. |
| **[!UICONTROL Último envio]** | A data e a hora em que os dados do público-alvo foram enviados mais recentemente para o colaborador. |
| **[!UICONTROL Duração do acesso]** | A configuração de acesso definida quando o público-alvo foi enviado. |
| **[!UICONTROL Chaves correspondentes]** | As teclas de correspondência usadas ao enviar o público-alvo. |

### Excluir um público-alvo enviado {#delete-sent-audience}

Exclua um público-alvo enviado para removê-lo da lista de públicos-alvo enviados e revogar o acesso do colaborador.

Selecione o ícone de exclusão (![Ícone de exclusão.](/help/assets/icons/delete.png)) ao lado do público na seção **[!UICONTROL Públicos enviados para o [colaborador]]**.

![A seção Públicos-alvo enviados com o ícone de exclusão exibido ao lado de uma linha de público-alvo.](/help/assets/collaborate/activate/delete-sent-audiences.png){zoomable="yes"}

Uma caixa de diálogo de confirmação é exibida. Selecione **[!UICONTROL Excluir]** para confirmar.

![A caixa de diálogo de confirmação de exclusão do público-alvo enviado explicando que o público-alvo será removido e o colaborador perderá o acesso, com os botões Cancelar e Excluir.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

O público-alvo é removido da seção e o colaborador perde acesso a ele.

## Exibir públicos-alvo recebidos {#received-audiences}

Use a seção **[!UICONTROL Públicos-alvo recebidos]** para analisar os públicos-alvo enviados pelo seu colaborador a você. Se um destino de ativação automática foi configurado antes do envio do público, o Collaboration cria automaticamente uma ativação quando o público é recebido. Para ativações automáticas recorrentes, você também pode criar uma ativação manual adicional para um destino diferente. Consulte [Ativar manualmente um público-alvo recebido](#activate-received-audience) para obter detalhes. Se nenhum destino de ativação automática foi configurado, ative o público-alvo manualmente.

Cada público-alvo recebido exibe as seguintes informações:

| Coluna | Descrição |
|---|---|
| **[!UICONTROL Nome do público-alvo]** | O nome do público-alvo recebido. |
| **[!UICONTROL Status]** | O status de acesso atual do público-alvo. |
| **[!UICONTROL Contagem de identidades]** | O número de identidades no público-alvo. |
| **[!UICONTROL Identidades sobrepostas]** | O número de identidades que se sobrepõem ao seu estoque. |
| **[!UICONTROL Última execução do fluxo de dados]** | A data e a hora da execução mais recente do fluxo de dados para o público-alvo. |
| **[!UICONTROL Duração do acesso]** | A configuração de acesso definida pelo colaborador que enviou o público. |
| **[!UICONTROL Chaves correspondentes]** | As chaves de correspondência usadas para o público-alvo. |

![A seção Públicos-alvo recebidos com contagem de público-alvo ativos e expirados. Cada linha de público mostra seu nome, status, informações de identidade, última execução do fluxo de dados, duração do acesso, chaves de correspondência e um ícone de adição usado para iniciar a ativação.](/help/assets/collaborate/activate/received-audiences-section.png){zoomable="yes"}

### Ativar manualmente um público recebido {#activate-received-audience}

Ative manualmente um público-alvo recebido para enviar seus dados a um dos destinos configurados.

Na seção **[!UICONTROL Públicos-alvo recebidos]**, selecione o ícone adicionar (![Ícone adicionar.](/help/assets/icons/plus.png)) ao lado do público que você deseja ativar.

A caixa de diálogo **[!UICONTROL Ativar público-alvo]** é exibida.

Use **[!UICONTROL Destino]** para selecionar o destino que recebe os dados do público-alvo. Se a lista de destinos estiver vazia, configure um destino antes de continuar. Para obter instruções, consulte a [visão geral sobre destinos](../destinations/overview.md).

Configure a **[!UICONTROL Frequência]** e os controles de agendamento disponíveis para escolher quando e com que frequência a ativação é executada. Em seguida, selecione **[!UICONTROL Ativar]**.

O exemplo a seguir mostra o fluxo de trabalho de ativação manual com **[!UICONTROL Exportações de público-alvo do Northstar]** selecionadas como destino.

![Um exemplo da caixa de diálogo Ativar público-alvo manual para Clientes da Campanha de outono do Northstar, com Exportações de Público-alvo do Northstar selecionadas e uma agenda diária, hora de início e intervalo de datas configurados.](/help/assets/collaborate/activate/manually-activate-received-audience.png){zoomable="yes"}

>[!NOTE]
>
>Para um público-alvo recebido com uma ativação automática recorrente, é possível criar manualmente uma ativação adicional para esse público-alvo para um destino diferente. A ativação automática recorrente continua de forma independente.

A caixa de diálogo é fechada e a ativação é exibida na seção **[!UICONTROL Públicos ativados]**. O público-alvo recebido permanece disponível na seção **[!UICONTROL Públicos-alvo recebidos]** enquanto seu acesso permanece ativo.

## Exibir públicos ativados {#activated-audiences}

Use a seção **[!UICONTROL Públicos-alvo ativados]** para confirmar quais públicos-alvo recebidos criaram ativações automática ou manualmente e revisar seu destino e status de entrega. As ativações criadas automaticamente aparecem aqui sem exigir que o receptor conclua o fluxo de trabalho de ativação manual.

![A guia Ativar, que mostra os clientes da campanha do Northstar Fall nos públicos-alvo recebidos, e a ativação diária criada automaticamente para as exportações de público-alvo do Northstar nos públicos-alvo ativados.](/help/assets/collaborate/activate/view-auto-activated-audience.png){zoomable="yes"}

Cada público ativado exibe as seguintes informações:

| Coluna | Descrição |
|---|---|
| **[!UICONTROL Nome do público-alvo]** | O nome do público-alvo ativado. |
| **[!UICONTROL Status]** | O status de ativação atual. |
| **[!UICONTROL Contagem ativada]** | O número de identidades ativadas para o destino. |
| **[!UICONTROL Última atualização]** | A data e a hora em que o público-alvo ativado foi atualizado mais recentemente. |
| **[!UICONTROL Destino]** | O destino que recebe os dados do público-alvo. |
| **[!UICONTROL Frequência]** | A frequência de ativação, como uma programação única ou recorrente. |
| **[!UICONTROL Data]** | A data ou o intervalo de datas em que a ativação é executada. |
| **[!UICONTROL Chaves correspondentes]** | As chaves de correspondência incluídas no público ativado. |

![A seção Públicos ativados com contagens de ativação ativas, arquivadas e pausadas. Cada linha mostra o nome do público-alvo, o status, a contagem ativada, a data da última atualização, o destino, a frequência, a data de ativação, as chaves de correspondência e um ícone de exclusão.](/help/assets/collaborate/activate/activated-audiences-section.png){zoomable="yes"}

### Excluir um público-alvo ativado {#delete-activated-audience}

Exclua um público-alvo ativado para remover a ativação da seção **[!UICONTROL Públicos-alvo ativados]**.

Selecione o ícone de exclusão (![Ícone de exclusão.](/help/assets/icons/delete.png)) ao lado do público-alvo ativado.

Uma caixa de diálogo de confirmação é exibida. Selecione **[!UICONTROL Excluir]** para confirmar.

![A caixa de diálogo de confirmação da exclusão de público-alvo ativado explicando que o público-alvo será removido da lista de públicos-alvo ativados e poderá ser ativado novamente mais tarde, com os botões Cancelar e Excluir.](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

A ativação é removida da lista. Você pode ativar o público-alvo recebido novamente enquanto o acesso dele permanecer ativo.

## Próximas etapas {#next-steps}

Após enviar ou ativar públicos, monitore seu status nas seções **[!UICONTROL Públicos enviados para [colaborador]]** e **[!UICONTROL Públicos ativados]**. Quando as campanhas estiverem concluídas, trabalhe com a equipe de capacitação e engenharia da Adobe para carregar dados de medição e exibir os [relatórios de medição](./measure.md) correspondentes.
