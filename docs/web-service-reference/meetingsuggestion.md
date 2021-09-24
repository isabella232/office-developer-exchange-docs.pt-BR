---
title: MeetingSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d6012063-eb67-4e83-a4a6-33482685083f
description: O elemento MeetingSuggestion especifica uma reunião proposta.
ms.openlocfilehash: 20523a77fc9fcdf22c837f2e4101ed699e1d4a7b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532486"
---
# <a name="meetingsuggestion"></a>MeetingSuggestion

O **elemento MeetingSuggestion** especifica uma reunião proposta. 
  
```XML
<MeetingSuggestion>
   <Attendees/>
   <Location/>
   <Subject/>
   <MeetingString/>
   <StartTime/>
   <EndTime/>
</MeetingSuggestion>
```

 **MeetingSuggestionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Participantes](attendees.md)  |  [Local](location.md)  |  [Assunto](subject.md)  |  [MeetingString](meetingstring.md)  |  [StartTime](starttime.md)  |  [EndTime](endtime.md)
  
### <a name="parent-elements"></a>Elementos pai

[MeetingSuggestions](meetingsuggestions.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

