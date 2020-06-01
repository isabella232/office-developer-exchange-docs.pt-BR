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
description: O elemento AlternatePublicFolderId descreve um identificador de pasta pública para converter para outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 54ad663117839222ea1174cd1c25600f31aa6b43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464795"
---
# <a name="alternatepublicfolderid"></a><span data-ttu-id="0c439-104">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="0c439-104">AlternatePublicFolderId</span></span>

<span data-ttu-id="0c439-105">O elemento **AlternatePublicFolderId** descreve um identificador de pasta pública para converter para outro formato de identificador.</span><span class="sxs-lookup"><span data-stu-id="0c439-105">The **AlternatePublicFolderId** element describes a public folder identifier to convert to another identifier format.</span></span> <span data-ttu-id="0c439-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0c439-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="0c439-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="0c439-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="0c439-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="0c439-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="0c439-109">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="0c439-109">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 <span data-ttu-id="0c439-110">**AlternatePublicFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="0c439-110">**AlternatePublicFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c439-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0c439-111">Attributes and elements</span></span>

<span data-ttu-id="0c439-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0c439-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c439-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="0c439-113">Attributes</span></span>

|<span data-ttu-id="0c439-114">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="0c439-114">**Attribute**</span></span>|<span data-ttu-id="0c439-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c439-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c439-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="0c439-116">FolderId</span></span>  <br/> |<span data-ttu-id="0c439-117">Contém o identificador de pasta pública a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="0c439-117">Contains the public folder identifier to convert.</span></span> <span data-ttu-id="0c439-118">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="0c439-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="0c439-119">Formatar</span><span class="sxs-lookup"><span data-stu-id="0c439-119">Format</span></span>  <br/> |<span data-ttu-id="0c439-120">Identifica o formato que descreve o identificador de pasta pública a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="0c439-120">Identifies the format that describes the public folder identifier to convert.</span></span> <span data-ttu-id="0c439-121">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="0c439-121">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute"></a><span data-ttu-id="0c439-122">Atributo Format</span><span class="sxs-lookup"><span data-stu-id="0c439-122">Format attribute</span></span>

|<span data-ttu-id="0c439-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0c439-123">**Value**</span></span>|<span data-ttu-id="0c439-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c439-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c439-125">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="0c439-125">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="0c439-126">Descreve os identificadores produzidos pelos serviços Web do Exchange na versão inicial de lançamento do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="0c439-126">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="0c439-127">EwsId</span><span class="sxs-lookup"><span data-stu-id="0c439-127">EwsId</span></span>  <br/> |<span data-ttu-id="0c439-128">Descreve os identificadores produzidos pelos serviços Web do Exchange a partir do Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0c439-128">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="0c439-129">EntryId</span><span class="sxs-lookup"><span data-stu-id="0c439-129">EntryId</span></span>  <br/> |<span data-ttu-id="0c439-130">Descreve os identificadores MAPI, como na propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="0c439-130">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="0c439-131">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="0c439-131">HexEntryId</span></span>  <br/> |<span data-ttu-id="0c439-132">Descreve uma representação codificada hexadecimal da propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="0c439-132">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="0c439-133">Este é o formato de identificadores de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c439-133">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="0c439-134">StoreId</span><span class="sxs-lookup"><span data-stu-id="0c439-134">StoreId</span></span>  <br/> |<span data-ttu-id="0c439-135">Descreve os identificadores de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c439-135">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="0c439-136">OwaId</span><span class="sxs-lookup"><span data-stu-id="0c439-136">OwaId</span></span>  <br/> |<span data-ttu-id="0c439-137">Descreve um identificador do Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="0c439-137">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0c439-138">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0c439-138">Child elements</span></span>

<span data-ttu-id="0c439-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c439-139">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0c439-140">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0c439-140">Parent elements</span></span>

|<span data-ttu-id="0c439-141">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c439-141">**Element**</span></span>|<span data-ttu-id="0c439-142">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c439-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c439-143">SourceIds</span><span class="sxs-lookup"><span data-stu-id="0c439-143">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="0c439-144">Contém os identificadores de origem a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="0c439-144">Contains the source identifiers to convert.</span></span> <span data-ttu-id="0c439-145">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0c439-145">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="0c439-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0c439-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c439-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c439-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c439-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0c439-148">Schema Name</span></span>  <br/> |<span data-ttu-id="0c439-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0c439-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c439-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0c439-150">Validation File</span></span>  <br/> |<span data-ttu-id="0c439-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0c439-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c439-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0c439-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c439-153">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0c439-153">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c439-154">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0c439-154">See also</span></span>

- [<span data-ttu-id="0c439-155">Operação convertid</span><span class="sxs-lookup"><span data-stu-id="0c439-155">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="0c439-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c439-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="0c439-157">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="0c439-157">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

