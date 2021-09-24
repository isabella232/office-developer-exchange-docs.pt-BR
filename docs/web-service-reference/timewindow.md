---
title: TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: O elemento TimeWindow identifica o período de tempo consultado para as informações de disponibilidade do usuário.
ms.openlocfilehash: 93a486a5bc2306cfa61b74de82d795a711dbbceb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531341"
---
# <a name="timewindow"></a>TimeWindow

O **elemento TimeWindow** identifica o período de tempo consultado para as informações de disponibilidade do usuário. 
  
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
|[StartTime](starttime.md) <br/> |Representa o início de um intervalo de tempo consultado para as informações de disponibilidade do usuário.  <br/> |
|[EndTime](endtime.md) <br/> |Representa o fim de um intervalo de tempo consultado para as informações de disponibilidade do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Especifica o tipo de informação de ocupado/livre retornada na resposta.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>Comentários

O valor máximo para esse período é de 42 dias. Esse valor máximo pode ser modificado. Qualquer solicitação de informações de disponibilidade do usuário além do valor máximo retornará um erro. Se algum compromisso estiver parcialmente no intervalo de tempo definido pelos elementos [StartTime](starttime.md) e [EndTime,](endtime.md) esse compromisso será incluído em sua totalidade. 
  
> [!NOTE]
> O esquema que descreve esse elemento está localizado no diretório /EWS/do computador que está executando o Microsoft® Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

