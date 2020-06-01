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
description: O elemento AcceptSharingInvitation é usado para aceitar um convite que permite o acesso a dados do calendário ou contatos de outro usuário.
ms.openlocfilehash: c8cdae707bd122e74fa0e284163d1540d857c3de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461706"
---
# <a name="acceptsharinginvitation"></a><span data-ttu-id="9fb31-103">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="9fb31-103">AcceptSharingInvitation</span></span>

<span data-ttu-id="9fb31-104">O elemento **AcceptSharingInvitation** é usado para aceitar um convite que permite o acesso a dados do calendário ou contatos de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="9fb31-104">The **AcceptSharingInvitation** element is used to accept an invitation that allows access to another user's calendar or contacts data.</span></span> 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 <span data-ttu-id="9fb31-105">**AcceptSharingInvitationType**</span><span class="sxs-lookup"><span data-stu-id="9fb31-105">**AcceptSharingInvitationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fb31-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9fb31-106">Attributes and elements</span></span>

<span data-ttu-id="9fb31-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9fb31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fb31-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9fb31-108">Attributes</span></span>

<span data-ttu-id="9fb31-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fb31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fb31-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9fb31-110">Child elements</span></span>

|<span data-ttu-id="9fb31-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fb31-111">**Element**</span></span>|<span data-ttu-id="9fb31-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fb31-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fb31-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="9fb31-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="9fb31-114">Identifica o item ao qual o objeto Response se refere.</span><span class="sxs-lookup"><span data-stu-id="9fb31-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9fb31-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9fb31-115">Parent elements</span></span>

|<span data-ttu-id="9fb31-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fb31-116">**Element**</span></span>|<span data-ttu-id="9fb31-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fb31-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fb31-118">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="9fb31-118">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="9fb31-119">Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fb31-119">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9fb31-120">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="9fb31-120">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="9fb31-121">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="9fb31-121">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9fb31-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="9fb31-122">Remarks</span></span>

<span data-ttu-id="9fb31-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fb31-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fb31-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9fb31-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fb31-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fb31-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fb31-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9fb31-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9fb31-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9fb31-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fb31-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9fb31-128">Validation File</span></span>  <br/> |<span data-ttu-id="9fb31-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9fb31-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fb31-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9fb31-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fb31-131">False</span><span class="sxs-lookup"><span data-stu-id="9fb31-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fb31-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="9fb31-132">See also</span></span>

- [<span data-ttu-id="9fb31-133">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="9fb31-133">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md)
- [<span data-ttu-id="9fb31-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9fb31-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

