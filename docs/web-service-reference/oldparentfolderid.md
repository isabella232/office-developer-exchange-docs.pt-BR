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
description: O elemento OldParentFolderId contém o identificador da pasta pai de um item ou a pasta que foi copiada ou movida.
ms.openlocfilehash: 1c4a51755c4194939dd797efa31cf5410b02bf85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824644"
---
# <a name="oldparentfolderid"></a><span data-ttu-id="3cbc3-103">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3cbc3-103">OldParentFolderId</span></span>

<span data-ttu-id="3cbc3-104">O elemento **OldParentFolderId** contém o identificador da pasta pai de um item ou a pasta que foi copiada ou movida.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-104">The **OldParentFolderId** element contains the identifier of the parent folder of an item or folder that was copied or moved.</span></span> 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="3cbc3-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cbc3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3cbc3-106">Attributes and elements</span></span>

<span data-ttu-id="3cbc3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cbc3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3cbc3-108">Attributes</span></span>

|<span data-ttu-id="3cbc3-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-109">**Attribute**</span></span>|<span data-ttu-id="3cbc3-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3cbc3-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-111">**Id**</span></span> <br/> |<span data-ttu-id="3cbc3-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="3cbc3-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="3cbc3-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="3cbc3-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo Id.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="3cbc3-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-116">This attribute is optional.</span></span> <span data-ttu-id="3cbc3-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3cbc3-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3cbc3-118">Child elements</span></span>

<span data-ttu-id="3cbc3-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3cbc3-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3cbc3-120">Parent elements</span></span>

|<span data-ttu-id="3cbc3-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-121">**Element**</span></span>|<span data-ttu-id="3cbc3-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3cbc3-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cbc3-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="3cbc3-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="3cbc3-124">Representa um evento no qual uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="3cbc3-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="3cbc3-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="3cbc3-126">Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3cbc3-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="3cbc3-127">Remarks</span></span>

<span data-ttu-id="3cbc3-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3cbc3-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3cbc3-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3cbc3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cbc3-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="3cbc3-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cbc3-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3cbc3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="3cbc3-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3cbc3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3cbc3-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3cbc3-133">Validation File</span></span>  <br/> |<span data-ttu-id="3cbc3-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3cbc3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cbc3-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3cbc3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="3cbc3-136">False</span><span class="sxs-lookup"><span data-stu-id="3cbc3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cbc3-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="3cbc3-137">See also</span></span>



[<span data-ttu-id="3cbc3-138">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="3cbc3-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3cbc3-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="3cbc3-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3cbc3-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="3cbc3-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="3cbc3-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3cbc3-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

