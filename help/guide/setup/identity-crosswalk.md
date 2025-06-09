---
title: Passarelas de Identificação
description: Saiba tudo sobre faixas de cruzamento de identidade no Real-Time CDP Collaboration, incluindo como trazer faixas de cruzamento de identidade de diferentes fontes e como gerenciar faixas de cruzamento de identidade
audience: admin, publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
hidefromtoc: true
hide: true
exl-id: a51f112d-3da7-4482-a24a-6d9f269d28d1
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 20%

---

# Passarelas de Identificação

{{limited-availability-release-note}}

Saiba tudo sobre faixas de cruzamento de identidade no Real-Time CDP Collaboration, incluindo como trazer faixas de cruzamento de identidade de diferentes fontes e como gerenciar faixas de cruzamento de identidade.

As passarelas de identificação facilitam a vinculação segura e compatível com a privacidade das identidades do cliente em vários conjuntos de dados e plataformas. Utilizando identificadores com hash, o Real-Time CDP Collaboration garante que os usuários possam sincronizar e reconciliar identidades sem expor informações pessoais identificáveis (PII). Isso permite uma visualização unificada do cliente para melhor colaboração e esforços de marketing direcionados.

<!--
In Real-Time CDP Collaboration, use identity crosswalks alongside your audiences by [TODO] insert material here. 
-->


Como primeiro passo, você deve importar as travessias de identidade para o Real-Time CDP Collaboration. Para importar as travessias de identidade para o Real-Time CDP Collaboration, leia a seção abaixo:

>[!NOTE]
>
>Na versão beta do Real-Time CDP Collaboration, você pode importar faixas de cruzamento de identidade de seus conjuntos de dados na Real-Time CDP. Outras opções estarão disponíveis nas versões subsequentes.

## Importação de travessias de identidade para o Real-Time CDP Collaboration {#import-crosswalk}

Navegue até a guia **[!UICONTROL Configuração]** > **[!UICONTROL Cruzamentos de identidade]**, selecione o ícone adicionar (![Ícone Adicionar.](/help/assets/icons/plus.png)) e selecione **[!UICONTROL Passarela de Identidade]**

![Gravação de como chegar à tela para adicionar faixas de pedestres de identidade](/help/assets/setup/identity-crosswalks/import-identity-crosswalk.gif)

### Selecionar origem da faixa de pedestres

Selecione uma fonte da qual você importará a faixa de cruzamento de identidade. Na primeira versão do Real-Time CDP Collaboration, o Experience Platform é a única fonte compatível para a importação de faixas de pedestres.

>[!TIP]
>
>As travessias que você está importando do Experience Platform são chamadas de *conjuntos de dados* na Platform.

Depois de selecionar o Experience Platform como origem das suas passarelas, selecione a [sandbox do Experience Platform](https://experienceleague.adobe.com/pt-br/docs/experience-platform/sandbox/home) da qual você está importando a passarela de identidade.

![Gravação de como selecionar uma fonte de faixa de pedestres](/help/assets/setup/identity-crosswalks/select-crosswalk-source.gif)

### Selecionar faixa de pedestres

Depois de selecionar o Experience Platform como fonte das suas passarelas,

### Fornecer detalhes

Forneça um nome e uma descrição para a faixa de cruzamento de identidade que você está importando para o produto.

### Selecionar chave de associação {#select-join-key}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_crosswalk_join_key"
>title="Chave de associação"
>abstract="Uma chave de associação é um identificador exclusivo usado para corresponder e vincular registros em diferentes conjuntos de dados. Ela garante que os dados de várias fontes possam ser associados com precisão ao mesmo indivíduo ou entidade. Qualquer um dos cabeçalhos de coluna da faixa de cruzamento selecionada pode servir como chave de associação."

Uma chave de associação é um identificador exclusivo usado para corresponder e vincular registros em diferentes conjuntos de dados. Ela garante que os dados de várias fontes possam ser associados com precisão ao mesmo indivíduo ou entidade. Ao selecionar a chave de junção apropriada, você pode mesclar e reconciliar dados de maneira eficaz, melhorando a precisão e a integridade de suas campanhas.

Qualquer um dos cabeçalhos de coluna da faixa de cruzamento selecionada pode servir como chave de associação.

Selecione a chave de junção desejada para a tabela de faixas e selecione **[!UICONTROL Avançar]** para prosseguir para a próxima etapa.

### Revisar

Revise qualquer uma das seleções nas telas anteriores. Quando satisfeito com sua seleção, selecione **[!UICONTROL Avançar]** para concluir o fluxo de trabalho.

## Próximas etapas

Depois de aprender a importar passadas de identidade para o Real-Time CDP, você pode visualizar todas as passadas de identidade adicionadas até agora ao Real-Time CDP Collaboration. Agora também é possível usar as faixas de cruzamento de identidade importadas ao importar públicos para o Real-Time CDP Collaboration.
