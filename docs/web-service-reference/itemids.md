---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: O elemento ItemIds contém as identidades exclusivas de itens, itens de ocorrência e itens mestres recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460600"
---
# <a name="itemids"></a>ItemIds
  
O elemento **ItemIds** contém as identidades exclusivas de itens, itens de ocorrência e itens mestres recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange.
  
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
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifica uma única ocorrência de um item recorrente.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifica um item mestre de recorrência identificando um de seus identificadores de itens de ocorrência relacionados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversa (Conversatype)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Define uma solicitação para excluir itens no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |O elemento raiz que define uma solicitação para enviar itens no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Define uma solicitação para obter itens do repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover itens no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar itens no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/CopyItem` <br/> |
   
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

