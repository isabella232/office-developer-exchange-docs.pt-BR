---
title: Atribuições (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: O elemento de atribuições especifica uma matriz de atribuições para o elemento de valor associado.
ms.openlocfilehash: 9fd552670c529009838125063869f65e130c1e63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463990"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Atribuições (ArrayOfValueAttributionsType)

O elemento de **atribuições** especifica uma matriz de atribuições para o elemento de **valor** associado. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atribuição (cadeia de caracteres)](attribution-string.md) <br/> |Especifica uma cadeia de caracteres usada para identificar um atributo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |Especifica o conteúdo do corpo de um item.  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |Especifica propriedades estendidas para uma pessoa.  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Especifica uma instância de uma matriz de números de telefone e suas atribuições associadas.  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |Especifica uma instância de uma matriz de endereços postais e suas atribuições associadas.  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Especifica uma instância de uma matriz de dados de cadeia de caracteres para um elemento persona.  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Especifica uma instância em uma matriz de atributos associados a um elemento persona.  <br/> |
   
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

