---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: O elemento DeliveryRestricted indica se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário.
ms.openlocfilehash: 58fc85873326179d7745db4ba7d4854a76ced6a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462686"
---
# <a name="deliveryrestricted"></a>DeliveryRestricted

O elemento **DeliveryRestricted** indica se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário. 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Dicas de Email](mailtips.md) <br/> |Representa valores de vários tipos de dicas de email.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto desse elemento será **true** se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário. O valor é **false** se as restrições de entrega não impedem que a mensagem do remetente atinja o destinatário. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

