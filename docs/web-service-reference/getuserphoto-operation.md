---
title: Operação GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Encontre informações sobre o EWS GetUserPhoto operação.
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823694"
---
# <a name="getuserphoto-operation"></a>Operação GetUserPhoto

Encontre informações sobre a operação de EWS **GetUserPhoto** . 
  
A operação **GetUserPhoto** obtém uma foto do usuário dos serviços de domínio Active Directory (AD DS). 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>Usando a operação GetUserPhoto

A operação de **RemoveContactFromImList** é uma operação simple que aceita o endereço de email do usuário e o tamanho da foto solicitado e retorna o fluxo de foto na resposta. 
  
> [!NOTE]
> EWS tem um SOAP e uma operação baseado em REST para obter as fotos dos usuários. Para obter informações sobre a interface REST, consulte [obter fotos de usuário usando o EWS no Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx). 
  
### <a name="getuserphoto-operation-soap-headers"></a>Cabeçalhos SOAP GetUserPhoto operação

A operação **GetUserPhoto** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Exemplo de solicitação de operação GetUserPhoto: Obtenha a foto do usuário

O exemplo a seguir de uma solicitação de operação **GetUserPhoto** mostra como obter a foto do usuário. Este exemplo solicita uma foto do usuário 48x48 pixels. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Os seguintes elementos são usados na solicitação de corpo SOAP:
  
- [GetUserPhoto](getuserphoto.md)
    
- [Email (String)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Resposta de operação GetUserPhoto bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma operação **GetUserPhoto** para obter a foto do usuário. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

Os seguintes elementos são usados no corpo SOAP de resposta:
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Resposta de erro de operação GetUserPhoto

O envelope SOAP não retornará um código de erro, se for feita uma tentativa para obter uma foto do usuário para um endereço de email que não existe na organização. Um código de status HTTP 500 será retornado na resposta para indicar que a solicitação foi bem sucedida. 
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)   
- [Obtenha as fotos de usuários usando o EWS no Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

