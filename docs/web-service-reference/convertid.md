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
description: O elemento de ConvertId define uma solicitação para converter os identificadores de item e pasta entre formatos suportados do Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751535"
---
# <a name="convertid"></a><span data-ttu-id="69fb3-104">ConvertId</span><span class="sxs-lookup"><span data-stu-id="69fb3-104">ConvertId</span></span>

<span data-ttu-id="69fb3-105">O elemento de **ConvertId** define uma solicitação para converter os identificadores de item e pasta entre formatos suportados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="69fb3-105">The **ConvertId** element defines a request to convert item and folder identifiers between supported Exchange formats.</span></span> <span data-ttu-id="69fb3-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="69fb3-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 <span data-ttu-id="69fb3-107">**ConvertIdType**</span><span class="sxs-lookup"><span data-stu-id="69fb3-107">**ConvertIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69fb3-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="69fb3-108">Attributes and elements</span></span>

<span data-ttu-id="69fb3-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="69fb3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69fb3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="69fb3-110">Attributes</span></span>

|<span data-ttu-id="69fb3-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="69fb3-111">**Attribute**</span></span>|<span data-ttu-id="69fb3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="69fb3-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="69fb3-113">**DestinationFormat**</span><span class="sxs-lookup"><span data-stu-id="69fb3-113">**DestinationFormat**</span></span> <br/> |<span data-ttu-id="69fb3-114">Descreve o formato do identificador que será retornado para todos os identificadores convertidos.</span><span class="sxs-lookup"><span data-stu-id="69fb3-114">Describes the identifier format that will be returned for all the converted identifiers.</span></span> <span data-ttu-id="69fb3-115">O DestinationFormat é descrito pelo IdFormatType.</span><span class="sxs-lookup"><span data-stu-id="69fb3-115">The DestinationFormat is described by the IdFormatType.</span></span>  <br/> |
   
#### <a name="destinationformat-attribute"></a><span data-ttu-id="69fb3-116">Atributo DestinationFormat</span><span class="sxs-lookup"><span data-stu-id="69fb3-116">DestinationFormat Attribute</span></span>

|<span data-ttu-id="69fb3-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="69fb3-117">**Value**</span></span>|<span data-ttu-id="69fb3-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="69fb3-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="69fb3-119">**EwsLegacyId**</span><span class="sxs-lookup"><span data-stu-id="69fb3-119">**EwsLegacyId**</span></span> <br/> |<span data-ttu-id="69fb3-120">Representa o formato do identificador que é usado para os identificadores de serviços Web do Exchange que são fornecidos na versão inicial do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="69fb3-120">Represents the identifier format that is used for Exchange Web Services identifiers that are provided in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="69fb3-121">**EwsId**</span><span class="sxs-lookup"><span data-stu-id="69fb3-121">**EwsId**</span></span> <br/> |<span data-ttu-id="69fb3-122">Representa o formato do identificador que é usado para identificadores de serviços Web do Exchange, começando com o Exchange Server 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="69fb3-122">Represents the identifier format that is used for Exchange Web Services identifiers starting with Exchange Server 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="69fb3-123">**EntryId**</span><span class="sxs-lookup"><span data-stu-id="69fb3-123">**EntryId**</span></span> <br/> |<span data-ttu-id="69fb3-124">Representa o identificador MAPI, como a propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="69fb3-124">Represents the MAPI identifier, as in the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="69fb3-125">**HexEntryId**</span><span class="sxs-lookup"><span data-stu-id="69fb3-125">**HexEntryId**</span></span> <br/> |<span data-ttu-id="69fb3-126">Representa o identificador de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="69fb3-126">Represents the availability calendar event identifier.</span></span> <span data-ttu-id="69fb3-127">Esta é uma representação hexadecimal codificado da propriedade PR_ENTRYID.</span><span class="sxs-lookup"><span data-stu-id="69fb3-127">This is a hexadecimal-encoded representation of the PR_ENTRYID property.</span></span>  <br/> |
|<span data-ttu-id="69fb3-128">**StoreId**</span><span class="sxs-lookup"><span data-stu-id="69fb3-128">**StoreId**</span></span> <br/> |<span data-ttu-id="69fb3-129">Representa o identificador de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="69fb3-129">Represents the Exchange store identifier.</span></span>  <br/> |
|<span data-ttu-id="69fb3-130">**OwaId**</span><span class="sxs-lookup"><span data-stu-id="69fb3-130">**OwaId**</span></span> <br/> |<span data-ttu-id="69fb3-131">Representa o formato de identificador do Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="69fb3-131">Represents the Outlook Web Access identifier format.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="69fb3-132">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="69fb3-132">Child elements</span></span>

|<span data-ttu-id="69fb3-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="69fb3-133">**Element**</span></span>|<span data-ttu-id="69fb3-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="69fb3-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69fb3-135">SourceIds</span><span class="sxs-lookup"><span data-stu-id="69fb3-135">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="69fb3-136">Contém os identificadores de origem para converter.</span><span class="sxs-lookup"><span data-stu-id="69fb3-136">Contains the source identifiers to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69fb3-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="69fb3-137">Parent elements</span></span>

<span data-ttu-id="69fb3-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="69fb3-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69fb3-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="69fb3-139">Remarks</span></span>

<span data-ttu-id="69fb3-140">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="69fb3-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69fb3-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="69fb3-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69fb3-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="69fb3-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69fb3-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="69fb3-143">Schema Name</span></span>  <br/> |<span data-ttu-id="69fb3-144">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="69fb3-144">messages schema</span></span>  <br/> |
|<span data-ttu-id="69fb3-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="69fb3-145">Validation File</span></span>  <br/> |<span data-ttu-id="69fb3-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="69fb3-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69fb3-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="69fb3-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="69fb3-148">False</span><span class="sxs-lookup"><span data-stu-id="69fb3-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69fb3-149">Ver também</span><span class="sxs-lookup"><span data-stu-id="69fb3-149">See also</span></span>



[<span data-ttu-id="69fb3-150">Operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="69fb3-150">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="69fb3-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="69fb3-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="69fb3-152">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="69fb3-152">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

