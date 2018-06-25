---
title: Ação (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: O elemento Action contém a ação a ser executada a conversa especificada pelo elemento ConversationId.
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751033"
---
# <a name="action-conversationactiontypetype"></a>Ação (ConversationActionTypeType)

O elemento **Action** contém a ação a ser executada a conversa especificada pelo elemento [ConversationId](conversationid.md) . 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Ação (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contém uma única ação a ser aplicado a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento **Action** indica a ação que será executada em uma conversa. Estes são os valores de texto possíveis e as ações correspondentes: 
  
- **AlwaysCategorize** - os itens atuais e novos itens da conversa serão definidas automaticamente com as categorias identificadas no elemento [categorias](categories-ex15websvcsotherref.md) . 
    
- **AlwaysDelete** - os itens atuais e novos itens da conversa serão excluídas automaticamente. O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) . 
    
- **AlwaysMove** - os itens atuais e novos itens da conversa serão movidas automaticamente para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) . 
    
- **Excluir** - os itens da conversa atuais será excluído. Os itens na conversa subsequentes não serão excluídos. O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) . 
    
- **Mova** - os itens atuais na conversa serão movidas para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) . Os itens na conversa subsequentes não serão movidos. 
    
- **Copy** - os itens da conversa atuais serão copiadas para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) . Os itens na conversa subsequentes não serão copiados. 
    
- **SetReadState** - os itens da conversa atuais terá seu estado de leitura definido. O estado lido é definido pelo elemento [foi lido](isread.md) . 
    
- **Sinalizador** - os itens da conversa atuais terão um sinalizador definido como determinado pelo elemento [sinalizador](flag.md) . 
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ApplyConversationAction](applyconversationaction-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

