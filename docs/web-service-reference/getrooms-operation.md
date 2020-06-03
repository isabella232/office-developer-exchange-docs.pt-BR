---
title: Operação getrooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 5501ddc0-3bfa-4da6-8e15-4223ca5499a3
description: A operação getrooms Obtém as salas dentro da lista de salas especificada.
ms.openlocfilehash: 4cb124b96637b9fcdca15595faebb2ce4d304de0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460544"
---
# <a name="getrooms-operation"></a>Operação getrooms

A operação **Getrooms** Obtém as salas dentro da lista de salas especificada. 
  
## <a name="soap-headers"></a>Cabeçalhos SOAP

A operação **Getrooms** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|Representação  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação.  <br/> |
   
## <a name="getrooms-request-example"></a>Exemplo de solicitação getrooms

### <a name="description"></a>Descrição

Veja a seguir um exemplo de uma solicitação **Getrooms** que obtém as salas que estão associadas a uma lista de salas. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>

```

### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [RequestServerVersion](requestserverversion.md)
    
- [Getrooms](getrooms.md)
    
- [RoomList](roomlist.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a>Exemplo de resposta de getrooms bem-sucedida

### <a name="description"></a>Descrição

A resposta a seguir mostra as informações de endereço de email para as salas que estão associadas à lista de salas.
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room02</t:Name>
            <t:EmailAddress>Room02@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="successful-getrooms-response-elements"></a>Elementos de resposta de getrooms bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetRoomsResponse](getroomsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Quartos](rooms.md)
    
- [Sala](room.md)
    
- [Nome (EmailAddress)](name-emailaddress.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddress)](routingtype-emailaddress.md)
    
- [MailboxType](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a>Exemplo de resposta de erro getrooms

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro causada por uma tentativa de obter informações de sala para uma lista de salas não existente.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a>Elementos de resposta de erro getrooms

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetRoomsResponse](getroomsresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

