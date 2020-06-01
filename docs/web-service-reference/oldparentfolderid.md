---
title: OldParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldParentFolderId
api_type:
- schema
ms.assetid: da1b8c88-c650-455d-b749-0cd160b012d8
description: O elemento OldParentFolderId contém o identificador da pasta pai de um item ou pasta que foi copiado ou movido.
ms.openlocfilehash: ad787e95f95b551393878b15783461d93ac08481
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467225"
---
# <a name="oldparentfolderid"></a><span data-ttu-id="3fe48-103">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3fe48-103">OldParentFolderId</span></span>

<span data-ttu-id="3fe48-104">O elemento **OldParentFolderId** contém o identificador da pasta pai de um item ou pasta que foi copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="3fe48-104">The **OldParentFolderId** element contains the identifier of the parent folder of an item or folder that was copied or moved.</span></span> 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="3fe48-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="3fe48-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fe48-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3fe48-106">Attributes and elements</span></span>

<span data-ttu-id="3fe48-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3fe48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fe48-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3fe48-108">Attributes</span></span>

|<span data-ttu-id="3fe48-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="3fe48-109">**Attribute**</span></span>|<span data-ttu-id="3fe48-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3fe48-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3fe48-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="3fe48-111">**Id**</span></span> <br/> |<span data-ttu-id="3fe48-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fe48-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="3fe48-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="3fe48-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="3fe48-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="3fe48-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="3fe48-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo ID.</span><span class="sxs-lookup"><span data-stu-id="3fe48-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="3fe48-116">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="3fe48-116">This attribute is optional.</span></span> <span data-ttu-id="3fe48-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="3fe48-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3fe48-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3fe48-118">Child elements</span></span>

<span data-ttu-id="3fe48-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3fe48-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3fe48-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3fe48-120">Parent elements</span></span>

|<span data-ttu-id="3fe48-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3fe48-121">**Element**</span></span>|<span data-ttu-id="3fe48-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3fe48-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fe48-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="3fe48-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="3fe48-124">Representa um evento no qual um item ou pasta é copiado.</span><span class="sxs-lookup"><span data-stu-id="3fe48-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="3fe48-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="3fe48-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="3fe48-126">Representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="3fe48-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3fe48-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="3fe48-127">Remarks</span></span>

<span data-ttu-id="3fe48-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3fe48-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fe48-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3fe48-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fe48-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="3fe48-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fe48-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3fe48-131">Schema Name</span></span>  <br/> |<span data-ttu-id="3fe48-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3fe48-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fe48-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3fe48-133">Validation File</span></span>  <br/> |<span data-ttu-id="3fe48-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3fe48-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fe48-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3fe48-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fe48-136">False</span><span class="sxs-lookup"><span data-stu-id="3fe48-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fe48-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="3fe48-137">See also</span></span>



[<span data-ttu-id="3fe48-138">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="3fe48-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3fe48-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="3fe48-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3fe48-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="3fe48-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="3fe48-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3fe48-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

