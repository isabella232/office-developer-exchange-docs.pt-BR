---
title: Operação CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: A operação CreateManagedFolder cria uma pasta gerenciada no repositório do Exchange.
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44444590"
---
# <a name="createmanagedfolder-operation"></a>Operação CreateManagedFolder

A operação CreateManagedFolder cria uma pasta gerenciada no repositório do Exchange.
  
## <a name="using-the-createmanagedfolder-operation"></a>Usando a operação CreateManagedFolder

A operação CreateManagedFolder adiciona uma pasta personalizada gerenciada à caixa de correio de um usuário. Você pode usar o cmdlet **Get-ManagedFolder** do Shell de gerenciamento do Exchange para localizar pastas gerenciadas disponíveis para adicionar. Embora este cmdlet retorne pastas personalizadas gerenciadas e pastas padrão gerenciadas, somente pastas personalizadas gerenciadas podem ser adicionadas. Pastas personalizadas gerenciadas são identificadas pelo tipo de pasta ManagedCustomFolder. O namespace System. DirectoryServices também inclui tipos que podem ser usados para descobrir os nomes das pastas gerenciadas disponíveis. 
  
> [!NOTE]
> Você não pode usar os serviços Web do Exchange para localizar os nomes das pastas gerenciadas disponíveis para adicionar a uma caixa de correio. 
  
Você pode usar as operações FindFolder e GetFolder para acessar pastas gerenciadas. FindFolder é usado para pesquisar pastas em uma pasta pai especificada. Isso pode ser usado para que pastas gerenciadas possam ser descobertas em uma pasta antes de tentar adicionar uma pasta personalizada gerenciada duplicada no mesmo diretório. GetFolder é usado após a operação FindFolder para obter mais informações sobre uma pasta personalizada gerenciada.
  
## <a name="remarks"></a>Comentários

Para obter informações sobre como configurar a política de gerenciamento de registros de mensagens (MRM), consulte [como criar uma política de caixa de correio de pasta gerenciada](https://go.microsoft.com/fwlink/?LinkId=100975).
  
Para obter informações sobre como remover pastas personalizadas gerenciadas de uma caixa de correio, consulte [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Exemplo de solicitação CreateManagedFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação CreateManagedFolder mostra como adicionar uma pasta gerenciada chamada testar pasta gerenciada a uma caixa de correio.
  
> [!NOTE]
> Você também pode usar o acesso de representante para adicionar pastas personalizadas gerenciadas. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [FolderNames](foldernames.md)
    
- [FolderName](foldername.md)
    
Para encontrar outras opções para a mensagem de solicitação da operação CreateManagedFolder, explore a hierarquia de esquema. Inicie no elemento [CreateManagedFolder](createmanagedfolder.md) . 
  
## <a name="successful-createmanagedfolder-response"></a>Resposta CreateManagedFolder bem-sucedida

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra uma resposta bem-sucedida a uma solicitação CreateManagedFolder.
  
> [!NOTE]
> Os valores de atributo **ID** e **ChangeKey** foram reduzidos para preservar a legibilidade. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta: 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Para encontrar outras opções para as mensagens de resposta da operação CreateManagedFolder, explore a hierarquia de esquema. Inicie no elemento [CreateManagedFolderResponse](createmanagedfolderresponse.md) . 
  
## <a name="createmanagedfolder-error-response"></a>Resposta de erro CreateManagedFolder

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra uma resposta de erro a uma solicitação CreateManagedFolder.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>Confira também



[Operação GetFolder](getfolder-operation.md)
  
[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

