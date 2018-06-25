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
description: O elemento ItemIds contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824155"
---
# <a name="itemids"></a>ItemIds
  
O elemento **ItemIds** contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes de mestres que são usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange.
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

**NonEmptyArrayOfBaseItemIdsType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai. 
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.  <br/> |
|[OccurrenceItemId](occurrenceitemid.md) <br/> |Identifica uma única ocorrência de um item recorrente.  <br/> |
|[RecurringMasterItemId](recurringmasteritemid.md) <br/> |Identifica um item-mestre recorrência identificando um dos identificadores dos seus itens relacionados ocorrência.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversa (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[DeleteItem](deleteitem.md) <br/> |Define uma solicitação para excluir itens no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/DeleteItem` <br/> |
|[SendItem](senditem.md) <br/> |O elemento raiz que define uma solicitação para enviar itens no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/SendItem` <br/> |
|[GetItem](getitem.md) <br/> |Define uma solicitação para obter itens do armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetItem` <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover itens no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar os itens no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação DeleteItem](deleteitem-operation.md)
- [Operação SendItem](senditem-operation.md) 
- [Operação GetItem](getitem-operation.md)
- [Operação MoveItem](moveitem-operation.md)
- [Operação CopyItem](copyitem-operation.md)
- [Operação FindConversation](findconversation-operation.md)

