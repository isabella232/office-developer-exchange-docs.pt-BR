---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: O elemento ConversationId contém o identificador de um item ou conversa.
ms.openlocfilehash: 345c7c692576abb8c1e1b9848b005ca3d0c0fa0f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547537"
---
# <a name="conversationid"></a>ConversationId

O **elemento ConversationId** contém o identificador de um item ou conversa. 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica um item específico no Exchange store.  <br/> |
|**ChangeKey** <br/> | Identifica uma versão específica de um item. Uma **ChangeKey** é necessária para os seguintes cenários:  <br/><br/>- O [elemento UpdateItem](updateitem.md) requer **um ChangeKey** se o atributo **ConflictResolution** estiver definido como AutoResolve. AutoResolve é um valor padrão. Se o **atributo ChangeKey** não estiver incluído, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorChangeKeyRequired**.<br/><br/>- [Os elementos SendItem,](senditem.md) [DeleteItem](deleteitem.md)e [DeleteFolder](deletefolder.md) exigem um **ChangeKey** para testar se a tentativa de operação agirá na versão mais recente de um item. Se o atributo **ChangeKey** não estiver incluído no **ItemId** ou se **o ChangeKey** estiver vazio, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[ConversationAction](conversationaction.md) <br/> |Representa uma única ação a ser aplicada a uma única conversa.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindConversation](findconversation-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

