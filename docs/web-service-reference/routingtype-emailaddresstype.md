---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: O elemento de RoutingType define o tipo de endereço da caixa de correio.
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825256"
---
# <a name="routingtype-emailaddresstype"></a>RoutingType (EmailAddressType)

O elemento de **RoutingType** define o tipo de endereço da caixa de correio. 
  
```XML
<RoutingType/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifica que o chamador está enviando como.  <br/> |
|[Caixa de correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa um tipo de roteamento. SMTP é o valor de texto típica para esse elemento.
  
## <a name="remarks"></a>Coment�rios

Esse elemento é opcional no elemento de [caixa de correio](mailbox.md) . Outro elemento [RoutingType (EmailAddress)](routingtype-emailaddress.md) é usado para operações de disponibilidade. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

