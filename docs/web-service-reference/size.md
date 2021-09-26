---
title: Size
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Size
api_type:
- schema
ms.assetid: 966f4daf-c20e-49f8-aeb6-965f3e2da7c3
description: O elemento Size representa o tamanho em bytes de um item ou todos os itens em uma conversa na pasta atual. Essa propriedade é somente leitura.
ms.openlocfilehash: efa841732ca03b410e0a5979ff7e282cf2c7dde9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545920"
---
# <a name="size"></a>Size

O **elemento Size** representa o tamanho em bytes de um item ou todos os itens em uma conversa na pasta atual. Essa propriedade é somente leitura. 
  
```XML
<Size/>
```

 **int**
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
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo anexado a um item no Exchange store.  <br/> |
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um Exchange que está anexado a outro Exchange item.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é um valor inteiro que identifica o tamanho do item em bytes.
  
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



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

