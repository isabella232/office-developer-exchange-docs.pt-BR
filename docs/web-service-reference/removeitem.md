---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: O elemento RemoveItem representa um objeto Response que é usado para remover um item de reunião quando uma mensagem MeetingCancellation é recebida.
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467687"
---
# <a name="removeitem"></a>RemoveItem

O elemento **RemoveItem** representa um objeto Response que é usado para remover um item de reunião quando uma mensagem MeetingCancellation é recebida. 
  
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
|**ObjectName** <br/> |Representa o nome da classe do objeto de resposta RemoveItem como uma cadeia de caracteres em inglês.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |Identifica o item ao qual o objeto de resposta RemoveItem se refere.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

 **RemoveItem** é válido somente para um [MeetingCancellation](meetingcancellation.md). Caso contrário, um erro será gerado.
  
> [!NOTE]
> O [pseudoclasse](itemclass.md) para um cancelamento de reunião é IPM. Schedule. Meeting. cancelada. 
  
Para remover um [MeetingRequest](meetingrequest.md) e o [CalendarItem](calendaritem.md)associado, use o objeto de resposta [DeclineItem](declineitem.md) em vez de **RemoveItem**.
  
 **RemoveItem** não tem suporte para acesso de representante. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

