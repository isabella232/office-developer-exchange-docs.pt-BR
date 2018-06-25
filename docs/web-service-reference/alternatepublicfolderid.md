---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: O elemento AlternatePublicFolderId descreve um identificador de pasta pública para converter em outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751087"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="700ad-104">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="700ad-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="700ad-105">O elemento **AlternatePublicFolderId** descreve um identificador de pasta pública para converter em outro formato de identificador.</span><span class="sxs-lookup"><span data-stu-id="700ad-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="700ad-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="700ad-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="700ad-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="700ad-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="700ad-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="700ad-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="700ad-109">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="700ad-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="700ad-110">**AlternatePublicFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="700ad-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="700ad-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="700ad-111">Attributes and elements</span></span>

<span data-ttu-id="700ad-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="700ad-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="700ad-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="700ad-113">Attributes</span></span>

|<span data-ttu-id="700ad-114">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="700ad-114">**Attribute**</span></span>|<span data-ttu-id="700ad-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="700ad-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="700ad-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="700ad-116">FolderId</span></span>  <br/> |<span data-ttu-id="700ad-117">Contém o identificador de pasta pública para converter.</span><span class="sxs-lookup"><span data-stu-id="700ad-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="700ad-118">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="700ad-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="700ad-119">Format</span><span class="sxs-lookup"><span data-stu-id="700ad-119">Format</span></span>  <br/> |<span data-ttu-id="700ad-120">Identifica o formato que descreve o identificador de pasta pública para converter.</span><span class="sxs-lookup"><span data-stu-id="700ad-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="700ad-121">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="700ad-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="700ad-122">Atributo Format</span><span class="sxs-lookup"><span data-stu-id="700ad-122">Format attribute</span></span>

|<span data-ttu-id="700ad-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="700ad-123">**Value**</span></span>|<span data-ttu-id="700ad-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="700ad-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="700ad-125">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="700ad-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="700ad-126">Descreve os identificadores que são produzidos pelo Exchange Web Services na versão inicial do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="700ad-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="700ad-127">EwsId</span><span class="sxs-lookup"><span data-stu-id="700ad-127">EwsId</span></span>  <br/> |<span data-ttu-id="700ad-128">Descreve os identificadores que são produzidos pelo Exchange Web Services começando com o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="700ad-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="700ad-129">EntryId</span><span class="sxs-lookup"><span data-stu-id="700ad-129">EntryId</span></span>  <br/> |<span data-ttu-id="700ad-130">Descreve os identificadores MAPI, como a propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="700ad-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="700ad-131">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="700ad-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="700ad-132">Descreve uma representação hexadecimal codificado da propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="700ad-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="700ad-133">Este é o formato de identificadores de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="700ad-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="700ad-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="700ad-134">StoreId</span></span>  <br/> |<span data-ttu-id="700ad-135">Descreve os identificadores de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="700ad-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="700ad-136">OwaId</span><span class="sxs-lookup"><span data-stu-id="700ad-136">OwaId</span></span>  <br/> |<span data-ttu-id="700ad-137">Descreve um identificador do Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="700ad-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="700ad-138">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="700ad-138">Child elements</span></span>

<span data-ttu-id="700ad-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="700ad-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="700ad-140">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="700ad-140">Parent elements</span></span>

|<span data-ttu-id="700ad-141">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="700ad-141">**Element**</span></span>|<span data-ttu-id="700ad-142">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="700ad-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="700ad-143">SourceIds</span><span class="sxs-lookup"><span data-stu-id="700ad-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="700ad-144">Contém os identificadores de origem para converter.</span><span class="sxs-lookup"><span data-stu-id="700ad-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="700ad-145">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="700ad-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="700ad-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="700ad-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="700ad-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="700ad-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="700ad-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="700ad-148">Schema Name</span></span>  <br/> |<span data-ttu-id="700ad-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="700ad-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="700ad-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="700ad-150">Validation File</span></span>  <br/> |<span data-ttu-id="700ad-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="700ad-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="700ad-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="700ad-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="700ad-153">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="700ad-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="700ad-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="700ad-154">See also</span></span>

- [<span data-ttu-id="700ad-155">Operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="700ad-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="700ad-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="700ad-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="700ad-157">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="700ad-157">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

