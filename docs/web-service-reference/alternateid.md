---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: O elemento AlternateId descreve um identificador para converter em uma solicitação e os resultados de um identificador convertido na resposta.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751080"
---
# <a name="alternateid"></a><span data-ttu-id="378ad-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="378ad-103">AlternateId</span></span>

<span data-ttu-id="378ad-104">O elemento **AlternateId** descreve um identificador para converter em uma solicitação e os resultados de um identificador convertido na resposta.</span><span class="sxs-lookup"><span data-stu-id="378ad-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="378ad-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="378ad-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="378ad-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="378ad-106">Attributes and elements</span></span>

<span data-ttu-id="378ad-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="378ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="378ad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="378ad-108">Attributes</span></span>

|<span data-ttu-id="378ad-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="378ad-109">**Attribute**</span></span>|<span data-ttu-id="378ad-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="378ad-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="378ad-111">Id</span><span class="sxs-lookup"><span data-stu-id="378ad-111">Id</span></span>  <br/> |<span data-ttu-id="378ad-112">Descreve o identificador de origem em uma solicitação de [operação ConvertId](convertid-operation.md) e o identificador de destino em uma resposta de [operação ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="378ad-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="378ad-113">Format</span><span class="sxs-lookup"><span data-stu-id="378ad-113">Format</span></span>  <br/> |<span data-ttu-id="378ad-114">Descreve o formato de fonte em uma solicitação de [operação ConvertId](convertid-operation.md) e o formato de destino em uma resposta de [operação ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="378ad-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="378ad-115">O formato de destino é descrito pelo atributo **DestinationFormat** do elemento [ConvertId](convertid.md) na solicitação.</span><span class="sxs-lookup"><span data-stu-id="378ad-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="378ad-116">Este atributo é do tipo **IdFormatType**.</span><span class="sxs-lookup"><span data-stu-id="378ad-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="378ad-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="378ad-117">Mailbox</span></span>  <br/> |<span data-ttu-id="378ad-118">Descreve o endereço Simple Mail Transfer Protocol (SMTP) da caixa de correio principal que contém os identificadores para converter.</span><span class="sxs-lookup"><span data-stu-id="378ad-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="378ad-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="378ad-119">IsArchive</span></span>  <br/> |<span data-ttu-id="378ad-120">Indica se o identificador representa uma pasta ou um item arquivado.</span><span class="sxs-lookup"><span data-stu-id="378ad-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="378ad-121">Um valor **true** indica que o identificador representa uma pasta ou um item arquivado.</span><span class="sxs-lookup"><span data-stu-id="378ad-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="378ad-122">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="378ad-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="378ad-123">Valores de atributos de formato</span><span class="sxs-lookup"><span data-stu-id="378ad-123">Format attribute values</span></span>

|<span data-ttu-id="378ad-124">**Valor**</span><span class="sxs-lookup"><span data-stu-id="378ad-124">**Value**</span></span>|<span data-ttu-id="378ad-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="378ad-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="378ad-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="378ad-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="378ad-127">Descreve os identificadores que são produzidos pelo Exchange Web Services na versão inicial do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="378ad-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="378ad-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="378ad-128">EwsId</span></span>  <br/> |<span data-ttu-id="378ad-129">Descreve os identificadores que são produzidos pelo Exchange Web Services começando com o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="378ad-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="378ad-130">EntryId</span><span class="sxs-lookup"><span data-stu-id="378ad-130">EntryId</span></span>  <br/> |<span data-ttu-id="378ad-131">Descreve os identificadores MAPI, como a propriedade **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="378ad-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="378ad-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="378ad-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="378ad-133">Descreve uma representação hexadecimal codificado da propriedade **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="378ad-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="378ad-134">Este é o formato de identificadores de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="378ad-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="378ad-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="378ad-135">StoreId</span></span>  <br/> |<span data-ttu-id="378ad-136">Descreve os identificadores de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="378ad-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="378ad-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="378ad-137">OwaId</span></span>  <br/> |<span data-ttu-id="378ad-138">Descreve um identificador do Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="378ad-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="378ad-139">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="378ad-139">Child elements</span></span>

<span data-ttu-id="378ad-140">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="378ad-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="378ad-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="378ad-141">Parent elements</span></span>

|<span data-ttu-id="378ad-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="378ad-142">**Element**</span></span>|<span data-ttu-id="378ad-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="378ad-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="378ad-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="378ad-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="378ad-145">Contém o status e o resultado de uma solicitação de [operação ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="378ad-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="378ad-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="378ad-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="378ad-147">Contém os identificadores de origem para converter.</span><span class="sxs-lookup"><span data-stu-id="378ad-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="378ad-148">Text value</span><span class="sxs-lookup"><span data-stu-id="378ad-148">Text value</span></span>

<span data-ttu-id="378ad-149">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="378ad-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="378ad-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="378ad-150">Remarks</span></span>

<span data-ttu-id="378ad-151">O elemento **AlternateId** descreve os dois identificadores, o identificador de origem a ser convertido na solicitação de [operação ConvertId](convertid-operation.md) e o identificador convertido no elemento [ConvertIdResponse](convertidresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="378ad-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="378ad-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="378ad-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="378ad-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="378ad-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="378ad-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="378ad-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="378ad-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="378ad-155">Schema Name</span></span>  <br/> |<span data-ttu-id="378ad-156">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="378ad-156">Messages schema</span></span>  <br/> |<span data-ttu-id="378ad-157">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="378ad-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="378ad-158">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="378ad-158">Validation File</span></span>  <br/> |<span data-ttu-id="378ad-159">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="378ad-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="378ad-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="378ad-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="378ad-161">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="378ad-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="378ad-162">False</span><span class="sxs-lookup"><span data-stu-id="378ad-162">False</span></span>  <br/> |<span data-ttu-id="378ad-163">False</span><span class="sxs-lookup"><span data-stu-id="378ad-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="378ad-164">Ver também</span><span class="sxs-lookup"><span data-stu-id="378ad-164">See also</span></span>

- [<span data-ttu-id="378ad-165">Operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="378ad-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="378ad-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="378ad-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="378ad-167">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="378ad-167">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

