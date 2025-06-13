---
title: Medir desempenho
description: Meça o desempenho de suas campanhas em diferentes canais. Saiba como usar e interpretar vários relatórios.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: b52fd181d80d5a70331571f7a4cbe3e5a7ec1d7c
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 18%

---

# Medir desempenho

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>O espaço de trabalho **[!UICONTROL Medida]** só estará disponível se o caso de uso **Medida** tiver sido habilitado [durante o processo de conexão](../connect/establishing-connections.md#connection-settings). Para obter mais informações sobre casos de uso, consulte o guia [gerenciar projetos](./manage-projects.md#project-use-cases).

Saiba mais sobre os relatórios disponíveis no Real-Time CDP Collaboration e entenda como medir e analisar o desempenho de suas campanhas de marketing em vários canais.

## Pré-requisitos

Antes de acessar os relatórios de medição no Real-Time CDP Collaboration, você já deve:

* [Conectado](/help/guide/connect/establishing-connections.md) com um anunciante ou editor desejado com o caso de uso **Medição** habilitado e começou a colaborar em [projetos](/help/guide/collaborate/manage-projects.md)
* Execute uma campanha e [carregue os dados de medição](/help/guide/setup/onboard-measurement-data.md) no Real-Time CDP Collaboration.

<!--

## Create a report {#create-report}

Hidden until functionality is live. At that point, move the contextualhelp from below into this section. 

The syntax rtcdp_collaboration_measurement_create_report is currently implemented in the UI. However, a preference would be to imlement the other contextualhelp ID from below instead, since that explicitly includes campaignID in the syntax. Need to sync up with UI team. More details in CORE-116991.

-->

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

## Próximas etapas

![Descobrir, ativar, medir para anunciantes.](/help/assets/end-to-end-workflow/discover-activate-measure.png)

No espírito do ciclicidade na imagem acima, use os insights que você obteve ao visualizar os relatórios no planejamento da próxima campanha. Como anunciante, se necessário, volte para descobrir diferentes editores e execute sobreposições para descobrir públicos diferentes para as próximas campanhas.
