---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: O elemento AbsoluteDateTransition representa uma transição de fuso horário que ocorre em uma data específica e em uma hora específica.
ms.openlocfilehash: 514464f69c3be5496aedbe184848ef9ed9f296b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461720"
---
# <a name="absolutedatetransition"></a>AbsoluteDateTransition

O elemento **AbsoluteDateTransition** representa uma transição de fuso horário que ocorre em uma data específica e em uma hora específica. 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

**AbsoluteDateTransitionType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[To](to.md) <br/> |Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.  <br/> |
|[DateTime](datetime.md) <br/> |Representa a data e a hora em que ocorre a transição de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transições](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

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

