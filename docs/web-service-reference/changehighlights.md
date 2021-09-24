---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: O elemento ChangeHighlights especifica o que mudou entre duas versões de uma mensagem de solicitação de reunião.
ms.openlocfilehash: 95f665f30c62d723cd97eaa2bd3eb3b2ed479967
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512209"
---
# <a name="changehighlights"></a>ChangeHighlights

O **elemento ChangeHighlights** especifica o que mudou entre duas versões de uma mensagem de solicitação de reunião. 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 **ChangeHighlightsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[HasLocationChanged](haslocationchanged.md) <br/> |Especifica se a propriedade de local de uma reunião foi alterada.  <br/> |
|[Location](location.md) <br/> |Representa o local de uma reunião ou compromisso.  <br/> |
|[HasStartTimeChanged](hasstarttimechanged.md) <br/> |Especifica se a hora de início de uma reunião foi alterada.  <br/> |
|[Start](start.md) <br/> |Representa o início de uma duração.  <br/> |
|[HasEndTimeChanged](hasendtimechanged.md) <br/> |Especifica se a hora de término de uma reunião foi alterada.  <br/> |
|[End ](end-ex15websvcsotherref.md) <br/> |Representa o fim de uma duração.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

