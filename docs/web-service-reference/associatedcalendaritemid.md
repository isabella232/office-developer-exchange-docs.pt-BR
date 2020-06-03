---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: O elemento AssociatedCalendarItemId representa o item de calendário que está associado a um MeetingMessage, MeetingRequest, MeetingResponse, MeetingCancellation ou ReminderMessageData.
ms.openlocfilehash: 816372c38243ba0fe5a7606c264dd1c5107350f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460880"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

O **elemento AssociatedCalendarItemId** representa o item de calendário que está associado a um [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md)ou [ReminderMessageData](remindermessagedata.md).
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **ItemIdtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica o item de calendário que está associado à reunião.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão específica do item de calendário que está associada a uma reunião.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>Comentários

As versões do Exchange que começam com o número de compilação 15.00.0913.09 podem incluir o elemento **AssociatedCalendarItemId** como um elemento filho do elemento **ReminderMessageData** . 
  
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

