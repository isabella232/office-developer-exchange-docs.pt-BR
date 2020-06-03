---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: O elemento EmailAddressAttributedValue especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.
ms.openlocfilehash: 09fdd5921cef3d70a6da4b6d4d38f08834c5d482
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530688"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

O elemento **EmailAddressAttributedValue** especifica uma instância de uma matriz de endereços de email e suas atribuições associadas. 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **EmailAddressAttributedValueType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Valor (EmailAddresstype)](value-emailaddresstype.md) <br/> |Especifica o valor de um **EmailAddress** associado a uma matriz de atribuições.  <br/> |
|[Atribuições (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Especifica uma matriz de atribuições para o elemento de **valor** associado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |Especifica uma matriz de valores de email e os identificadores de suas atribuições de origem para o persona associado.  <br/> |
|[Emails2](emails2.md) <br/> |Especifica uma matriz de valores de email e os identificadores de suas atribuições de origem para o persona associado.  <br/> |
|[Emails3](emails3.md) <br/> |Especifica uma matriz de valores de email e os identificadores de suas atribuições de origem para o persona associado.  <br/> |
   
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
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

