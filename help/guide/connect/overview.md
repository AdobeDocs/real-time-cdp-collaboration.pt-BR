---
title: Visão geral das conexões
description: Saiba mais sobre conexões no Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="Disponibilidade limitada" type="Informative" url="https://helpx.adobe.com/br/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 5c08738cdc8e1e208203ee1f9a1cf1891b5b07cb
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# Visão geral das conexões

{{limited-availability-release-note}}

Antes que os colaboradores possam trabalhar juntos em campanhas, eles devem estabelecer uma conexão. Essa conexão permite que eles ativem públicos, criem projetos e executem relatórios sobre o desempenho da campanha.

As conexões são estabelecidas com base no padrão de colaboração escolhido. A Collaboration oferece suporte a três principais padrões de colaboração: anunciante-para-publicador, marca-para-marca e anunciante-para-plataforma-de-publicidade. Para ler mais sobre esses padrões, consulte o guia [padrões de colaboração](/help/guide/overview/collaboration-patterns.md).

Para saber como estabelecer uma conexão, leia a seção abaixo que corresponde ao seu padrão de colaboração:

- [Conexão do anunciante com o editor](#advertiser-to-publisher-connection)
- [Conexão marca a marca](#brand-to-brand-connection)
- [Conexão do anunciante com a plataforma de publicidade](#advertiser-to-advertising-platform-connection)

## Conexão do anunciante com o editor {#advertiser-to-publisher-connection}

![Diagrama de alto nível do processo de conexão anunciante-publicador.](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

No padrão anunciante para editor, um anunciante descobre um editor com o qual deseja trabalhar por meio do espaço de trabalho **[!UICONTROL Descobrir editores]** e envia um convite de conexão. O editor então revisa o convite e o aceita, permitindo que o anunciante proponha configurações de conexão. Quando o editor aceita as configurações de conexão, a conexão é estabelecida e ambos os colaboradores podem começar a trabalhar juntos nos projetos.

### Visão geral de alto nível

Para estabelecer uma conexão entre um anunciante e um editor, as seguintes etapas estão envolvidas:

1. [Descobrir editores](./discover-collaborators.md): o anunciante identifica possíveis editores com os quais colaborar.
2. [Enviar convite](./establishing-connections.md#send-invite): o anunciante envia um convite de conexão para o editor selecionado.
3. [Aceitar convite](./establishing-connections.md#accept-invite): o editor revisa e aceita o convite.
4. [Definir configurações de conexão](./establishing-connections.md#configure-connection-settings): o anunciante define as configurações de conexão e as envia ao editor para revisão.
5. [Confirmar configurações de conexão](./establishing-connections.md#review-connection-settings): o publicador revisa as configurações de conexão e as aceita ou rejeita. Se aceita, a conexão é estabelecida. Se rejeitado, o editor pode fornecer feedback para revisões fora do produto. O anunciante poderá então revisar as configurações e reenviá-las para revisão.

Depois que as configurações de conexão forem aceitas, a conexão será estabelecida e os colaboradores estarão prontos para [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para começar a colaborar em campanhas.

## Conexão marca a marca {#brand-to-brand-connection}

![Diagrama de alto nível do processo de conexão marca a marca.](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>O termo **marca** é usado para se referir a uma empresa ou marca fora da Collaboration. O termo **colaborador** se refere a qualquer conta que possa formar uma conexão no Collaboration, independentemente de ser um anunciante ou um editor.

No padrão marca a marca, duas marcas que se comunicaram fora do produto podem se conectar diretamente ao Collaboration usando um [convite de conexão privada](#private-connection-invite). Uma marca pode ser um anunciante ou um editor. Esse padrão é particularmente útil para marcas que podem não se encaixar no modelo tradicional de anunciante-editor, como dois anunciantes ou dois editores.

Para começar, um colaborador envia um convite de conexão privada para outro colaborador. O recipient revisa o convite e o aceita, permitindo que o proprietário proponha configurações de conexão. Depois que o recipient aceitar as configurações de conexão, a conexão será estabelecida e ambos os colaboradores poderão começar a trabalhar juntos nos projetos.

### Visão geral de alto nível

>[!TIP]
>
>Ao discutir o processo de conexão, haverá uma distinção entre **proprietário** e **destinatário**. O proprietário é o colaborador que inicia a conexão enviando o convite, enquanto o destinatário é o colaborador que recebe e revisa o convite.

O processo de conexão entre duas marcas envolve várias etapas. Antes de o processo de conexão começar, alguns pré-requisitos devem ser atendidos:

1. Duas marcas se comunicam fora do produto para discutir a conexão potencial.
1. As marcas [criam contas](/help/guide/setup/onboard-account.md) na Collaboration, se ainda não o fizeram, certificando-se de selecionar o tipo de função apropriado (anunciante ou editor).

Depois que os pré-requisitos forem atendidos, o processo de conexão poderá ser iniciado. As etapas a seguir descrevem o processo:

1. [Enviar convite de conexão privada](./establishing-connections.md#private-connection-invite): um colaborador envia um convite de conexão privada para outro colaborador.
2. [Aceitar convite de conexão privada](./establishing-connections.md#accept-invite): o destinatário revisa e aceita o convite de conexão privada.
3. [Definir configurações de conexão](./establishing-connections.md#configure-connection-settings): o proprietário define as configurações de conexão e as envia ao destinatário para revisão e aceitação.
4. [Confirmar configurações da conexão](./establishing-connections.md#review-connection-settings): o destinatário revisa as configurações da conexão e as aceita ou rejeita.

Depois que as configurações de conexão forem aceitas, a conexão será estabelecida e os colaboradores estarão prontos para [criar um projeto](/help/guide/collaborate/manage-projects.md#create-project) para começar a colaborar em campanhas.

## Conexão do anunciante com a plataforma de publicidade {#advertiser-to-advertising-platform-connection}

O processo de conexão anunciante-plataforma de publicidade permite que os anunciantes se conectem a plataformas de publicidade de terceiros, como Amazon Marketing Cloud (AMC), para aprimorar seus recursos de marketing.

### Visão geral de alto nível

O processo de conexão entre um anunciante e uma plataforma de publicidade envolve várias etapas. Antes do início do processo de conexão, verifique se você tem uma conta ativa com a plataforma de publicidade e se está aprovado para usar os serviços. As etapas a seguir descrevem o processo de conexão:

1. [Descubra plataformas de publicidade](./discover-collaborators.md): o anunciante identifica plataformas de publicidade em potencial com as quais colaborar.
2. [Conectar-se à plataforma de publicidade](./advertising-platforms/overview.md#advertising-platforms-overview): o anunciante inicia o processo de conexão selecionando a plataforma de publicidade à qual deseja se conectar e segue as instruções para autenticar e autorizar a conexão.
