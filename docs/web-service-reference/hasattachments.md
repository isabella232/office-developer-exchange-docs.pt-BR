---
title: HasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- HasAttachments
api_type:
- schema
ms.assetid: 538b7a85-11d7-4daa-8458-09b540760e8b
description: O elemento HasAttachments representa uma propriedade definida como true se um item tiver pelo menos um anexo visível ou se uma conversa contiver pelo menos um item que tenha um anexo. Essa propriedade é somente leitura.
ms.openlocfilehash: dea1ffdc5ae29a0bc7c585e0ebee9ed104143c53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547285"
---
# <a name="hasattachments"></a>HasAttachments

O **elemento HasAttachments** representa uma propriedade definida como **true** se um item tiver pelo menos um anexo visível ou se uma conversa contiver pelo menos um item que tenha um anexo. Essa propriedade é somente leitura. 
  
```XML
<HasAttachments/>
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
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Condições](conditions.md) <br/> |Representa as condições que, quando cumpridas, dispararão as ações de regra para essa regra.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para a regra caixa de entrada.  <br/> |
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor Boolean é necessário. Um valor verdadeiro **significa** que o item ou conversa tem pelo menos um anexo visível. Um valor false **significa** que o item ou conversa não tem anexos ou tem apenas anexos ocultos. 
  
## <a name="remarks"></a>Comentários

A **propriedade HasAttachments** é calculada a partir da propriedade **Boolean AllAttachmentsHidden** MAPI. Se um item não tiver um anexo, a **propriedade AllAttachmentsHidden** não existirá. Se todos os anexos no item estão ocultos, a **propriedade AllAttachmentsHidden** será **true**. A **propriedade AllAttachmentsHidden** é **false** se tiver pelo menos um anexo e pelo menos um dos anexos estiver visível. Use a **propriedade MAPI AllAttachmentsHidden** para pesquisar, agrupar e classificar itens. 
  
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
  
[Referência do EWS para Exchange](ews-reference-for-exchange.md)

