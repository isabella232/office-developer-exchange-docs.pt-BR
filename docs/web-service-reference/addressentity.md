---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: O elemento AddressEntity especifica uma única entidade de endereço.
ms.openlocfilehash: c597557fe02a9c0ff7ed3c9862e1662cfbae596a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466903"
---
# <a name="addressentity"></a>AddressEntity

O elemento **AddressEntity** especifica uma única entidade de endereço. 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 **AddressEntityType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Endereço (cadeia de caracteres)](address-string.md) <br/> |Especifica um endereço.  <br/> |
|[Posição](position.md) <br/> |Especifica a posição em uma mensagem de email.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Endereços (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |Especifica uma matriz de elementos **AddressEntity** .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
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

