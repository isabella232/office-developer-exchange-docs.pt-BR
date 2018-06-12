---
title: OldItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldItemId
api_type:
- schema
ms.assetid: fb57deee-9cc3-4730-9805-ff34f39e3ab7
description: O elemento OldItemId contém o identificador exclusivo do item que foi copiado ou movido.
ms.openlocfilehash: ced7fc6891e0d1fde42a8cb9cad4f4e55493b5d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824648"
---
# <a name="olditemid"></a><span data-ttu-id="676ff-103">OldItemId</span><span class="sxs-lookup"><span data-stu-id="676ff-103">OldItemId</span></span>

<span data-ttu-id="676ff-104">O elemento **OldItemId** contém o identificador exclusivo do item que foi copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="676ff-104">The **OldItemId** element contains the unique identifier of the item that was copied or moved.</span></span> 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="676ff-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="676ff-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="676ff-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="676ff-106">Attributes and elements</span></span>

<span data-ttu-id="676ff-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="676ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="676ff-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="676ff-108">Attributes</span></span>

|<span data-ttu-id="676ff-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="676ff-109">**Attribute**</span></span>|<span data-ttu-id="676ff-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="676ff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="676ff-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="676ff-111">**Id**</span></span> <br/> |<span data-ttu-id="676ff-112">Contém uma cadeia de caracteres que identifica um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="676ff-112">Contains a string that identifies an item in the Exchange store.</span></span> <span data-ttu-id="676ff-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="676ff-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="676ff-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="676ff-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="676ff-115">Contém uma cadeia de caracteres que identifica uma versão de um item que é identificado pelo atributo Id.</span><span class="sxs-lookup"><span data-stu-id="676ff-115">Contains a string that identifies a version of an item that is identified by the Id attribute.</span></span> <span data-ttu-id="676ff-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="676ff-116">This attribute is optional.</span></span> <span data-ttu-id="676ff-117">Use este atributo para certificar-se de que a versão correta de um item é usada.</span><span class="sxs-lookup"><span data-stu-id="676ff-117">Use this attribute to make sure that the correct version of an item is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="676ff-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="676ff-118">Child elements</span></span>

<span data-ttu-id="676ff-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="676ff-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="676ff-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="676ff-120">Parent elements</span></span>

|<span data-ttu-id="676ff-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="676ff-121">**Element**</span></span>|<span data-ttu-id="676ff-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="676ff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="676ff-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="676ff-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="676ff-124">Representa um evento no qual uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="676ff-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="676ff-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="676ff-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="676ff-126">Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="676ff-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="676ff-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="676ff-127">Remarks</span></span>

<span data-ttu-id="676ff-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="676ff-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="676ff-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="676ff-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="676ff-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="676ff-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="676ff-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="676ff-131">Schema Name</span></span>  <br/> |<span data-ttu-id="676ff-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="676ff-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="676ff-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="676ff-133">Validation File</span></span>  <br/> |<span data-ttu-id="676ff-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="676ff-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="676ff-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="676ff-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="676ff-136">False</span><span class="sxs-lookup"><span data-stu-id="676ff-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="676ff-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="676ff-137">See also</span></span>



[<span data-ttu-id="676ff-138">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="676ff-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="676ff-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="676ff-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="676ff-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="676ff-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="676ff-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="676ff-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

