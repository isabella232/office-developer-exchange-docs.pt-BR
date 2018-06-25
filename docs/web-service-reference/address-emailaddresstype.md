---
title: Endereço (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: O elemento de endereço representa um endereço de email totalmente resolvido.
ms.openlocfilehash: 2a2d409edcc3a04bf82c6da0080183becfc9b25b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751133"
---
# <a name="address-emailaddresstype"></a>Endereço (EmailAddressType)

O elemento de **endereço** representa um endereço de email totalmente resolvido. 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddressType)](name-emailaddresstype.md) <br/> |Define o nome do usuário da caixa de correio. Esse elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento que é usado para a caixa de correio. O padrão é SMTP. Esse elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OriginalRecipients](originalrecipients.md) <br/> |Contém uma coleção de endereços de email que representam os destinatários originais de uma mensagem controlada.  <br/> |
|[RoomLists](roomlists.md) <br/> |Contém uma lista de salas em uma organização de reunião.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Contém uma lista de endereços de email que precisam foram enviadas em ordem para a condição ou exceção para aplicar a mensagens de entrada.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) 
- [Operação GetRoomLists](getroomlists-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

