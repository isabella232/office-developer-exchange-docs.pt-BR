---
title: Operação GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Encontre informações sobre a operação GetUserPhoto EWS.
ms.openlocfilehash: 6dd1ce73d6291e60ce188b98b917a4c79ce792b5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547481"
---
# <a name="getuserphoto-operation"></a>Operação GetUserPhoto

Encontre informações sobre a **operação GetUserPhoto** EWS. 
  
A **operação GetUserPhoto** obtém uma foto do usuário dos Serviços de Domínio do Active Directory (AD DS). 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>Usando a operação GetUserPhoto

A **operação RemoveContactFromImList** é uma operação simples que aceita o endereço de email de um usuário e o tamanho da foto solicitada e retorna o fluxo de fotos na resposta. 
  
> [!NOTE]
> O EWS tem um SOAP e uma operação baseada em REST para obter fotos do usuário. Para obter informações sobre a interface REST, consulte [Obter fotos do usuário usando o EWS em Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx). 
  
### <a name="getuserphoto-operation-soap-headers"></a>Headers SOAP da operação GetUserPhoto

A **operação GetUserPhoto** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Exemplo da solicitação de operação GetUserPhoto: Obter a foto de um usuário

O exemplo a seguir de uma **solicitação de operação GetUserPhoto** mostra como obter a foto de um usuário. Este exemplo solicita uma foto do usuário de 48 x 48 pixels. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

Os seguintes elementos são usados no corpo SOAP da solicitação:
  
- [GetUserPhoto](getuserphoto.md)
    
- [Email (String)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Resposta bem-sucedida da operação GetUserPhoto

O exemplo a seguir mostra uma resposta bem-sucedida a **uma operação GetUserPhoto** para obter a foto de um usuário. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

Os seguintes elementos são usados no corpo SOAP da resposta:
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Resposta de erro da operação GetUserPhoto

O envelope SOAP não retornará um código de erro se for feita uma tentativa de obter uma foto de usuário para um endereço de email que não existe na organização. Um código de status HTTP 500 será retornado na resposta para indicar que a solicitação não foi bem-sucedida. 
  
## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)   
- [Obter fotos do usuário usando o EWS no Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

