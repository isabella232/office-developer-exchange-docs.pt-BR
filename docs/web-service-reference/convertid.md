---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: O elemento convertid define uma solicitação para converter o item e os identificadores de pasta entre os formatos compatíveis com o Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452535"
---
# <a name="convertid"></a><span data-ttu-id="bf659-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="bf659-104">ConvertId</span></span>

<span data-ttu-id="bf659-105">O elemento **convertid** define uma solicitação para converter o item e os identificadores de pasta entre os formatos compatíveis com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf659-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="bf659-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bf659-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="bf659-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="bf659-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf659-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bf659-108">Attributes and elements</span></span>

<span data-ttu-id="bf659-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bf659-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf659-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="bf659-110">Attributes</span></span>

|<span data-ttu-id="bf659-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="bf659-111">**Attribute**</span></span>|<span data-ttu-id="bf659-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf659-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf659-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="bf659-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="bf659-114">Descreve o formato de identificador que será retornado para todos os identificadores convertidos.</span><span class="sxs-lookup"><span data-stu-id="bf659-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="bf659-115">O DestinationFormat é descrito pelo IdFormattype.</span><span class="sxs-lookup"><span data-stu-id="bf659-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="bf659-116">Atributo DestinationFormat</span><span class="sxs-lookup"><span data-stu-id="bf659-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="bf659-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="bf659-117">**Value**</span></span>|<span data-ttu-id="bf659-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf659-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bf659-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="bf659-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="bf659-120">Representa o formato de identificador usado para os identificadores de serviços Web do Exchange fornecidos na versão inicial de lançamento do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="bf659-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="bf659-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="bf659-121">**EwsId**</span></span> <br/> |<span data-ttu-id="bf659-122">Representa o formato de identificador usado para identificadores de serviços Web do Exchange a partir do Exchange Server 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="bf659-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="bf659-123">**EntryId**</span><span class="sxs-lookup"><span data-stu-id="bf659-123">**EntryId**</span></span> <br/> |<span data-ttu-id="bf659-124">Representa o identificador MAPI, como na propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="bf659-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="bf659-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="bf659-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="bf659-126">Representa o identificador de eventos do calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf659-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="bf659-127">Esta é uma representação codificada em hexadecimal da propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="bf659-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="bf659-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="bf659-128">**StoreId**</span></span> <br/> |<span data-ttu-id="bf659-129">Representa o identificador do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf659-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="bf659-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="bf659-130">**OwaId**</span></span> <br/> |<span data-ttu-id="bf659-131">Representa o formato de identificador do Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="bf659-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bf659-132">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bf659-132">Child elements</span></span>

|<span data-ttu-id="bf659-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bf659-133">**Element**</span></span>|<span data-ttu-id="bf659-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf659-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf659-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="bf659-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="bf659-136">Contém os identificadores de origem a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="bf659-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf659-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bf659-137">Parent elements</span></span>

<span data-ttu-id="bf659-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf659-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf659-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf659-139">Remarks</span></span>

<span data-ttu-id="bf659-140">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="bf659-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf659-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bf659-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf659-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="bf659-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bf659-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bf659-143">Schema Name</span></span>  <br/> |<span data-ttu-id="bf659-144">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="bf659-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="bf659-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bf659-145">Validation File</span></span>  <br/> |<span data-ttu-id="bf659-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bf659-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bf659-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bf659-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf659-148">False</span><span class="sxs-lookup"><span data-stu-id="bf659-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf659-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf659-149">See also</span></span>



[<span data-ttu-id="bf659-150">Operação convertid</span><span class="sxs-lookup"><span data-stu-id="bf659-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="bf659-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bf659-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="bf659-152">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="bf659-152">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

