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
description: O elemento Alternateid descreve um identificador a ser convertido em uma solicitação e os resultados de um identificador convertido na resposta.
ms.openlocfilehash: 26df68bd814c2d323630c6bb40b4c31745017c71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527450"
---
# <a name="alternateid"></a><span data-ttu-id="cea36-103">AlternateId</span><span class="sxs-lookup"><span data-stu-id="cea36-103">AlternateId</span></span>

<span data-ttu-id="cea36-104">O elemento **alternateid** descreve um identificador a ser convertido em uma solicitação e os resultados de um identificador convertido na resposta.</span><span class="sxs-lookup"><span data-stu-id="cea36-104">The **AlternateId** element describes an identifier to convert in a request and the results of a converted identifier in the response.</span></span> 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 <span data-ttu-id="cea36-105">**AlternateIdType**</span><span class="sxs-lookup"><span data-stu-id="cea36-105">**AlternateIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cea36-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cea36-106">Attributes and elements</span></span>

<span data-ttu-id="cea36-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cea36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cea36-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cea36-108">Attributes</span></span>

|<span data-ttu-id="cea36-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="cea36-109">**Attribute**</span></span>|<span data-ttu-id="cea36-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cea36-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cea36-111">Id</span><span class="sxs-lookup"><span data-stu-id="cea36-111">Id</span></span>  <br/> |<span data-ttu-id="cea36-112">Descreve o identificador de origem em uma solicitação de [operação convertid](convertid-operation.md) e descreve o identificador de destino em uma resposta de [operação convertid](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cea36-112">Describes the source identifier in a [ConvertId operation](convertid-operation.md) request and describes the destination identifier in a [ConvertId operation](convertid-operation.md) response.</span></span>  <br/> |
|<span data-ttu-id="cea36-113">Formatar</span><span class="sxs-lookup"><span data-stu-id="cea36-113">Format</span></span>  <br/> |<span data-ttu-id="cea36-114">Descreve o formato de origem em uma solicitação de [operação convertid](convertid-operation.md) e descreve o formato de destino em uma resposta de [operação convertid](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cea36-114">Describes the source format in a [ConvertId operation](convertid-operation.md) request and describes the destination format in a [ConvertId operation](convertid-operation.md) response.</span></span> <span data-ttu-id="cea36-115">O formato de destino é descrito pelo atributo **DestinationFormat** do elemento [convertid](convertid.md) na solicitação.</span><span class="sxs-lookup"><span data-stu-id="cea36-115">The destination format is described by the **DestinationFormat** attribute of the [ConvertId](convertid.md) element in the request.</span></span> <span data-ttu-id="cea36-116">Este atributo é do tipo **idformattype**.</span><span class="sxs-lookup"><span data-stu-id="cea36-116">This attribute is of type **IdFormatType**.</span></span>  <br/> |
|<span data-ttu-id="cea36-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="cea36-117">Mailbox</span></span>  <br/> |<span data-ttu-id="cea36-118">Descreve o endereço SMTP (Simple Mail Transfer Protocol) principal da caixa de correio que contém os identificadores a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="cea36-118">Describes the mailbox primary Simple Mail Transfer Protocol (SMTP) address that contains the identifiers to translate.</span></span>  <br/> |
|<span data-ttu-id="cea36-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="cea36-119">IsArchive</span></span>  <br/> |<span data-ttu-id="cea36-120">Indica se o identificador representa um item ou pasta arquivada.</span><span class="sxs-lookup"><span data-stu-id="cea36-120">Indicates whether the identifier represents an archived item or folder.</span></span> <span data-ttu-id="cea36-121">Um valor **true** indica que o identificador representa um item ou uma pasta arquivada.</span><span class="sxs-lookup"><span data-stu-id="cea36-121">A value of **true** indicates that the identifier represents an archived item or folder.</span></span> <span data-ttu-id="cea36-122">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="cea36-122">This attribute is optional.</span></span>  <br/> |
   
#### <a name="format-attribute-values"></a><span data-ttu-id="cea36-123">Valores de atributo de formato</span><span class="sxs-lookup"><span data-stu-id="cea36-123">Format attribute values</span></span>

|<span data-ttu-id="cea36-124">**Valor**</span><span class="sxs-lookup"><span data-stu-id="cea36-124">**Value**</span></span>|<span data-ttu-id="cea36-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cea36-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cea36-126">EwsLegacyId</span><span class="sxs-lookup"><span data-stu-id="cea36-126">EwsLegacyId</span></span>  <br/> |<span data-ttu-id="cea36-127">Descreve os identificadores produzidos pelos serviços Web do Exchange na versão inicial de lançamento do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="cea36-127">Describes identifiers that are produced by Exchange Web Services in the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="cea36-128">EwsId</span><span class="sxs-lookup"><span data-stu-id="cea36-128">EwsId</span></span>  <br/> |<span data-ttu-id="cea36-129">Descreve os identificadores produzidos pelos serviços Web do Exchange a partir do Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="cea36-129">Describes identifiers that are produced by Exchange Web Services starting with Exchange 2007 SP1.</span></span>  <br/> |
|<span data-ttu-id="cea36-130">EntryId</span><span class="sxs-lookup"><span data-stu-id="cea36-130">EntryId</span></span>  <br/> |<span data-ttu-id="cea36-131">Descreve os identificadores MAPI, como na propriedade **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="cea36-131">Describes MAPI identifiers, as in the **PR_ENTRYID** property.</span></span>  <br/> |
|<span data-ttu-id="cea36-132">HexEntryId</span><span class="sxs-lookup"><span data-stu-id="cea36-132">HexEntryId</span></span>  <br/> |<span data-ttu-id="cea36-133">Descreve uma representação codificada hexadecimal da propriedade **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="cea36-133">Describes a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="cea36-134">Este é o formato de identificadores de eventos de calendário de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="cea36-134">This is the format of availability calendar event identifiers.</span></span>  <br/> |
|<span data-ttu-id="cea36-135">StoreId</span><span class="sxs-lookup"><span data-stu-id="cea36-135">StoreId</span></span>  <br/> |<span data-ttu-id="cea36-136">Descreve os identificadores de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cea36-136">Describes Exchange store identifiers.</span></span>  <br/> |
|<span data-ttu-id="cea36-137">OwaId</span><span class="sxs-lookup"><span data-stu-id="cea36-137">OwaId</span></span>  <br/> |<span data-ttu-id="cea36-138">Descreve um identificador do Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="cea36-138">Describes an Outlook Web App identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cea36-139">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cea36-139">Child elements</span></span>

<span data-ttu-id="cea36-140">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cea36-140">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cea36-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cea36-141">Parent elements</span></span>

|<span data-ttu-id="cea36-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cea36-142">**Element**</span></span>|<span data-ttu-id="cea36-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cea36-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cea36-144">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cea36-144">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="cea36-145">Contém o status e o resultado de uma solicitação de [operação convertid](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cea36-145">Contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="cea36-146">SourceIds</span><span class="sxs-lookup"><span data-stu-id="cea36-146">SourceIds</span></span>](sourceids.md) <br/> |<span data-ttu-id="cea36-147">Contém os identificadores de origem a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="cea36-147">Contains the source identifiers to convert.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cea36-148">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cea36-148">Text value</span></span>

<span data-ttu-id="cea36-149">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cea36-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cea36-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="cea36-150">Remarks</span></span>

<span data-ttu-id="cea36-151">O elemento **alternateid** descreve dois identificadores, o identificador de origem que deve ser convertido na solicitação de [operação convertid](convertid-operation.md) e o identificador convertido no elemento [ConvertIdResponse](convertidresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="cea36-151">The **AlternateId** element describes two identifiers, the source identifier that is to be converted in the [ConvertId operation](convertid-operation.md) request, and the converted identifier in the [ConvertIdResponse](convertidresponse.md) element.</span></span> 
  
<span data-ttu-id="cea36-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cea36-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cea36-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cea36-153">Element information</span></span>

||||
|:-----|:-----|:-----|
|<span data-ttu-id="cea36-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="cea36-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cea36-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cea36-155">Schema Name</span></span>  <br/> |<span data-ttu-id="cea36-156">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cea36-156">Messages schema</span></span>  <br/> |<span data-ttu-id="cea36-157">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cea36-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="cea36-158">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cea36-158">Validation File</span></span>  <br/> |<span data-ttu-id="cea36-159">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cea36-159">Messages.xsd</span></span>  <br/> |<span data-ttu-id="cea36-160">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cea36-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cea36-161">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cea36-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="cea36-162">Falso</span><span class="sxs-lookup"><span data-stu-id="cea36-162">False</span></span>  <br/> |<span data-ttu-id="cea36-163">False</span><span class="sxs-lookup"><span data-stu-id="cea36-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cea36-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="cea36-164">See also</span></span>

- [<span data-ttu-id="cea36-165">Operação convertid</span><span class="sxs-lookup"><span data-stu-id="cea36-165">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="cea36-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cea36-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cea36-167">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="cea36-167">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

