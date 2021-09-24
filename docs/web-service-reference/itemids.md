---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: O elemento ItemIds contém as identidades exclusivas de itens, itens de ocorrência e itens mestras recorrentes usados para excluir, enviar, obter, mover ou copiar itens no Exchange store.
ms.openlocfilehash: 7341b8214b4d61564bd87707a9d8c76fbca07628
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522884"
---
# <a name="itemids"></a>ItemIds
  
O **elemento ItemIds** contém as identidades exclusivas de itens, itens de ocorrência e itens mestras recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no Exchange store.
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**NonEmptyArrayOfBaseItemIdsType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai. 
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no Exchange store.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifica uma única ocorrência de um item recorrente.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifica um item mestre de recorrência identificando um dos identificadores de itens de ocorrência relacionados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Define uma solicitação para excluir itens no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |O elemento raiz que define uma solicitação para enviar itens no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Define uma solicitação para obter itens do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover itens no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar itens no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação DeleteItem](deleteitem-operation.md)
- [Operação SendItem](senditem-operation.md) 
- [Operação GetItem](getitem-operation.md)
- [Operação MoveItem](moveitem-operation.md)
- [Operação CopyItem](copyitem-operation.md)
- [Operação FindConversation](findconversation-operation.md)

