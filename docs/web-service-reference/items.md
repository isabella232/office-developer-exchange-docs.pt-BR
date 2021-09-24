---
title: Itens
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: O elemento Items contém uma matriz de itens.
ms.openlocfilehash: b6e9db6524640098a902f431393fccd6bd4e8868
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540880"
---
# <a name="items"></a>Itens

O **elemento Items** contém uma matriz de itens. 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 **ArrayOfRealItemsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Item](item.md) <br/> |Representa um item no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma mensagem de reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação CopyItem.](copyitem-operation.md)  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateItem.](createitem-operation.md)  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação GetItem.](getitem-operation.md)  <br/> |
|[GroupedItems](groupeditems.md) <br/> |Representa uma coleção de itens que são o resultado de uma chamada de operação [FindItem](finditem-operation.md) agrupada.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação MoveItem.](moveitem-operation.md)  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindItem](finditem-operation.md).  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação UpdateItem.](updateitem-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

Para obter informações sobre o conjunto de itens em uma solicitação de operação [CreateItem,](createitem-operation.md) consulte [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).
  
[Os](message-ex15websvcsotherref.md) elementos de mensagem representam mensagens de email e todos os outros itens que não são fortemente digitados pelo esquema Exchange Web Services (EWS). Itens como IPM. O compartilhamento e o IPM.InfoPath são retornados como **elementos message.** As versões Exchange a partir Exchange Server 2010 não retornam o elemento [Item](item.md) base em respostas. 
  
O esquema que descreve esse elemento está localizado no diretório virtual EWS do computador que está executando Exchange que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Referência do EWS para Exchange](ews-reference-for-exchange.md)
  
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

