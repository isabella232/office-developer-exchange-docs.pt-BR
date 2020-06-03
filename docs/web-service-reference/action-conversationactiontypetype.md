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
description: O elemento Action contém a ação a ser executada na conversa especificada pelo elemento CONVERSATION.
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527541"
---
# <a name="action-conversationactiontypetype"></a>Ação (ConversationActionTypeType)

O elemento **Action** contém a ação a ser executada na conversa especificada pelo elemento [Conversation](conversationid.md) . 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [Conversation](conversationaction.md)
  
- [Ação (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
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
|[Conversation](conversationaction.md) <br/> |Contém uma única ação a ser aplicada a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Action** indica qual ação será executada em uma conversa. Estes são os valores de texto possíveis e as ações correspondentes: 
  
- **AlwaysCategorize** -os itens atuais e novos itens na conversa serão automaticamente definidos com as categorias identificadas no elemento [Categories](categories-ex15websvcsotherref.md) . 
    
- **AlwaysDelete** -os itens atuais e novos itens na conversa serão excluídos automaticamente. O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) . 
    
- **AlwaysMove** -os itens atuais e os novos itens da conversa serão movidos automaticamente para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) . 
    
- **Excluir** -os itens atuais da conversa serão excluídos. Os itens subsequentes na conversa não serão excluídos. O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) . 
    
- **Move** -os itens atuais na conversa serão movidos para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) . Os itens subsequentes na conversa não serão movidos. 
    
- **Copy** – os itens atuais na conversa serão copiados para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) . Os itens subsequentes na conversa não serão copiados. 
    
- **Setreadstate** -os itens atuais na conversa terão o estado de leitura definido. O estado de leitura é definido pelo elemento [IsRead](isread.md) . 
    
- **Flag** -os itens atuais na conversa terão um sinalizador definido conforme definido pelo elemento [Flag](flag.md) . 
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ApplyConversationAction](applyconversationaction-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

