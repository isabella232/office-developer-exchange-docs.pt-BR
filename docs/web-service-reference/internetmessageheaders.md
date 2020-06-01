---
title: Propriedadeinternetmessageheaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: O elemento Propriedadeinternetmessageheaders contém uma coleção de alguns cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio. Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, Consulteobter Internet Message cabeçalhos no EWS, MIME e os cabeçalhos de mensagem da Internet ausentes.
ms.openlocfilehash: 4719050c02590e021b29173c234466de3fdc58a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467323"
---
# <a name="internetmessageheaders"></a>Propriedadeinternetmessageheaders

O elemento **propriedadeinternetmessageheaders** contém uma coleção de alguns cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio. Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** . Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, consulte "obtendo cabeçalhos de mensagens da Internet" em [EWS, MIME e cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 **NonEmptyArrayOfInternetHeadersType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InternetMessageHeader](internetmessageheader.md) <br/> |Representa o cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Representa uma resposta de aceitação para uma solicitação de reunião.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Representa uma resposta de recusa a uma solicitação de reunião.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item no repositório do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do repositório do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Representa uma resposta provisoriamente aceita a uma solicitação de reunião.  <br/> |
   
## <a name="remarks"></a>Comentários

A seguir está a definição da propriedade estendida da API gerenciada do EWS para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[EWS, MIME e os cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

