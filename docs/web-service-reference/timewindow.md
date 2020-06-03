---
title: TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: O elemento TimeWindow identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.
ms.openlocfilehash: 5c66614520f9d616687d67ad609b3d55d9cf6571
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458926"
---
# <a name="timewindow"></a>TimeWindow

O elemento **TimeWindow** identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[TimeWindow](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 **Duration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Representa o início de um período de tempo consultado para as informações de disponibilidade do usuário.  <br/> |
|[EndTime](endtime.md) <br/> |Representa o final de um período de tempo consultado para as informações de disponibilidade do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Especifica o tipo de informações de disponibilidade retornadas na resposta.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>Comentários

O valor máximo para esse período de tempo é de 42 dias. Esse valor máximo pode ser modificado. Todas as solicitações de informações de disponibilidade do usuário além do valor máximo retornará um erro. Se algum compromisso estiver parcialmente no intervalo de tempo definido pelos elementos [StartTime](starttime.md) e [EndTime](endtime.md) , esse compromisso será incluído em sua totalidade. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o Microsoft® Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

