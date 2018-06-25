---
title: Atribuições (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: O elemento de atribuições Especifica uma matriz de atribuições para seu elemento valor associado.
ms.openlocfilehash: a64510cacb9923682418ca8a9b203c765a129bdd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751239"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Atribuições (ArrayOfValueAttributionsType)

O elemento de **atribuições** Especifica uma matriz de atribuições para seu elemento **valor** associado. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atribuição (string)](attribution-string.md) <br/> |Especifica uma cadeia de caracteres usada para identificar um atributo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |Especifica o conteúdo do corpo de um item.  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |Especifica as propriedades estendidas para uma pessoa.  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Especifica uma instância de uma matriz de números de telefone e suas atribuições associadas.  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |Especifica uma instância de uma matriz de endereços postais e suas atribuições associadas.  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Especifica uma instância de uma matriz de dados de cadeia de caracteres de um elemento de pessoa.  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Especifica uma instância em uma matriz de atributos associados a um elemento de pessoa.  <br/> |
   
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

