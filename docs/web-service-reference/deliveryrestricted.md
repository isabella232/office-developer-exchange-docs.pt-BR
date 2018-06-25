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
description: O elemento DeliveryRestricted indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751776"
---
# <a name="deliveryrestricted"></a>DeliveryRestricted

O elemento **DeliveryRestricted** indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário. 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Dicas de email](mailtips.md) <br/> |Representa os valores para os vários tipos de dicas de email.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto deste elemento é **true** se as restrições de entrega impedirá que a mensagem do remetente está atingindo o destinatário. O valor é **false** se restrições de entrega não impede que a mensagem do remetente está atingindo o destinatário. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

