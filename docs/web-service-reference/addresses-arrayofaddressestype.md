---
title: Endereços (ArrayOfAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 711acc90-8e5b-4658-92d2-16cd441db56e
description: O elemento de endereços Especifica uma matriz de elementos de endereço.
ms.openlocfilehash: c1ee79611da1d19ce85202f9e3c0f68c421e98c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751071"
---
# <a name="addresses-arrayofaddressestype"></a>Endereços (ArrayOfAddressesType)

O elemento de **endereços** Especifica uma matriz de elementos de **endereço** . 
  
```XML
<Addresses>
    <Address></Address>
</Addresses>
```

 **ArrayOfAddressesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Endereço (ContactType)](address-contacttype.md) <br/> |Especifica o endereço de um contato.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Contato (ContactType)](contact-contacttype.md) <br/> |Especifica um contato no repositório unificado de contatos.  <br/> |
   
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

