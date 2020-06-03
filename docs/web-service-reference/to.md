---
title: To
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: O elemento to especifica o destino da transição de fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário.
ms.openlocfilehash: 8cce700eedd64035f2e21be4db6b517f3f85d98d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44468793"
---
# <a name="to"></a>To

O elemento **to** especifica o destino da transição de fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário. 
  
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
|Período  <br/> |Especifica que o destino de transição de fuso horário é um período de fuso horário.  <br/> |
|Group  <br/> |Especifica que o destino de transição de fuso horário é um grupo de transições de fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Representa uma transição de fuso horário que ocorre em uma data específica e em uma hora específica.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Representa uma transição de fuso horário que ocorre em um dia do ano especificado.  <br/> |
|[Transição](transition.md) <br/> |Representa uma transição de fuso horário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é uma cadeia de caracteres que especifica o identificador exclusivo do [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

