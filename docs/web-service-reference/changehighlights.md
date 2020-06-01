---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: O elemento ChangeHighlights especifica o que foi alterado entre duas versões de uma mensagem de solicitação de reunião.
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463276"
---
# <a name="changehighlights"></a>ChangeHighlights

O elemento **ChangeHighlights** especifica o que foi alterado entre duas versões de uma mensagem de solicitação de reunião. 
  
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
|[HasLocationChanged](haslocationchanged.md) <br/> |Especifica se a propriedade Location de uma reunião foi alterada.  <br/> |
|[Localização](location.md) <br/> |Representa o local de uma reunião ou compromisso.  <br/> |
|[HasStartTimeChanged](hasstarttimechanged.md) <br/> |Especifica se a hora de início de uma reunião foi alterada.  <br/> |
|[Start](start.md) <br/> |Representa o início de uma duração.  <br/> |
|[HasEndTimeChanged](hasendtimechanged.md) <br/> |Especifica se a hora de término de uma reunião foi alterada.  <br/> |
|[Ponto](end-ex15websvcsotherref.md) <br/> |Representa o final de uma duração.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Também consulte



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

