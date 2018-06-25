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
description: O elemento AssociatedCalendarItemId representa o item de calendário que está associado um MeetingMessage, MeetingRequest, MeetingResponse, MeetingCancellation ou ReminderMessageData.
ms.openlocfilehash: 4445da88d6fec42c1e02cd8de4d2e423485a4472
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751216"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

O elemento **AssociatedCalendarItemId** representa o item de calendário que está associado um [MeetingMessage](meetingmessage.md), [MeetingRequest](meetingrequest.md), [MeetingResponse](meetingresponse.md), [MeetingCancellation](meetingcancellation.md)ou [ReminderMessageData](remindermessagedata.md).
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Identifica o item de calendário que está associado à reunião.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão específica do item de calendário que está associado uma reunião.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>Comentários

Versões do Exchange, começando com o número de compilação 15.00.0913.09 podem incluir o elemento **AssociatedCalendarItemId** como um elemento filho do elemento **ReminderMessageData** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

