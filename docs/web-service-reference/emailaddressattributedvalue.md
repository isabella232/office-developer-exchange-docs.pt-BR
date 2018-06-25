---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: O elemento EmailAddressAttributedValue Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.
ms.openlocfilehash: 3bcbb5c0a2bc9a2dc24516b5fc62e6e3363a360b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752001"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

O elemento **EmailAddressAttributedValue** Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas. 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **EmailAddressAttributedValueType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Valor (EmailAddressType)](value-emailaddresstype.md) <br/> |Especifica que o valor de um **endereço de email** associado a uma matriz de atribuições.  <br/> |
|[Atribuições (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Especifica uma matriz de atribuições para seu elemento **valor** associado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |Especifica uma matriz de valores de email e os identificadores de suas atribuições de origem para a pessoa associada.  <br/> |
|[Emails2](emails2.md) <br/> |Especifica uma matriz de valores de email e os identificadores de suas atribuições de origem para a pessoa associada.  <br/> |
|[Emails3](emails3.md) <br/> |Especifica uma matriz de valores de email e os identificadores de suas atribuições de origem para a pessoa associada.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

