---
title: Conversa (Conversatype)
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
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458933"
---
# <a name="conversation-conversationtype"></a>Conversa (Conversatype)

O elemento **Conversation** representa uma única conversa. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversas](conversations-ex15websvcsotherref.md)
  
[Conversa (Conversatype)](conversation-conversationtype.md)
  
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

 **Conversation**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |Representa o identificador de uma conversa.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Representa o tópico da conversa. Este elemento é somente leitura.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contém a lista de destinatários de uma conversa agregada a partir de uma pasta específica. Este elemento é somente leitura.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contém a lista de destinatários de uma conversa agregada em uma caixa de correio. Este elemento é somente leitura.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa na pasta atual. Este elemento é somente leitura.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contém uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa em todas as pastas da caixa de correio.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contém uma lista de todos os remetentes dos itens de conversa na pasta atual. Este elemento é somente leitura.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contém uma lista de todos os remetentes de itens de conversa na caixa de correio.  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |Contém o tempo de entrega da mensagem que foi recebida pela última vez nesta conversa na pasta atual.  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |Contém o tempo de entrega da mensagem que foi recebida pela última vez nesta conversa em todas as pastas da caixa de correio.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam as categorias que são aplicadas a todos os itens de conversa na pasta atual.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contém a lista de categorias de todos os itens de conversa em uma caixa de correio.  <br/> |
|[FlagStatus](flagstatus.md) <br/> |Contém o status de sinalizador agregado para itens de conversa na pasta atual.  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |Contém o status de sinalizador agregado para todos os itens de conversa em uma caixa de correio.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Contém um valor que indica se pelo menos um item de conversa na pasta atual tem um anexo.  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |Contém um valor que indica se pelo menos um item de conversa em uma caixa de correio tem um anexo.  <br/> |
|[MessageCount](messagecount.md) <br/> |Contém o número total de itens de conversa na pasta atual.  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |Contém o número total de itens de conversa na caixa de correio.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Contém a contagem de itens de conversa não lidos em uma pasta.  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |Contém uma contagem de todos os itens de conversa não lidos na caixa de correio.  <br/> |
|[Tamanho](size.md) <br/> |Contém o tamanho da conversa calculado a partir do tamanho de todos os itens de conversa na pasta atual.  <br/> |
|[GlobalSize](globalsize.md) <br/> |Contém o tamanho da conversa calculada a partir do tamanho de todos os itens de conversa da caixa de correio.  <br/> |
|[Doclasss (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |Contém uma lista de classes de item que representa todas as classes de item dos itens de conversa na pasta atual.  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |Contém uma lista de classes de item que representa todas as classes de item dos itens de conversa em uma caixa de correio.  <br/> |
|[Importance](importance.md) <br/> |Contém a importância agregada para todos os itens de conversa na pasta atual.  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |Contém a importância agregada para todos os itens de conversa em uma caixa de correio.  <br/> |
|[ItemIds](itemids.md) <br/> |Contém a coleção de identificadores de item para todos os itens de conversa na pasta atual.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversas](conversations-ex15websvcsotherref.md) <br/> |Contém uma matriz de conversas que são retornadas na resposta **FindConversation** .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)
  
[Operação ApplyConversationAction](applyconversationaction-operation.md)


[Conversas no EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

