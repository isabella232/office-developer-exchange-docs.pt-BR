---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: O elemento AbsoluteDateTransition representa uma transição de fuso horário que ocorre em uma data específica e em um horário específico.
ms.openlocfilehash: c0d4e28d8ecefaaa72ded50ab3022666d74ce479
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542544"
---
# <a name="absolutedatetransition"></a>AbsoluteDateTransition

O **elemento AbsoluteDateTransition** representa uma transição de fuso horário que ocorre em uma data específica e em um horário específico. 
  
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
|[To](to.md) <br/> |Especifica o [Period ou](period.md) [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.  <br/> |
|[DateTime](datetime.md) <br/> |Representa a data e a hora em que ocorre a transição do fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Representa uma coleção de transições de fuso horário.  <br/> |
   
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

