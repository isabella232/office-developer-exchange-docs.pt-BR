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
ms.openlocfilehash: 9fab14478ffbb2dd8ad013d59520af943584f2eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467463"
---
# <a name="olditemid"></a><span data-ttu-id="8c531-103">OldItemId</span><span class="sxs-lookup"><span data-stu-id="8c531-103">OldItemId</span></span>

<span data-ttu-id="8c531-104">O elemento **OldItemId** contém o identificador exclusivo do item que foi copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="8c531-104">The **OldItemId** element contains the unique identifier of the item that was copied or moved.</span></span> 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="8c531-105">**ItemIdtype**</span><span class="sxs-lookup"><span data-stu-id="8c531-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c531-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8c531-106">Attributes and elements</span></span>

<span data-ttu-id="8c531-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8c531-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c531-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8c531-108">Attributes</span></span>

|<span data-ttu-id="8c531-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="8c531-109">**Attribute**</span></span>|<span data-ttu-id="8c531-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8c531-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8c531-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="8c531-111">**Id**</span></span> <br/> |<span data-ttu-id="8c531-112">Contém uma cadeia de caracteres que identifica um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c531-112">Contains a string that identifies an item in the Exchange store.</span></span> <span data-ttu-id="8c531-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="8c531-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="8c531-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="8c531-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="8c531-115">Contém uma cadeia de caracteres que identifica uma versão de um item que é identificada pelo atributo ID.</span><span class="sxs-lookup"><span data-stu-id="8c531-115">Contains a string that identifies a version of an item that is identified by the Id attribute.</span></span> <span data-ttu-id="8c531-116">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="8c531-116">This attribute is optional.</span></span> <span data-ttu-id="8c531-117">Use este atributo para certificar-se de que a versão correta de um item é usada.</span><span class="sxs-lookup"><span data-stu-id="8c531-117">Use this attribute to make sure that the correct version of an item is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8c531-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8c531-118">Child elements</span></span>

<span data-ttu-id="8c531-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8c531-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c531-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8c531-120">Parent elements</span></span>

|<span data-ttu-id="8c531-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8c531-121">**Element**</span></span>|<span data-ttu-id="8c531-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8c531-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c531-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="8c531-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="8c531-124">Representa um evento no qual um item ou pasta é copiado.</span><span class="sxs-lookup"><span data-stu-id="8c531-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="8c531-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="8c531-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="8c531-126">Representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="8c531-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8c531-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="8c531-127">Remarks</span></span>

<span data-ttu-id="8c531-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8c531-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c531-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8c531-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c531-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="8c531-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c531-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8c531-131">Schema Name</span></span>  <br/> |<span data-ttu-id="8c531-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8c531-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8c531-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8c531-133">Validation File</span></span>  <br/> |<span data-ttu-id="8c531-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8c531-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c531-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8c531-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="8c531-136">False</span><span class="sxs-lookup"><span data-stu-id="8c531-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c531-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="8c531-137">See also</span></span>



[<span data-ttu-id="8c531-138">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="8c531-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="8c531-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="8c531-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="8c531-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="8c531-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="8c531-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8c531-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

