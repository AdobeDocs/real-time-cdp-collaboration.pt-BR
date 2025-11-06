---
title: Configurar permissões do AWS para origem do público-alvo
description: Saiba como configurar as permissões do AWS Identity and Access Management (IAM) para conceder ao Adobe acesso seguro e somente leitura ao seu bucket [!DNL Amazon S3] de origem de público-alvo no Real-Time CDP Collaboration.
source-git-commit: 4f223890dabb4897c9e9264655ff9217e323dc91
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Configurar permissões do AWS para fornecimento de público

Use este guia para configurar as políticas e funções do AWS Identity and Access Management (IAM) que concedem ao Adobe acesso seguro e somente leitura ao seu bucket do Amazon S3. Esse acesso permite que o Real-Time CDP Collaboration origine públicos-alvo do seu bucket do S3.

## Pré-requisitos {#prerequisites}

Antes de continuar, confirme se você atende aos requisitos a seguir e tem acesso às informações necessárias.

### Permissões necessárias do AWS

Para concluir essa configuração, sua conta deve ter acesso de administrador do AWS. O acesso do administrador garante que você possa criar e gerenciar as políticas e funções do IAM necessárias para autorizar o acesso da Adobe ao seu bucket do S3. Se você não tiver privilégios de administrador, entre em contato com o administrador do AWS antes de continuar.

### Informações necessárias

Conforme você seguir as etapas abaixo, anote as informações a seguir. Estes detalhes são usados no [[!DNL Amazon S3] guia de interface do usuário para fornecimento de público-alvo](./configure-aws-s3-audience-sourcing.md).

* O nome do bucket do S3 em que os arquivos de público-alvo são armazenados.
* O caminho da pasta (prefixo) no qual os arquivos de público-alvo estão localizados.
* O ARN (Amazon Resource Name) para a sua Função IAM recém-criada, por exemplo: `arn:aws:s3:::my-company-data/audience-files/`

>[!TIP]
>
>Um ARN (Amazon Resource Name) identifica exclusivamente os recursos do AWS, como buckets do S3 e funções IAM. Use o formato a seguir para especificar o bucket e o caminho de pasta opcional:
>
>```
>arn:aws:s3:::<bucket-name>/<optional-folder-path>
>```

## Criar uma política IAM {#create-policy}

Para começar a configuração, primeiro crie uma política IAM que conceda **acesso somente leitura** ao seu bucket S3. Essa política permite que o Adobe leia os arquivos necessários para o fornecimento de público-alvo, mas não concede permissões de gravação ou exclusão.

Abra o [Console de Gerenciamento do AWS](https://aws.amazon.com/console/) e navegue até **[!DNL IAM]** > **[!DNL Policies]** > **[!DNL Create policy]**.

No espaço de trabalho Criar política do AWS, selecione a guia **JSON** e cole a política de exemplo a seguir.

>[!NOTE]
>
>Substitua `<Your AWS ARN for bucket folder path>` e `<Your AWS ARN for bucket>` por seus ARNs S3 específicos. Ao especificar o caminho da pasta do bucket, inclua `/*` no final do ARN (por exemplo, `arn:aws:s3:::my-company-data/audience-files/*`). Isso garante que o Adobe tenha acesso a todos os arquivos e subpastas no caminho de pasta especificado.

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Action": [
        "s3:GetObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": "<Your AWS ARN for bucket folder path>"
    },
    {
      "Sid": "Statement2",
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket"
      ],
      "Resource": "<Your AWS ARN for bucket>"
    }
  ]
}
```

Revise as configurações de política e selecione **[!DNL Create policy]**. Registre o nome da política para uso em uma etapa posterior.

>[!TIP]
>
>Para localizar o nome do bucket e o caminho da pasta, abra o **Console de Gerenciamento do Amazon S3**. Na página **Compartimentos**, selecione o nome do seu compartimento para abri-lo. A exibição **Objetos** lista seus arquivos e pastas, e o caminho na parte superior da página mostra o caminho da pasta atual.

## Criar uma função IAM {#create-role}

Em seguida, crie uma função IAM e defina a função IAM do Real-Time CDP Collaboration AWS como a **entidade confiável**. Isso permite que os serviços da Adobe assumam a função e leiam com segurança seus dados de público-alvo do S3.

Na guia **[!DNL IAM]** do Console de Gerenciamento do Amazon S3, navegue até **[!DNL Roles]** > **[!DNL Create role]**.

Em [!DNL Step 1] do fluxo de trabalho [!DNL Create role], na seção **[!DNL Trusted entity type]**, selecione **[!DNL Custom trust policy]**. Em seguida, no editor **[!DNL Custom trust policy]**, cole o exemplo a seguir e substitua `<Adobe IAM Role ARN>` pelo valor da sua região.

* A ARN de função do Adobe IAM apropriada para sua região:

| Região | ARN de função do Adobe IAM |
|---------|-------------------|
| América do Norte | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-va6-role` |
| Austrália | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-aus3-role` |

Um exemplo de diretiva de confiança:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": {
        "AWS": "<Adobe IAM Role ARN>"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

Revise a política e selecione **Próximo** para continuar.

Na seção [!DNL Step 2] **[!DNL Add permissions]** do fluxo de trabalho [!DNL Create role], procure e anexe a política IAM que você criou [anteriormente](#create-policy). Selecione a política seguida por **[!DNL Next]** para continuar para [!DNL Step 3].

Na seção [!DNL Step 3] **[!DNL Name review, and create - Role details]**, forneça um nome de função (por exemplo, `s3-iam-role`) e uma descrição opcional.

Esta página exibe a política da entidade confiável, o resumo da política de permissões e quaisquer tags adicionadas para organização interna e rastreamento.

Finalmente, selecione **Criar função** para confirmar a configuração.

>[!IMPORTANT]
>
>Você deve registrar o ARN (Amazon Resource Name) após criar a função. Você precisará fornecer a Função IAM ARN durante a etapa **Autenticar sua conexão S3** no fluxo de trabalho [Configurar o AWS S3 para fornecimento de público-alvo](./configure-aws-s3-audience-sourcing.md).

## Próximas etapas {#next-steps}

Essa configuração concede à Adobe acesso somente leitura ao seu bucket do S3 e estabelece uma conexão confiável com a função IAM da Adobe.

Em seguida, prossiga para [Configurar o AWS S3 para fornecimento de público-alvo](./configure-aws-s3-audience-sourcing.md) para conectar seu bucket do S3 à Collaboration.

Para obter mais informações sobre públicos-alvo de origem, consulte [Source e gerenciar públicos-alvo](./onboard-audiences.md).
