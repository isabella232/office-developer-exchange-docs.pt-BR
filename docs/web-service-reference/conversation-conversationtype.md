---
title: Conversa (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: O elemento Conversation representa uma única conversa.
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751522"
---
# <a name="conversation-conversationtype"></a>Conversa (ConversationType)

O elemento **Conversation** representa uma única conversa. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversas](conversations-ex15websvcsotherref.md)
  
[Conversa (ConversationType)](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 **ConversationType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |Representa o identificador de uma conversa.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Representa o tópico de conversação. Este elemento é somente leitura.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contém a lista de destinatários de uma conversa agregada de uma determinada pasta. Este elemento é somente leitura.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contém a lista de destinatários de uma conversa agregada em uma caixa de correio. Este elemento é somente leitura.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa na pasta atual. Este elemento é somente leitura.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa entre todas as pastas na caixa de correio.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contém uma lista de todos os remetentes dos itens de conversa na pasta atual. Este elemento é somente leitura.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contém uma lista de todos os remetentes dos itens de conversa na caixa de correio.  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |Contém o tempo de entrega da mensagem foi recebida pela última nesta conversa na pasta atual.  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |Contém o tempo de entrega da mensagem foi recebida pela última nesta conversa entre todas as pastas na caixa de correio.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam as categorias que são aplicadas a todos os itens de conversa na pasta atual.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contém a lista de categorias para todos os itens de conversa em uma caixa de correio.  <br/> |
|[FlagStatus](flagstatus.md) <br/> |Contém o status do sinalizador agregados para itens de conversa na pasta atual.  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |Contém o status do sinalizador agregados de todos os itens de conversa em uma caixa de correio.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Contém um valor que indica se o item de pelo menos uma conversa na pasta atual tiver um anexo.  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |Contém um valor que indica se o item de pelo menos uma conversa em uma caixa de correio tem um anexo.  <br/> |
|[MessageCount](messagecount.md) <br/> |Contém o número total de itens de conversa na pasta atual.  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |Contém o número total de itens de conversa, na caixa de correio.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Contém a contagem de itens não lidos conversa dentro de uma pasta.  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |Contém uma contagem de todos os itens de conversa não lidas na caixa de correio.  <br/> |
|[Size](size.md) <br/> |Contém o tamanho de conversa calculado a partir do tamanho de todos os itens de conversa na pasta atual.  <br/> |
|[GlobalSize](globalsize.md) <br/> |Contém o tamanho da conversa calculado a partir do tamanho de todos os itens de conversa, na caixa de correio.  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |Contém uma lista das classes de item que representa todas as classes de item, os itens de conversa na pasta atual.  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |Contém uma lista das classes de item que representa todas as classes de item, os itens de conversa de uma caixa de correio.  <br/> |
|[Importância](importance.md) <br/> |Contém a importância agregada de todos os itens de conversa na pasta atual.  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |Contém a importância agregada de todos os itens de conversa em uma caixa de correio.  <br/> |
|[ItemIds](itemids.md) <br/> |Contém o conjunto de identificadores de item para todos os itens de conversa na pasta atual.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contém o conjunto de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversas](conversations-ex15websvcsotherref.md) <br/> |Contém uma matriz de conversas que são retornados na resposta **FindConversation** .  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindConversation](findconversation-operation.md)
  
[Operação ApplyConversationAction](applyconversationaction-operation.md)


[Conversas no EWS](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

