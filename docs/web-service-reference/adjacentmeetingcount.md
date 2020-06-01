---
title: AdjacentMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetingCount
api_type:
- schema
ms.assetid: 35045024-f6e1-47d1-89be-f100b7b4f3c7
description: O elemento AdjacentMeetingCount representa o número total de itens de calendário adjacentes a um horário de reunião.
ms.openlocfilehash: 145010b345c3f9792a37c0662b87649b7f20a618
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463591"
---
# <a name="adjacentmeetingcount"></a>AdjacentMeetingCount

O elemento **AdjacentMeetingCount** representa o número total de itens de calendário adjacentes a um horário de reunião. 
  
```xml
<AdjacentMeetingCount/>
```

 **Int**
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
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um inteiro é necessário.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

