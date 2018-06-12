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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825108"
---
# <a name="removeitem"></a><span data-ttu-id="9fcb2-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="9fcb2-103">RemoveItem</span></span>

<span data-ttu-id="9fcb2-104">O elemento **RemoveItem** representa um objeto de resposta que é usado para remover um item de reunião, quando uma mensagem MeetingCancellation é recebida.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="9fcb2-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fcb2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9fcb2-106">Attributes and elements</span></span>

<span data-ttu-id="9fcb2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fcb2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9fcb2-108">Attributes</span></span>

|<span data-ttu-id="9fcb2-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-109">**Attribute**</span></span>|<span data-ttu-id="9fcb2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9fcb2-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="9fcb2-112">Representa o nome da classe de objeto de resposta RemoveItem como uma cadeia de caracteres de inglês.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9fcb2-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9fcb2-113">Child elements</span></span>

|<span data-ttu-id="9fcb2-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-114">**Element**</span></span>|<span data-ttu-id="9fcb2-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fcb2-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="9fcb2-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="9fcb2-117">Identifica o item para o qual o objeto de resposta RemoveItem refere-se.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9fcb2-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9fcb2-118">Parent elements</span></span>

|<span data-ttu-id="9fcb2-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-119">**Element**</span></span>|<span data-ttu-id="9fcb2-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fcb2-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fcb2-121">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="9fcb2-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="9fcb2-122">Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="9fcb2-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="9fcb2-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="9fcb2-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="9fcb2-124">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9fcb2-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="9fcb2-125">Remarks</span></span>

 <span data-ttu-id="9fcb2-126">**RemoveItem** é válida apenas para um [MeetingCancellation](meetingcancellation.md).</span><span class="sxs-lookup"><span data-stu-id="9fcb2-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="9fcb2-127">Caso contrário, será gerado um erro.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="9fcb2-128">O [ItemClass](itemclass.md) para o cancelamento da reunião é IPM. Schedule.Meeting.Canceled.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="9fcb2-129">Para remover um [MeetingRequest](meetingrequest.md) e o associado [CalendarItem](calendaritem.md), use o objeto de resposta de [DeclineItem](declineitem.md) , em vez de **RemoveItem**.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="9fcb2-130">Não há suporte para **RemoveItem** para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="9fcb2-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9fcb2-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fcb2-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9fcb2-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fcb2-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fcb2-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fcb2-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9fcb2-134">Schema Name</span></span>  <br/> |<span data-ttu-id="9fcb2-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9fcb2-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fcb2-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9fcb2-136">Validation File</span></span>  <br/> |<span data-ttu-id="9fcb2-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9fcb2-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fcb2-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9fcb2-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fcb2-139">False</span><span class="sxs-lookup"><span data-stu-id="9fcb2-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fcb2-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="9fcb2-140">See also</span></span>



- [<span data-ttu-id="9fcb2-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9fcb2-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

