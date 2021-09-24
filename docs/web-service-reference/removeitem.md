---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: O elemento RemoveItem representa um objeto de resposta usado para remover um item de reunião quando uma mensagem MeetingCancellation é recebida.
ms.openlocfilehash: 4dbe9ede36bf6e3c008a2186cfe617519ecfae1f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517956"
---
# <a name="removeitem"></a>RemoveItem

O **elemento RemoveItem** representa um objeto de resposta usado para remover um item de reunião quando uma mensagem MeetingCancellation é recebida. 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ObjectName** <br/> |Representa o nome da classe de objeto de resposta RemoveItem como uma cadeia de caracteres em inglês.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |Identifica o item ao qual o objeto de resposta RemoveItem se refere.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a ser criado na pasta identificada pelo elemento [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta associados a um item no Exchange store.  <br/> |
   
## <a name="remarks"></a>Comentários

 **RemoveItem** só é válido para [um MeetingCancellation](meetingcancellation.md). Caso contrário, um erro é lançado.
  
> [!NOTE]
> A [ItemClass para](itemclass.md) um cancelamento de reunião é IPM. Schedule.Meeting.Canceled. 
  
Para remover um [MeetingRequest](meetingrequest.md) e [o CalendarItem](calendaritem.md)associado, use o objeto de resposta [DeclineItem](declineitem.md) em vez de **RemoveItem**.
  
 **RemoveItem não** tem suporte para acesso de representante. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

