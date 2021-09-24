---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: O elemento RoutingType define o tipo de endereço da caixa de correio.
ms.openlocfilehash: fdbe40bd74debe517739e0fe0c47ed108bd614c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509361"
---
# <a name="routingtype-emailaddresstype"></a>RoutingType (EmailAddressType)

O **elemento RoutingType** define o tipo de endereço da caixa de correio. 
  
```XML
<RoutingType/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifica quem o chamador está enviando como.  <br/> |
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um tipo de roteamento. SMTP é o valor de texto típico para esse elemento.
  
## <a name="remarks"></a>Comentários

Esse elemento é opcional no elemento [Mailbox.](mailbox.md) Outro [elemento RoutingType (EmailAddress)](routingtype-emailaddress.md) é usado para operações de disponibilidade. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

