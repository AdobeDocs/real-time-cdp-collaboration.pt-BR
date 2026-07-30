---
title: Requisitos de conexão de destino
description: Revise as informações de conexão necessárias para configurar os destinos compatíveis com o Real-Time CDP Collaboration.
audience: admin, publisher
source-git-commit: c84582bb81289ce761c664af7db177535ff00a00
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# Requisitos de conexão de destino

Antes de configurar um destino no Real-Time CDP Collaboration, obtenha as credenciais e as informações de conexão exigidas pelo provedor de destino.

Esta página resume os métodos de autenticação disponíveis no Collaboration. Para obter instruções sobre como criar credenciais, atribuir permissões, configurar o acesso à rede ou preparar o sistema de destino, consulte a documentação de destino vinculada do Adobe Experience Platform.

>[!NOTE]
>
>A documentação vinculada do Adobe Experience Platform descreve o workflow padrão de destino. Algumas etapas, campos ou opções podem não se aplicar ao configurar o destino no Real-Time CDP Collaboration.

## Principais características dos requisitos {#requirements-at-a-glance}

| Destino | Método de autenticação ou conexão | Preparar antes de iniciar | Requisitos detalhados |
|---|---|---|---|
| [!DNL Amazon S3] | Chave de acesso e chave secreta, ou função assumida | Par de chaves de acesso do AWS ou função ARN do IAM; informações do bucket e da pasta | [[!DNL Amazon S3] documentação de destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3) |
| SFTP | Senha ou chave SSH | Domínio do servidor, porta, nome de usuário, credencial de autenticação e caminho da pasta | [Documentação de destino SFTP](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/sftp) |
| [!DNL Azure Blob Storage] | String de conexão | Informações sobre a cadeia de conexão de armazenamento, o container e a pasta do Azure | [[!DNL Azure Blob Storage] documentação de destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob) |
| [!DNL Google Cloud Storage] | ID da chave de acesso e chave de acesso secreta | [!DNL Google Cloud Storage] credenciais de interoperabilidade, bucket e informações de pasta | [[!DNL Google Cloud Storage] documentação de destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage) |
| [!DNL Snowflake Batch] | Compartilhamento de dados do [!DNL Snowflake] | [!DNL Snowflake] ID da conta, região, status de Link Privado e acesso a listagens privadas | [[!DNL Snowflake Batch] documentação de destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch) |
| [!DNL Data Landing Zone] | Não é necessária uma autenticação separada | Preferências de caminho da pasta de destino e saída de arquivo | [[!DNL Data Landing Zone] documentação de destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone) |

## Notas do conector {#connector-notes}

Analise os seguintes métodos de autenticação específicos do conector e as diferenças do fluxo de trabalho antes de configurar um destino.

### [!DNL Amazon S3] {#amazon-s3}

O Collaboration oferece suporte à autenticação **[!UICONTROL Chave de Acesso]** e **[!UICONTROL Função Presumida]**. A autenticação da chave de acesso exige uma chave de acesso e uma chave de acesso secreta. A autenticação de função assumida requer o ARN de uma função do AWS IAM que a Adobe possa assumir.

Para configuração de credenciais, funções e permissões, consulte [Autenticar no [!DNL Amazon S3] destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3#authenticate).

### SFTP {#sftp}

A Collaboration oferece suporte a **[!UICONTROL SFTP com Senha]** e **[!UICONTROL SFTP com autenticação de Chave SSH]**. Ambos os métodos exigem o domínio, a porta e o nome de usuário do servidor. A porta padrão é `22`.

Para obter os requisitos de formato de chave SSH, servidor, rede e incluo na lista de permissões, consulte [informações de autenticação SFTP](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/sftp#authentication-information).

### [!DNL Azure Blob Storage] {#azure-blob-storage}

O Collaboration é autenticado em [!DNL Azure Blob Storage] usando uma cadeia de conexão de conta de armazenamento.

Para obter instruções sobre como obter a cadeia de conexão e atribuir permissões de armazenamento, consulte [Autenticar no [!DNL Azure Blob Storage] destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob#authenticate).

### [!DNL Google Cloud Storage] {#google-cloud-storage}

O Collaboration requer uma ID de chave de acesso [!DNL Google Cloud Storage] e uma chave de acesso secreta geradas pelas configurações de interoperabilidade [!DNL Google Cloud Storage].

Para obter os requisitos de geração de credenciais e permissão de bucket, consulte [Autenticar no [!DNL Google Cloud Storage] destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage#authenticate).

### [!DNL Snowflake Batch] {#snowflake-batch}

[!DNL Snowflake Batch] usa compartilhamento de dados [!DNL Snowflake] em vez de exportar arquivos para armazenamento gerenciado pelo cliente. No Collaboration, não há nenhuma etapa de autenticação separada. Insira a ID da conta da Snowflake, a região, o status do Link privado e a confirmação de propriedade da conta durante a criação do destino.

Para saber mais sobre os requisitos de preparação de conta e listagem privada, consulte [[!DNL Snowflake Batch] documentação de destino](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch).

### [!DNL Data Landing Zone] {#data-landing-zone}

[!DNL Data Landing Zone] é provisionado pela Adobe e não requer uma etapa de autenticação separada no Collaboration. Durante a criação do destino, especifique o caminho da pasta de destino e as configurações de saída do arquivo.

Para obter informações sobre como acessar uma [!DNL Data Landing Zone] provisionada pela AWS, consulte [Autenticar para a Zona de Aterrissagem de Dados provisionada pela AWS](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone#authenticate-dlz-aws).

## Próximas etapas {#next-steps}

Após obter as informações de conexão necessárias, [configure e gerencie um destino](./manage-destinations.md).
