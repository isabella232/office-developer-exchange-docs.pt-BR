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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467687"
---
# <a name="removeitem"></a><span data-ttu-id="88539-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="88539-103">RemoveItem</span></span>

<span data-ttu-id="88539-104">O elemento **RemoveItem** representa um objeto Response que é usado para remover um item de reunião quando uma mensagem MeetingCancellation é recebida.</span><span class="sxs-lookup"><span data-stu-id="88539-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="88539-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="88539-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88539-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="88539-106">Attributes and elements</span></span>

<span data-ttu-id="88539-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="88539-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88539-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="88539-108">Attributes</span></span>

|<span data-ttu-id="88539-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="88539-109">**Attribute**</span></span>|<span data-ttu-id="88539-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88539-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88539-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="88539-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="88539-112">Representa o nome da classe do objeto de resposta RemoveItem como uma cadeia de caracteres em inglês.</span><span class="sxs-lookup"><span data-stu-id="88539-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="88539-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="88539-113">Child elements</span></span>

|<span data-ttu-id="88539-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88539-114">**Element**</span></span>|<span data-ttu-id="88539-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88539-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88539-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="88539-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="88539-117">Identifica o item ao qual o objeto de resposta RemoveItem se refere.</span><span class="sxs-lookup"><span data-stu-id="88539-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88539-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="88539-118">Parent elements</span></span>

|<span data-ttu-id="88539-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88539-119">**Element**</span></span>|<span data-ttu-id="88539-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88539-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88539-121">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="88539-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="88539-122">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="88539-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="88539-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="88539-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="88539-124">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88539-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88539-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="88539-125">Remarks</span></span>

 <span data-ttu-id="88539-126">**RemoveItem** é válido somente para um [MeetingCancellation](meetingcancellation.md).</span><span class="sxs-lookup"><span data-stu-id="88539-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="88539-127">Caso contrário, um erro será gerado.</span><span class="sxs-lookup"><span data-stu-id="88539-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="88539-128">O [pseudoclasse](itemclass.md) para um cancelamento de reunião é IPM. Schedule. Meeting. cancelada.</span><span class="sxs-lookup"><span data-stu-id="88539-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="88539-129">Para remover um [MeetingRequest](meetingrequest.md) e o [CalendarItem](calendaritem.md)associado, use o objeto de resposta [DeclineItem](declineitem.md) em vez de **RemoveItem**.</span><span class="sxs-lookup"><span data-stu-id="88539-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="88539-130">**RemoveItem** não tem suporte para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="88539-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="88539-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="88539-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88539-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="88539-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88539-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="88539-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88539-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="88539-134">Schema Name</span></span>  <br/> |<span data-ttu-id="88539-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="88539-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="88539-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="88539-136">Validation File</span></span>  <br/> |<span data-ttu-id="88539-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="88539-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88539-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="88539-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="88539-139">False</span><span class="sxs-lookup"><span data-stu-id="88539-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88539-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="88539-140">See also</span></span>



- [<span data-ttu-id="88539-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="88539-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

