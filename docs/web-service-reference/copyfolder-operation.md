---
title: Operação CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: A operação CopyFolder copia pastas em uma caixa de correio.
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751545"
---
# <a name="copyfolder-operation"></a>Operação CopyFolder

A operação CopyFolder copia pastas em uma caixa de correio.
  
## <a name="using-the-copyfolder-operation"></a>Usando a operação CopyFolder

A operação CopyFolder é semelhante à [operação MoveFolder](movefolder-operation.md). Ele copia pastas identificadas e retorna a **Id** e a **ChangeKey** das pastas copiadas. 
  
## <a name="copyfolder-request-example"></a>Exemplo de solicitação CopyFolder

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de CopyFolder mostra como copie as pastas na pasta caixa de entrada.
  
> [!NOTE]
> O valor do atributo **Id** do elemento [FolderId](folderid.md) foi reduzido para melhorar a legibilidade. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Pastas podem ser identificadas por elemento [DistinguishedFolderId](distinguishedfolderid.md) ou o elemento [FolderId](folderid.md) para uso em tanto o [ToFolderId](tofolderid.md) ou os elementos de [FolderIds](folderids.md) . 
  
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [CopyFolder](copyfolder.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
Para localizar outras opções para a mensagem de solicitação da operação CopyFolder, explore a hierarquia de esquema. Inicie o elemento [CopyFolder](copyfolder.md) . 
  
## <a name="successful-copyfolder-response"></a>Resposta de CopyFolder bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CopyFolder. 
  
> [!NOTE]
> A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Comment

O elemento [FolderId](folderid.md) retornado na resposta representa a pasta que foi copiada no novo local de pasta. 
  
### <a name="response-elements"></a>Elementos de resposta

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Para localizar outras opções para a mensagem de resposta da operação CopyFolder, explore a hierarquia de esquema. Inicie o elemento [CopyFolderResponse](copyfolderresponse.md) . 
  
## <a name="copyfolder-error-response"></a>Resposta de erro CopyFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação de CopyFolder. O erro ocorreu porque já existe uma pasta com o mesmo nome de exibição.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Pastas](folders-ex15websvcsotherref.md)
    
Para localizar outras opções para a mensagem de resposta de erro da operação CopyFolder, explore a hierarquia de esquema. Inicie o elemento [CopyFolderResponse](copyfolderresponse.md) . 
  
## <a name="see-also"></a>Confira também

- [Operação MoveFolder](movefolder-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

