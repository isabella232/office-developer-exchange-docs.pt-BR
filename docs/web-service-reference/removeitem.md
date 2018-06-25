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
description: O elemento RemoveItem representa um objeto de resposta que é usado para remover um item de reunião, quando uma mensagem MeetingCancellation é recebida.
ms.openlocfilehash: 6897363eba602e6a135ad255822197f9296dd44a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825108"
---
# <a name="removeitem"></a>RemoveItem

O elemento **RemoveItem** representa um objeto de resposta que é usado para remover um item de reunião, quando uma mensagem MeetingCancellation é recebida. 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ObjectName** <br/> |Representa o nome da classe de objeto de resposta RemoveItem como uma cadeia de caracteres de inglês.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |Identifica o item para o qual o objeto de resposta RemoveItem refere-se.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

 **RemoveItem** é válida apenas para um [MeetingCancellation](meetingcancellation.md). Caso contrário, será gerado um erro.
  
> [!NOTE]
> O [ItemClass](itemclass.md) para o cancelamento da reunião é IPM. Schedule.Meeting.Canceled. 
  
Para remover um [MeetingRequest](meetingrequest.md) e o associado [CalendarItem](calendaritem.md), use o objeto de resposta de [DeclineItem](declineitem.md) , em vez de **RemoveItem**.
  
 Não há suporte para **RemoveItem** para acesso de representante. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

