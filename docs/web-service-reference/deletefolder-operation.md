---
title: Operação DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: A operação DeleteFolder exclui pastas de uma caixa de correio.
ms.openlocfilehash: fdd8519adbf9e0112f5fdd6a411dd6e7710f7d37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545430"
---
# <a name="deletefolder-operation"></a>Operação DeleteFolder

A **operação DeleteFolder** exclui pastas de uma caixa de correio. 
  
## <a name="deletefolder-request-example"></a>Exemplo de solicitação DeleteFolder

### <a name="description"></a>Descrição

Este exemplo a seguir de uma **solicitação DeleteFolder** mostra como formar uma solicitação para excluir uma pasta. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Este exemplo executa uma exclusão difícil na pasta.
  
> [!NOTE]
> A ID da pasta foi reduzida para preservar a capacidade de leitura. 
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [DeleteFolder](deletefolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada. 
  
Para encontrar outras opções para a mensagem de solicitação da **operação DeleteFolder,** explore a hierarquia de esquema. Comece no [elemento DeleteFolder.](deletefolder.md) 
  
## <a name="successful-deletefolder-response"></a>Resposta Bem-sucedida DeleteFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à **solicitação DeleteFolder.** 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Elementos de resposta

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
Para encontrar outras opções para a mensagem de resposta da **operação DeleteFolder,** explore a hierarquia de esquema. Comece no [elemento DeleteFolderResponse.](deletefolderresponse.md) 
  
## <a name="deletefolder-error-response"></a>Resposta de erro DeleteFolder

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma **solicitação DeleteFolder.** O erro foi causado por uma solicitação para excluir uma pasta que não estava presente na caixa de correio. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

A **operação DeleteFolder** não pode ser usada em pastas distintas. 
  
### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para encontrar outras opções para a mensagem de resposta de erro da **operação DeleteFolder,** explore a hierarquia de esquema. Comece no [elemento DeleteFolderResponse.](deletefolderresponse.md) 
  
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Excluir Pastas](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

