---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: O elemento Conversation contém o identificador de um item ou uma conversa.
ms.openlocfilehash: 4f12d70ae6b72773760a731f5778cf6743ce699f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461468"
---
# <a name="conversationid"></a>ConversationId

O elemento **Conversation** contém o identificador de um item ou uma conversa. 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 **ItemIdtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica um item específico no repositório do Exchange.  <br/> |
|**ChangeKey** <br/> | Identifica uma versão específica de um item. Um **ChangeKey** é necessário para os seguintes cenários:  <br/><br/>– O elemento [UpdateItem](updateitem.md) requer um **ChangeKey** se o atributo **ConflictResolution** estiver definido como autoresolver. Autoresolver é um valor padrão. Se o atributo **ChangeKey** não for incluído, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorChangeKeyRequired**.<br/><br/>- Os elementos [SendItem](senditem.md), [DeleteItem](deleteitem.md)e [DeleteFolder](deletefolder.md) exigem um **ChangeKey** para testar se a operação tentada funcionará na versão mais recente de um item. Se o atributo **ChangeKey** não estiver incluído no **ItemId** ou se o **ChangeKey** estiver vazio, a resposta retornará um valor de [ResponseCode](responsecode.md) igual a **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[Conversation](conversationaction.md) <br/> |Representa uma única ação a ser aplicada a uma única conversa.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item no repositório do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item de postagem no repositório do Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do repositório do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[Conversa (Conversatype)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
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

- [Operação FindConversation](findconversation-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

