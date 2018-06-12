---
title: Para
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
description: O elemento To Especifica o destino da transição fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837754"
---
# <a name="to"></a>Para

Elemento **To** Especifica o destino da transição fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário. 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Tipo  <br/> |Indica se o destino de transição do fuso horário é um período de fuso horário ou de um grupo de transições de fuso horário.  <br/> |
   
#### <a name="kind-attribute-values"></a>Valores de atributo Kind

|**Valor**|**Descrição**|
|:-----|:-----|
|Ponto  <br/> |Especifica que o destino de transição do fuso horário é um período de fuso horário.  <br/> |
|Group  <br/> |Especifica que a meta de transição do fuso horário é um grupo de transições de fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Representa uma transição de fuso horário que ocorre em uma data específica e, em um momento específico.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Representa uma transição de fuso horário que ocorre em um dia especificado do ano.  <br/> |
|[Transição](transition.md) <br/> |Representa uma transição de fuso horário.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é uma cadeia de caracteres que especifica o identificador exclusivo do [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário. 
  
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

