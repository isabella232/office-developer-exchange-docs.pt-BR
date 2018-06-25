---
title: AcceptSharingInvitation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptSharingInvitation
api_type:
- schema
ms.assetid: 3c2a47d6-490d-425b-8893-089a4f8882cd
description: O elemento AcceptSharingInvitation é usado para aceitar um convite que permite o acesso aos dados de contatos ou de calendário de outro usuário.
ms.openlocfilehash: 06439739e6cc544d5039ac9d18e0452b1d42a0ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752191"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="c188b-103">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="c188b-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="c188b-104">O elemento **AcceptSharingInvitation** é usado para aceitar um convite que permite o acesso aos dados de contatos ou de calendário de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="c188b-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="c188b-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="c188b-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c188b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c188b-106">Attributes and elements</span></span>

<span data-ttu-id="c188b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c188b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c188b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c188b-108">Attributes</span></span>

<span data-ttu-id="c188b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c188b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c188b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c188b-110">Child elements</span></span>

|<span data-ttu-id="c188b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c188b-111">**Element**</span></span>|<span data-ttu-id="c188b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c188b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c188b-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="c188b-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="c188b-114">Identifica o item ao qual se refere no objeto response.</span><span class="sxs-lookup"><span data-stu-id="c188b-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c188b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c188b-115">Parent elements</span></span>

|<span data-ttu-id="c188b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c188b-116">**Element**</span></span>|<span data-ttu-id="c188b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c188b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c188b-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="c188b-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="c188b-119">Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c188b-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c188b-120">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="c188b-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="c188b-121">Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="c188b-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c188b-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c188b-122">Remarks</span></span>

<span data-ttu-id="c188b-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c188b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c188b-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c188b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c188b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c188b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c188b-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c188b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c188b-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c188b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c188b-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c188b-128">Validation File</span></span>  <br/> |<span data-ttu-id="c188b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c188b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c188b-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c188b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c188b-131">False</span><span class="sxs-lookup"><span data-stu-id="c188b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c188b-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="c188b-132">See also</span></span>

- [<span data-ttu-id="c188b-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="c188b-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="c188b-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c188b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

