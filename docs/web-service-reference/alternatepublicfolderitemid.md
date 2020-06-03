---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: O elemento AlternatePublicFolderItemId descreve um identificador de item de pasta pública para converter para outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 11a9fafec78a9bd14e4d98982fd38954d45e4d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464767"
---
# <a name="alternatepublicfolderitemid"></a><span data-ttu-id="0c78e-104">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="0c78e-104">AlternatePublicFolderItemId</span></span>

<span data-ttu-id="0c78e-105">O elemento **AlternatePublicFolderItemId** descreve um identificador de item de pasta pública para converter para outro formato de identificador.</span><span class="sxs-lookup"><span data-stu-id="0c78e-105">The **AlternatePublicFolderItemId** element describes a public folder item identifier to convert to another identifier format.</span></span> <span data-ttu-id="0c78e-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0c78e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
- [<span data-ttu-id="0c78e-107">ConvertId</span><span class="sxs-lookup"><span data-stu-id="0c78e-107">ConvertId</span></span>](convertid.md)
  
- [<span data-ttu-id="0c78e-108">SourceIds</span><span class="sxs-lookup"><span data-stu-id="0c78e-108">SourceIds</span></span>](sourceids.md)
  
- [<span data-ttu-id="0c78e-109">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="0c78e-109">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 <span data-ttu-id="0c78e-110">**AlternatePublicFolderItemIdType**</span><span class="sxs-lookup"><span data-stu-id="0c78e-110">**AlternatePublicFolderItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c78e-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0c78e-111">Attributes and elements</span></span>

<span data-ttu-id="0c78e-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0c78e-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c78e-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="0c78e-113">Attributes</span></span>

|<span data-ttu-id="0c78e-114">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="0c78e-114">**Attribute**</span></span>|<span data-ttu-id="0c78e-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c78e-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c78e-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="0c78e-116">FolderId</span></span>  <br/> |<span data-ttu-id="0c78e-117">Identifica a pasta pública que contém o item de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="0c78e-117">Identifies the public folder that contains the public folder item.</span></span> <span data-ttu-id="0c78e-118">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="0c78e-118">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="0c78e-119">Formatar</span><span class="sxs-lookup"><span data-stu-id="0c78e-119">Format</span></span>  <br/> |<span data-ttu-id="0c78e-120">Identifica o formato que descreve o identificador de item de pasta pública a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="0c78e-120">Identifies the format that describes the public folder item identifier to convert.</span></span> <span data-ttu-id="0c78e-121">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="0c78e-121">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="0c78e-122">ItemId</span><span class="sxs-lookup"><span data-stu-id="0c78e-122">ItemId</span></span>  <br/> |<span data-ttu-id="0c78e-123">Identificador o item de pasta pública a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="0c78e-123">Identifier the public folder item to convert.</span></span> <span data-ttu-id="0c78e-124">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="0c78e-124">This attribute is required.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="0c78e-125">Valores de atributo de formato</span><span class="sxs-lookup"><span data-stu-id="0c78e-125">Format attribute values</span></span>

|<span data-ttu-id="0c78e-126">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0c78e-126">**Value**</span></span>|<span data-ttu-id="0c78e-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c78e-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c78e-128">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="0c78e-128">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="0c78e-129">Descreve os identificadores produzidos pelos serviços Web do Exchange na versão inicial de lançamento do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="0c78e-129">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="0c78e-130">EwsId</span><span class="sxs-lookup"><span data-stu-id="0c78e-130">EwsId</span></span>  <br/> |<span data-ttu-id="0c78e-131">Descreve os identificadores produzidos pelos serviços Web do Exchange a partir do Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0c78e-131">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="0c78e-132">EntryId</span><span class="sxs-lookup"><span data-stu-id="0c78e-132">EntryId</span></span>  <br/> |<span data-ttu-id="0c78e-133">Descreve os identificadores MAPI, como na propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="0c78e-133">Describes MAPI identifiers, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="0c78e-134">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="0c78e-134">HexEntryId</span></span>  <br/> |<span data-ttu-id="0c78e-135">Descreve uma representação codificada hexadecimal da propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="0c78e-135">Describes a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span> <span data-ttu-id="0c78e-136">Este é o formato de identificadores de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c78e-136">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="0c78e-137">StoreId</span><span class="sxs-lookup"><span data-stu-id="0c78e-137">StoreId</span></span>  <br/> |<span data-ttu-id="0c78e-138">Descreve os identificadores de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c78e-138">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="0c78e-139">OwaId</span><span class="sxs-lookup"><span data-stu-id="0c78e-139">OwaId</span></span>  <br/> |<span data-ttu-id="0c78e-140">Descreve um identificador do Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="0c78e-140">Describes an Outlook Web Access identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0c78e-141">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0c78e-141">Child elements</span></span>

<span data-ttu-id="0c78e-142">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c78e-142">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0c78e-143">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0c78e-143">Parent elements</span></span>

|<span data-ttu-id="0c78e-144">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c78e-144">**Element**</span></span>|<span data-ttu-id="0c78e-145">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c78e-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c78e-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="0c78e-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="0c78e-147">Contém os identificadores de origem a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="0c78e-147">Contains the source identifiers to convert.</span></span> <span data-ttu-id="0c78e-148">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0c78e-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c78e-149">Comentários</span><span class="sxs-lookup"><span data-stu-id="0c78e-149">Remarks</span></span>

<span data-ttu-id="0c78e-150">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0c78e-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c78e-151">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0c78e-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c78e-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c78e-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c78e-153">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0c78e-153">Schema Name</span></span>  <br/> |<span data-ttu-id="0c78e-154">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0c78e-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c78e-155">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0c78e-155">Validation File</span></span>  <br/> |<span data-ttu-id="0c78e-156">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0c78e-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c78e-157">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0c78e-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c78e-158">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0c78e-158">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c78e-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="0c78e-159">See also</span></span>

- [<span data-ttu-id="0c78e-160">Operação convertid</span><span class="sxs-lookup"><span data-stu-id="0c78e-160">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="0c78e-161">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c78e-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="0c78e-162">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="0c78e-162">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

