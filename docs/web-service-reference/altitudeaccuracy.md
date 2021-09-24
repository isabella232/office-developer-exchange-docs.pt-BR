---
title: AltitudeAccuracy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: aadc1f90-e9ab-4411-b51f-2d43e5e22f2a
description: O elemento AltitudeAccuracy especifica a precisão da propriedade altitude para um endereço postal.
ms.openlocfilehash: 75b56b0623de9c1a0945d9a569602e9863997498
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531273"
---
# <a name="altitudeaccuracy"></a>AltitudeAccuracy

O **elemento AltitudeAccuracy** especifica a precisão da propriedade altitude para um endereço postal. 
  
```XML
<AltitudeAccuracy></AltitudeAccuracy>
```

 **xs:double**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |Especifica o endereço postal do local.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento AltitudeAccuracy** é a estimativa de precisão para a propriedade de altitude de um endereço postal. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

