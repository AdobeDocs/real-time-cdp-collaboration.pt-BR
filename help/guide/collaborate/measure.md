---
title: Medir desempenho
description: Meça o desempenho de suas campanhas em diferentes canais. Saiba como usar e interpretar vários relatórios.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: 0cf888e36ffc4730fc8de4d8adccae0e0fc2caa8
workflow-type: tm+mt
source-wordcount: '1949'
ht-degree: 6%

---

# Medir desempenho

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Medida]** só estará disponível se o caso de uso **Medida** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

Saiba mais sobre os relatórios disponíveis no Adobe Real-Time CDP Collaboration e entenda como medir e analisar o desempenho de suas campanhas de marketing em vários canais.

## Pré-requisitos {#prerequisites}

Antes de acessar os relatórios de medição no Collaboration, você deve:

* [Conecte-se](/help/guide/connect/establishing-connections.md) a um colaborador com o caso de uso **Medição** habilitado
* Colabore em pelo menos um projeto com seu colaborador. Saiba como [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project).
* Execute sua campanha e verifique se uma [ID da campanha](../collaborate/manage-projects.md#manage-campaign-id) foi fornecida:
   * Se você for um editor, insira a ID da campanha vinculada à campanha do anunciante.
   * Se você for um anunciante, solicite que seu colaborador (editor) forneça a ID do Campaign. Isso é necessário para [gerar relatórios no espaço de trabalho de Medidas](#create-measurement-report).
* [Carregar dados de medição](/help/guide/setup/onboard-measurement-data.md) no Collaboration se desejar [criar relatórios de Atribuição](#create-attribution-report).

## Exibir relatórios {#view-reports}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report_campaignID"
>title="IDs de campanha"
>abstract="Espaço reservado para adicionar informações relevantes na interface sobre o que são as IDs de campanha."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report"
>title="IDs de campanha"
>abstract="Espaço reservado para adicionar informações relevantes na interface sobre o que são as IDs de campanha."

Para exibir os relatórios disponíveis na guia mensuração:

1. Navegue até **[!UICONTROL Colaborar]** > **[!UICONTROL Meus projetos]**.
2. Para o projeto desejado e selecione **[!UICONTROL Exibir]**.
3. No projeto, selecione a guia **[!UICONTROL Medida]**.

Selecione **[!UICONTROL Exibir relatório completo]** para acessar os vários relatórios disponíveis, detalhados mais abaixo.

![Como acessar a guia de medição em um projeto.](/help/assets/collaborate/measure/measurement.gif)

### Exibição de resumo

A exibição do topo da página na guia Measurement mostra um resumo da campanha com alguns números de alto nível que você pode consultar:

**[!UICONTROL Impressões]**: o número total de vezes que o criativo foi exibido.
**[!UICONTROL Alcance único]**: o número de identidades individuais que viram o criativo.
**[!UICONTROL Frequência média total]**: o número de impressões dividido por identidades exclusivas foi atingido. Este número indica com que frequência cada identidade foi exibida pelo criativo.

![Exibição do resumo da campanha](/help/assets/collaborate/measure/campaign-summary.png)

### Métricas ao longo do tempo {#metrics-over-time}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measure_metricsovertime"
>title="Métricas ao longo do tempo"
>abstract="Use a exibição métricas ao longo do tempo para entender o número total de impressões exibidas à equipe de criação durante todo o período da campanha. É possível selecionar um máximo de duas dimensões para exibir no relatório."

Use a exibição métricas ao longo do tempo para entender o número total de impressões exibidas à equipe de criação durante todo o período da campanha. Observe que é possível selecionar no máximo duas métricas para exibir e analisar no relatório.

![Métricas ao longo da exibição de tempo.](/help/assets/collaborate/measure/metrics-over-time.png)

### Distribuição de frequência {#frequency-distribution}

Use a exibição de distribuição de frequência para entender o detalhamento de quantas impressões foram mostradas para cada usuário único. Essa exibição pode ajudá-lo em campanhas futuras a decidir a partir de qual ponto você deseja começar a suprimir públicos. Por exemplo, talvez você queira suprimir perfis que já viram um criativo três vezes.

![Modo de exibição de distribuição de frequência.](/help/assets/collaborate/measure/frequency-distribution.gif)

### Métrica por dimensão {#metric-by-dimension}

Analise diferentes métricas, como impressões, impressões visualizáveis, alcance exclusivo, custo e muito mais, no contexto da mídia de posicionamento. Analise qual mídia (por exemplo, transmissão móvel, CTV programática ou outras) está gerando os melhores resultados para suas campanhas.

![Métrica por dimensão.](/help/assets/collaborate/measure/metric-by-dimension.png)

### Curva de alcance cumulativo {#cumulative-reach-curve}

Conforme a campanha avançava e o número de impressões aumentava, entenda se o número de usuários que você conseguia alcançar também aumentou. Um padrão comum em campanhas é que, após um determinado ponto, um plateau é atingido, onde o criativo é exibido para as mesmas pessoas repetidamente. Essa visualização pode ajudá-lo a ajustar a duração das campanhas futuras, dependendo do momento em que novas pessoas não estão mais sendo atingidas.

![Curva de alcance cumulativa.](/help/assets/collaborate/measure/cumulative-reach-curve.png)

### Impressões por posicionamento {#impressions-by-placement}

Entenda qual mídia está gerando impressões para o seu criativo. Isso pode ajudá-lo a decidir onde investir seu investimento em anúncios em campanhas futuras.

![Impressões por posicionamento.](/help/assets/collaborate/measure/impressions-by-placement.png)

### Conversões cumulativas {#cumulative-conversions}

Essa visualização fornece um detalhamento dos eventos de conversão que você escolhe medir em formato tabular. A tabela inclui:

* **Evento de conversão**: nome de cada evento de conversão que você está rastreando.
* **Contagem de conversão**: Contagem total de conversões que ocorreram para cada evento.
* **Receita estimada**: valor estimado atribuído a cada evento de conversão.

Consulte esta tabela para avaliar a eficácia da campanha na condução das ações desejadas.

![Conversões cumulativas.](/help/assets/collaborate/measure/cumulative-conversions.png)

### Conversões por dia {#conversions-by-day}

Este gráfico fornece um detalhamento diário das conversões para cada evento configurado ao criar um relatório de Atribuição. Use essa exibição para descobrir padrões diários, identificar períodos de atividade de conversão alta ou baixa e comparar o desempenho de diferentes eventos de conversão na linha do tempo da campanha.

![Conversões por dia.](/help/assets/collaborate/measure/conversions-by-day.gif)

## Criar relatório de medição {#create-measurement-report}

No Collaboration, você pode criar dois tipos principais de relatórios de medição:

* **Resumo da campanha**: fornece métricas de alto nível, como alcance, impressões, frequência média e entrega por canal, fornecendo uma visão geral rápida do desempenho geral da campanha.
* **Atribuição**: mede como as exposições da campanha direcionam as ações downstream, como conversões ou compras, ajudando você a entender a eficácia da campanha.

Você pode executar o relatório de Resumo da campanha por conta própria, enquanto o relatório de Atribuição requer que ambos os tipos de relatório sejam selecionados juntos.

### Criar relatório de resumo da campanha {#create-campaign-summary-report}

Tanto editores quanto anunciantes podem gerar relatórios do **Resumo da campanha** para avaliar o desempenho da campanha. Use esses relatórios para obter insights sobre métricas principais, como [alcance](#cumulative-reach-curve), [frequência](#frequency-distribution) e [impressões](#impressions-by-placement), e entender como sua campanha foi entregue e seu impacto geral.

Para gerar um relatório de **Resumo da Campanha**, navegue até o espaço de trabalho de projeto a partir do espaço de trabalho **[!UICONTROL Colaborador]**. Na guia **[!UICONTROL Medida]**, selecione o ícone adicionar (![Ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Medida]**.

Se este for seu primeiro relatório, você também poderá selecionar a opção **[!UICONTROL Executar relatório]**.

![A guia Measure destacando a opção Executar relatório e a opção Measure.](/help/assets/collaborate/measure/run-measure-report.png)

A tela **[!UICONTROL Criar relatório de medição]** aparece com informações e campos de entrada agrupados nas seções **[!UICONTROL Detalhes do faturamento]**, **[!UICONTROL Detalhes da campanha]** e **[!UICONTROL Detalhes do relatório]**.

#### Detalhes de faturamento {#billing-details}

Esta seção explica como os créditos são usados ao gerar relatórios de mensuração. A responsabilidade de crédito é estabelecida durante a [configuração de conexão](../connect/establishing-connections.md#credit-split). Antes de executar qualquer relatório, revise e confirme as configurações de divisão de crédito e as funções de relatório com seu colaborador.

#### Detalhes da campanha {#campaign-details}

Na seção **[!UICONTROL Detalhes da campanha]**, selecione a **ID do anunciante** apropriada para associar ao seu relatório. Esses nomes ou IDs de anunciante foram adicionados durante a [configuração da conexão](../connect/establishing-connections.md#advertiser-names). Se apenas um nome tiver sido configurado, ele será exibido por padrão. Se nenhum nome for configurado, o campo **[!UICONTROL ID do anunciante (Nome)]** será desabilitado e preenchido com o nome da conta do anunciante.

![A tela Criar relatório de medição mostrando a opção ID (Nome) do Anunciante desabilitada.](/help/assets/collaborate/measure/advertiser-id.png)

Em seguida, selecione a campanha desejada no menu suspenso **[!UICONTROL ID de campanha]**. Esse menu lista todas as IDs de campanha inseridas pelo editor para o seu projeto. Se a campanha necessária não estiver disponível, [adicione-a à interface](./manage-projects.md#manage-campaign-id) antes de gerar o relatório.

![A tela Criar relatório de medição mostrando o menu suspenso ID de Campanha expandido.](/help/assets/collaborate/measure/campaign-id.png)

Em seguida, especifique o período que deseja que o relatório cubra. Selecione **[!UICONTROL Intervalo de datas do relatório]** e use o calendário para escolher as datas de início e término.

![A tela Criar relatório de medição mostrando o calendário de intervalo de datas do Relatório.](/help/assets/collaborate/measure/report-date-range.png)

#### Detalhes do relatório {#report-details}

**Data de execução do relatório**

Na seção **[!UICONTROL Detalhes do relatório]**, escolha a data em que o relatório deve ser executado. Selecione **[!UICONTROL Data de execução do relatório]** e escolha sua data preferida no calendário.

* Se você escolher a data de hoje ou uma data no passado, o relatório **Resumo da campanha** será executado imediatamente.
* Se você escolher uma data futura, o relatório de **Resumo da campanha** será executado nesse dia.

![A tela Criar relatório de medição mostrando o calendário de datas de execução do Relatório.](/help/assets/collaborate/measure/report-run-date.png)

**Tipo de relatório**

* Se você for um anunciante, poderá selecionar o tipo de relatório **[!UICONTROL Resumo da campanha]** dentre as opções disponíveis. Somente anunciantes podem gerar relatórios de atribuição.
* Se você for um editor, o tipo de relatório **[!UICONTROL Resumo da campanha]** será pré-selecionado e não poderá ser alterado. No momento, os editores não podem executar relatórios de atribuição.

![A tela Criar relatório de medição mostrando a opção Resumo da campanha como um tipo de relatório pré-selecionado e inalterável.](/help/assets/collaborate/measure/cs-report-type.png)

Por fim, revise suas configurações e selecione **[!UICONTROL Criar]**. O relatório de resumo da campanha é gerado imediatamente se a data de execução for hoje ou anterior, ou na data futura escolhida. Você pode editar o relatório agendado antes de sua data de execução. Para obter instruções passo a passo, consulte a seção [Editar relatório de medição].

Assim que estiver disponível, você poderá exibir seu relatório a qualquer momento na guia **[!UICONTROL Medida]** do espaço de trabalho do projeto.

![A tela Criar relatório de medição mostrando as informações e a opção Criar realçada.](/help/assets/collaborate/measure/cs-review.png)

### Criar relatório de atribuição {#create-attribution-report}

Como anunciante, você pode gerar relatórios de **Atribuição** para avaliar como as exposições da sua campanha contribuem para os principais resultados, como inscrições ou compras. Use esses relatórios para entender as interações do usuário com sua campanha, identificar quais pontos de contato causam mais impacto e informar estratégias de marketing mais eficazes.

>[!IMPORTANT]
>
> Você deve [originar seus dados de medição](../setup/onboard-measurement-data.md#add-measurement-data) no Collaboration antes de gerar relatórios de Atribuição.
>![A guia Measure com os requisitos para Dados de medição e a opção Measure desabilitada.](/help/assets/collaborate/measure/require-measurement-data.png)

Para gerar um relatório de **Atribuição**, navegue até o espaço de trabalho de projeto a partir do espaço de trabalho **[!UICONTROL Colaborador]**. Na guia **[!UICONTROL Medida]**, selecione o ícone adicionar (![Ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Medida]**.

Se este for seu primeiro relatório, você também poderá selecionar a opção **[!UICONTROL Executar relatório]**.

![A guia Measure destacando a opção Executar relatório e a opção Measure.](/help/assets/collaborate/measure/run-measure-report-attribution.png)

A tela **[!UICONTROL Criar relatório de medição]** aparece com informações e campos de entrada agrupados nas seções **[!UICONTROL Detalhes do faturamento]**, **[!UICONTROL Detalhes da campanha]** e **[!UICONTROL Detalhes do relatório]**.

Leia e siga as etapas na seção [Criar relatório de resumo da campanha](#create-campaign-summary-report) para definir as seguintes configurações:

* [Detalhes de cobrança](#billing-details)
* [Detalhes da campanha](#campaign-details)

#### Detalhes do relatório para relatórios de Atribuição {#report-details-attribution}

**Data de execução do relatório**

>[!IMPORTANT]
>
> Para relatórios de atribuição, a data de execução do relatório deve ser uma data futura e deve ocorrer pelo menos um dia após a data final do intervalo de datas do relatório mais a duração total da janela de pesquisa definida.
> **Data de execução do relatório ≥ data de término do relatório + janela de retrospectiva + 1**
> 
> Por exemplo, se o intervalo de datas do relatório terminar em 15 de junho e a janela de lookback for de 14 dias, a data de execução do relatório será 30 de junho ou posterior.

Na seção **[!UICONTROL Detalhes do relatório]**, escolha a data em que o relatório deve ser executado. Selecione **[!UICONTROL Data de execução do relatório]** e escolha sua data preferida no calendário.

**Tipo de relatório**

Como anunciante, você pode selecionar **[!UICONTROL Atribuição]** como tipo de relatório além de **[!UICONTROL Resumo da campanha]**. Ao escolher o relatório de Atribuição, seus resultados incluem métricas padrão do Resumo da campanha e uma análise de Atribuição detalhada, fornecendo uma visualização abrangente do desempenho da campanha.

![A tela Criar relatório de medição destacando os tipos de relatório Resumo da campanha e Atribuição selecionados.](/help/assets/collaborate/measure/attribution-report-type.png)

Ao selecionar **[!UICONTROL Atribuição]** como o tipo de relatório, uma seção de configuração **[!UICONTROL Atribuição]** é exibida com as configurações adicionais necessárias:

* **Janela de retrospectiva em dias**: define até que ponto o relatório considera as impressões da campanha antes de cada conversão. Somente impressões nesse período têm direito a crédito de atribuição.
* **Eventos de conversão**: especifica quais ações de conversão você deseja medir, por exemplo, compras ou inscrições. Esses eventos devem ser configurados com antecedência quando você [origina seus dados de medição](../setup/onboard-measurement-data.md#add-conversion-event) na Collaboration.

Primeiro, insira um valor para o campo **[!UICONTROL Janela de pesquisa em dias]** ou ajuste-o com as opções de incremento/decremento.

![A tela Criar relatório de medição destacando o valor da janela de pesquisa em dias.](/help/assets/collaborate/measure/lookback-window-in-days.png)

Em seguida, escolha até **3** eventos de conversão na lista disponível. Para obter mais informações sobre um evento específico, selecione o ícone **[!UICONTROL i]** para exibir seus detalhes.

![A tela Criar relatório de medição destacando os eventos de conversão selecionados e as informações do evento Compra.](/help/assets/collaborate/measure/attribution-conversion-events.png)

Por fim, revise suas configurações e selecione **[!UICONTROL Criar]** para agendar o relatório. Seu relatório de atribuição será gerado na data de execução especificada. Você pode editar o relatório agendado antes de sua data de execução. Para obter instruções passo a passo, consulte a seção [Editar relatório de medição].

Assim que estiver disponível, você poderá exibir seu relatório a qualquer momento na guia **[!UICONTROL Medida]** do espaço de trabalho do projeto.

![A tela Criar relatório de medição mostrando as informações e a opção Criar realçada.](/help/assets/collaborate/measure/attribution-review.png)
