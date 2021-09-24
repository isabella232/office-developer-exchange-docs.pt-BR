---
title: IsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsRead
api_type:
- schema
ms.assetid: 161455d5-a870-4c99-b2eb-c759c538f1bc
description: O elemento IsRead indica se uma mensagem foi lida.
ms.openlocfilehash: cbd2fb90a413e1ec700cf07a11e0082a985545b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539392"
---
# <a name="isread"></a>IsRead

O **elemento IsRead** indica se uma mensagem foi lida. 
  
```XML
<IsRead/>
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
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[ConversationAction](conversationaction.md) <br/> |Contém uma única ação a ser aplicada a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que a mensagem foi lida. Um valor de texto **false** indica que a mensagem não foi lida. 
  
## <a name="remarks"></a>Comentários

Se [IsReadReceiptRequested](isreadreceiptrequested.md) for **true**, a configuração **de IsRead** como **true** envia um recibo de leitura. O destinatário pode suprimir recibos de leitura enviando o objeto de resposta [SuppressReadReceipt](suppressreadreceipt.md) antes de definir a **propriedade IsRead.** 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

