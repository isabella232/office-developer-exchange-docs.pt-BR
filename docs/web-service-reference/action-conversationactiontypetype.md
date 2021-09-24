---
title: Action (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: O elemento Action contém a ação a ser feita na conversa especificada pelo elemento ConversationId.
ms.openlocfilehash: e75d9d5df75894d1de9831b0022269e7ace4fa63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514890"
---
# <a name="action-conversationactiontypetype"></a>Action (ConversationActionTypeType)

O **elemento Action** contém a ação a ser feita na conversa especificada pelo elemento [ConversationId.](conversationid.md) 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Action (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contém uma única ação a ser aplicada a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento Action** indica qual ação será executada em uma conversa. Veja a seguir os valores de texto possíveis e as ações correspondentes: 
  
- **AlwaysCategorize** - Os itens atuais e novos itens na conversa serão definidos automaticamente com as categorias identificadas no [elemento Categories.](categories-ex15websvcsotherref.md) 
    
- **AlwaysDelete** - Os itens atuais e novos itens na conversa serão excluídos automaticamente. O modo de exclusão é definido pelo [elemento DeleteType.](deletetype.md) 
    
- **AlwaysMove** - Os itens atuais e novos itens na conversa serão movidos automaticamente para a pasta identificada pelo [elemento DestinationFolderId.](destinationfolderid.md) 
    
- **Excluir** - Os itens atuais na conversa serão excluídos. Os itens subsequentes na conversa não serão excluídos. O modo de exclusão é definido pelo [elemento DeleteType.](deletetype.md) 
    
- **Mover** - Os itens atuais da conversa serão movidos para a pasta identificada pelo [elemento DestinationFolderId.](destinationfolderid.md) Os itens subsequentes na conversa não serão movidos. 
    
- **Copiar** - Os itens atuais da conversa serão copiados para a pasta identificada pelo [elemento DestinationFolderId.](destinationfolderid.md) Os itens subsequentes na conversa não serão copiados. 
    
- **SetReadState** - Os itens atuais da conversa terão seu estado de leitura definido. O estado de leitura é definido pelo [elemento IsRead.](isread.md) 
    
- **Sinalizador** - Os itens atuais da conversa terão um sinalizador definido como definido pelo [elemento Flag.](flag.md) 
    
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ApplyConversationAction](applyconversationaction-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

