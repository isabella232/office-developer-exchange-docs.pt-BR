---
title: SuppressReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuppressReadReceipt
api_type:
- schema
ms.assetid: fc09bcc2-c003-4322-8315-d929bd0a9e2e
description: O elemento SuppressReadReceipt é usado para suprimir confirmações de leitura.
ms.openlocfilehash: de2eef68abd25c8208530ba5e98ab3278c8702d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837676"
---
# <a name="suppressreadreceipt"></a><span data-ttu-id="cc74f-103">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="cc74f-103">SuppressReadReceipt</span></span>

<span data-ttu-id="cc74f-104">O elemento **SuppressReadReceipt** é usado para suprimir confirmações de leitura.</span><span class="sxs-lookup"><span data-stu-id="cc74f-104">The **SuppressReadReceipt** element is used to suppress read receipts.</span></span> 
  
```xml
<SuppressReadReceipt>
   <ReferenceItemId/>
</SuppressReadReceipt>
```

 <span data-ttu-id="cc74f-105">**SuppressReadReceiptType**</span><span class="sxs-lookup"><span data-stu-id="cc74f-105">**SuppressReadReceiptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc74f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cc74f-106">Attributes and elements</span></span>

<span data-ttu-id="cc74f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cc74f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc74f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cc74f-108">Attributes</span></span>

<span data-ttu-id="cc74f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc74f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc74f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cc74f-110">Child elements</span></span>

|<span data-ttu-id="cc74f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc74f-111">**Element**</span></span>|<span data-ttu-id="cc74f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc74f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc74f-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="cc74f-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="cc74f-114">Identifica o item ao qual se refere no objeto response.</span><span class="sxs-lookup"><span data-stu-id="cc74f-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc74f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cc74f-115">Parent elements</span></span>

|<span data-ttu-id="cc74f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc74f-116">**Element**</span></span>|<span data-ttu-id="cc74f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc74f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc74f-118">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="cc74f-118">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="cc74f-119">Descreve todos os itens que são adjacentes para um horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="cc74f-119">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="cc74f-120">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="cc74f-120">The following are some of the XPath expressions to this element:</span></span><br/>  <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="cc74f-121">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="cc74f-121">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="cc74f-122">Descreve todos os itens que estão em conflito com um tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="cc74f-122">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="cc74f-123">A seguir estão algumas das expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="cc74f-123">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="cc74f-124">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="cc74f-124">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="cc74f-125">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc74f-125">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cc74f-126">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="cc74f-126">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="cc74f-127">Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="cc74f-127">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc74f-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="cc74f-128">Remarks</span></span>

<span data-ttu-id="cc74f-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cc74f-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc74f-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cc74f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc74f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc74f-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc74f-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cc74f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="cc74f-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cc74f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="cc74f-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cc74f-134">Validation File</span></span>  <br/> |<span data-ttu-id="cc74f-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cc74f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc74f-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cc74f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc74f-137">False</span><span class="sxs-lookup"><span data-stu-id="cc74f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc74f-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="cc74f-138">See also</span></span>

- [<span data-ttu-id="cc74f-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cc74f-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

