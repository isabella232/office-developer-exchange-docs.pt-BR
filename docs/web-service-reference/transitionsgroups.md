---
title: TransitionsGroups
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: O elemento TransitionsGroups representa uma matriz de grupos de transição de fuso horário.
ms.openlocfilehash: cd394d0ec333f639542c44cef6c992b24b69f65c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515115"
---
# <a name="transitionsgroups"></a>TransitionsGroups

O **elemento TransitionsGroups** representa uma matriz de grupos de transição de fuso horário. 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 **ArrayOfTransitionsGroupsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma matriz de transições de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |Define o fuso horário para a hora de início de [um CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Define o fuso horário para a hora de término de [um CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Define um fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

