---
title: Para
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: O elemento Para especifica o destino da transição do fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário.
ms.openlocfilehash: 64f3f3258fd7c2bad051eabb1b33617bb056ab39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522548"
---
# <a name="to"></a>Para

O **elemento Para** especifica o destino da transição do fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário. 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Tipo  <br/> |Indica se o destino de transição de fuso horário é um período de fuso horário ou de um grupo de transições de fuso horário.  <br/> |
   
#### <a name="kind-attribute-values"></a>Valores de atributo Kind

|**Valor**|**Descrição**|
|:-----|:-----|
|Period  <br/> |Especifica que o destino de transição do fuso horário é um período de fuso horário.  <br/> |
|Group  <br/> |Especifica que o destino de transição do fuso horário é um grupo de transições de fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Representa uma transição de fuso horário que ocorre em uma data específica e em um horário específico.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Representa uma transição de fuso horário que ocorre em um dia especificado do ano.  <br/> |
|[Transition](transition.md) <br/> |Representa uma transição de fuso horário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é uma cadeia de caracteres que especifica o identificador exclusivo do [Period](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição do fuso horário. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

