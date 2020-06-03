---
title: RecurrenceType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: O elemento RecurrenceType é usado para identificar uma instância específica de um item de calendário recorrente.
ms.openlocfilehash: 58a379f2cffa7ff37181e93ad1c45c9752e84f1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461608"
---
# <a name="recurrenceid"></a>RecurrenceType

O elemento **RecurrenceType** é usado para identificar uma instância específica de um item de calendário recorrente. 
  
```xml
<RecurrenceId/>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma mensagem de reunião.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um valor de data/hora que identifica uma ocorrência de calendário.
  
## <a name="remarks"></a>Comentários

Essa propriedade é usada com a propriedade [UID](uid.md) para identificar uma instância específica de um item de calendário recorrente. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

