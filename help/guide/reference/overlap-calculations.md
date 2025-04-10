---
title: Cálculo de contagens e porcentagens de sobreposição
description: Entenda como as contagens e porcentagens de sobreposição são calculadas em várias áreas do Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 23dc33af83366806f7d99161b4b713a33daeec76
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---


# Cálculo de contagens e porcentagens de sobreposição

No Adobe Real-Time CDP Collaboration, entender a sobreposição de público é fundamental para otimizar suas estratégias de marketing e garantir uma colaboração eficaz entre anunciantes e editores. Este documento explica como as contagens e porcentagens de sobreposição em várias áreas de produtos são calculadas usando dados de amostra.

## Dados de exemplo - Contagem de identidades

### Pressupostos para Fins de Cálculo

Neste exemplo, considere que:

* O anunciante tem três públicos-alvo (A1, A2, A3).
* O editor tem três públicos-alvo (P1, P2, P3).
* Todas as identidades principais de correspondência são mutuamente exclusivas em todos os públicos-alvo.

>[!NOTE]
>
>Na realidade, haveria alguma sobreposição entre as identidades principais de correspondência de cada público-alvo, mas, para simplificar, este exemplo presume que elas são exclusivas neste caso.

### Públicos-alvo do anunciante

| Públicos-alvo do anunciante | A1 | A2 | A3 | TODOS |
|----------------------|------|------|------|------|
| Identidades de email com hash | 300 K | 450 K | 250 K | 1M |
| Identidades de Liveramp | 500 K | 200 K | 700 K | 1,4 M |
| Contagem total de identidades | 800 K | 650 K | 950 K | 2,4 M |

### Públicos-alvo do editor

| Públicos-alvo do editor | P1 | P2 | P3 | TODOS |
|---------------------|------|------|------|------|
| Identidades de email com hash | 150 K | 600 K | 550 K | 1,3M |
| Identidades de Liveramp | 400 K | 350 K | 100 mil | 850 K |
| Contagem total de identidades | 550 K | 950 K | 800 K | 2,3M |

## Calcular contagens e porcentagens de sobreposição

### Dados de exemplo - Contagem de sobreposição

#### Anunciante cada vs Editor cada

|                     | A1 - P1 | A2 - P2 | A3 - P3 |
|---------------------|---------|---------|---------|
| Sobreposição por email com hash | 100 mil | 300 K | 150 K |
| Sobreposição por ID de Liveramp | 200 K | 150 K | 50 K |
| Sobreposição total | 300 K | 450 K | 200 K |

#### Anunciante cada vs. Editor TODOS

|                     | A1 - P ALL | A2 - P ALL | A3 - P ALL |
|---------------------|------------|------------|------------|
| Sobreposição por email com hash | 250 K | 400 K | 200 K |
| Sobreposição por ID de Liveramp | 350 K | 150 K | 230 K |
| Sobreposição total | 600 K | 550 K | 430 K |

#### Anunciante ALL vs Editor Each

|                     | A TUDO - P1 | A TUDO - P2 | A TUDO - P3 |
|---------------------|------------|------------|------------|
| Sobreposição por email com hash | 120 K | 530 K | 200 K |
| Sobreposição por ID de Liveramp | 350 K | 330 K | 50 K |
| Sobreposição total | 470 K | 860 K | 250 K |

#### Anunciante TODOS vs Editor TODOS

|                     | A TUDO - P ALL |
|---------------------|---------------|
| Sobreposição por email com hash | 850 K |
| Sobreposição por ID de Liveramp | 730 K |
| Sobreposição total | 1,58 M |

## Módulo Discover

O módulo **[!UICONTROL Discover]** no Adobe Real-Time CDP Collaboration fornece informações valiosas sobre os dados do público-alvo. Ao entender as sobreposições de público-alvo, é possível identificar oportunidades potenciais de colaboração entre editores e anunciantes. A seção **[!UICONTROL Insights de Público-alvo]** do módulo **[!UICONTROL Discover]** ajuda a analisar as contagens e porcentagens de sobreposição entre públicos-alvo diferentes.

![O módulo de descoberta do fluxo de trabalho de colaboração.](/help/assets/reference/overlap-calculations/discover-module-overlap-calculations.png)

Veja abaixo exemplos de cálculos e fórmulas para vários cenários de sobreposição.

### Todos os públicos-alvo do anunciante e todos os públicos-alvo do editor

| Públicos-alvo do anunciante | Públicos-alvo do editor | Contagem de identidade (A) | Identidades Sobrepostas (B) | Percentual de sobreposição | Detalhamento da chave de correspondência | % de Detalhamento da Chave de Correspondência |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| TODOS | TODOS | Contagem total de identidades de TODOS os públicos-alvo do anunciante <br> Contagem de identidades = 1M + 1,4M = 2,4M | Sobreposição total entre TODOS os públicos-alvo do anunciante e TODOS os públicos-alvo do publicador para todas as chaves de correspondência <br> Identidades sobrepostas = 1,58 M | Porcentagem de identidades sobrepostas em relação à contagem total de identidades de TODOS os públicos-alvo do anunciante <br> % de sobreposição = (B / A) * 100 = (1,58 M / 2,4 M) * 100 = 65,83% <br> Porcentagem de sobreposição = 65,83% | Sobreposição de identidades por chave de correspondência <br> Sobreposição por email com hash = 850K <br> Sobreposição por ID de Liveramp = 730K | Porcentagem de sobreposição de chave de correspondência em relação ao total de identidades sobrepostas <br> % de chave de correspondência para email com hash = (850K / 1,58M) * 100 = 53,8% <br> para ID de Liveramp = (730K / 1,58M) * 100 = 46,2% |

### Todos os públicos-alvo do anunciante e um público-alvo do editor

| Públicos-alvo do anunciante | Públicos-alvo do editor | Contagem de identidade (A) | Identidades Sobrepostas (B) | Percentual de sobreposição | Detalhamento da chave de correspondência | % de Detalhamento da Chave de Correspondência |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| TODOS | 1 P2 | Contagem total de identidades de todos os públicos-alvo do anunciante <br> Contagem de identidades = 1M + 1,4M = 2,4M | Sobreposição total entre TODOS os públicos-alvo do anunciante e o público-alvo do publicador selecionado P2 para todas as chaves de correspondência <br> Identidades sobrepostas = 860K | Porcentagem de identidades sobrepostas em relação à contagem total de identidades de TODOS os públicos-alvo do anunciante <br> % de sobreposição = (B / A) * 100 = (860K / 2,4M) * 100 = 35,83% <br> Porcentagem de sobreposição = 35,83% | Sobreposição de identidades por chave de correspondência <br> Sobreposição por email com hash = 530K <br> Sobreposição por ID de Liveramp = 330K | Porcentagem de sobreposição de chave de correspondência em relação ao total de identidades sobrepostas <br> % de chave de correspondência para email com hash = (530K / 860K) * 100 = 61,62% <br> para ID de Liveramp = (330K / 860K) * 100 = 38,38% |

### Um público-alvo de anunciante e todos os públicos-alvo de editores

| Públicos-alvo do anunciante | Públicos-alvo do editor | Contagem de identidade (A) | Identidades Sobrepostas (B) | Percentual de sobreposição | Detalhamento da chave de correspondência | % de Detalhamento da Chave de Correspondência |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| 1 A1 | TODOS | Contagem total de identidades do público-alvo selecionado pelo anunciante A1 <br> Contagem de identidades = 300 K + 500 K = 800 K | Sobreposição total entre o público-alvo do anunciante A1 e TODOS os públicos-alvo do publicador para todas as chaves de correspondência <br> Identidades sobrepostas = 600K | Porcentagem de identidades sobrepostas em relação à contagem de identidades do público-alvo selecionado pelo anunciante (A1) <br> % de sobreposição = (B / A) * 100 = (600 K / 800 K) * 100 = 75% <br> Porcentagem de sobreposição = 75% | Sobreposição de identidades por chave de correspondência <br> Sobreposição por email com hash = 250K <br> Sobreposição por ID de Liveramp = 350K | Porcentagem de sobreposição de chave de correspondência em relação ao total de identidades sobrepostas <br> % de chave de correspondência para email com hash = (250K / 600K) * 100 = 41,67% <br> para ID de Liveramp = (350K / 600K) * 100 = 58,33% |

### Um público-alvo de anunciante e um público-alvo de editor

| Públicos-alvo do anunciante | Públicos-alvo do editor | Contagem de identidade (A) | Identidades Sobrepostas (B) | Percentual de sobreposição | Detalhamento da chave de correspondência | % de Detalhamento da Chave de Correspondência |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| 1 A2 | 1 P2 | Contagem total de identidades do público-alvo selecionado pelo anunciante A2 <br> Contagem de identidades = 450 K + 200 K = 650 K | Sobreposição total entre o público-alvo do anunciante selecionado A2 e o público-alvo do publicador selecionado P2 para todas as chaves de correspondência <br> Identidades sobrepostas = 450K | Porcentagem de identidades sobrepostas sobre a contagem de identidades do público selecionado (A2) <br> % de sobreposição = (B / A) * 100 = (450 K / 650 K) * 100 = 69,23% <br> Porcentagem de sobreposição = 69,23% | Sobreposição de identidades por chave de correspondência <br> Sobreposição por email com hash = 300K <br> Sobreposição por ID de Liveramp = 150K | Porcentagem de sobreposição de chave de correspondência em relação ao total de identidades sobrepostas <br> % de chave de correspondência para email com hash = (300K / 450K) * 100 = 66,67% <br> para ID de Liveramp = (150K / 450K) * 100 = 33,33% |
