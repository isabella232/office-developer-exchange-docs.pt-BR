---
title: LastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- LastDeliveryTime
api_type:
- schema
ms.assetid: 23d02ceb-f28e-40f2-8f63-673723a50e2a
description: O elemento LastDeliveryTime contém o tempo de entrega da mensagem recebida pela última vez nesta conversa na pasta atual.
ms.openlocfilehash: bb0ad41272d26efecf36113d9c82a647c237ac47
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546172"
---
# <a name="lastdeliverytime"></a>LastDeliveryTime

O **elemento LastDeliveryTime** contém o tempo de entrega da mensagem recebida pela última vez nesta conversa na pasta atual. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversas](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
[LastDeliveryTime](lastdeliverytime.md)
  
```XML
<LastDeliveryTime/>
```

 **xs:dateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento LastDeliveryTime** é a data e a hora da mensagem recebida pela última vez nesta conversa na pasta atual. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)
  
[Operação ApplyConversationAction](applyconversationaction-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Conversas no EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

