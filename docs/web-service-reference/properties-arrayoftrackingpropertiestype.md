---
title: Propriedades (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: O elemento de propriedades contém uma lista de uma ou mais propriedades de controle.
ms.openlocfilehash: 079d2d2c101fdeb7f26d65798048c3c6c59f3e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824897"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="66b8f-103">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="66b8f-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="66b8f-104">O elemento de **Propriedades** contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="66b8f-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="66b8f-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="66b8f-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="66b8f-106">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="66b8f-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="66b8f-107">**ArrayOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="66b8f-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="66b8f-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="66b8f-108">Attributes and elements</span></span>

<span data-ttu-id="66b8f-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="66b8f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66b8f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="66b8f-110">Attributes</span></span>

<span data-ttu-id="66b8f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="66b8f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66b8f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="66b8f-112">Child elements</span></span>

|<span data-ttu-id="66b8f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66b8f-113">**Element**</span></span>|<span data-ttu-id="66b8f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66b8f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66b8f-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="66b8f-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="66b8f-116">Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de acompanhamento de mensagens.</span><span class="sxs-lookup"><span data-stu-id="66b8f-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66b8f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="66b8f-117">Parent elements</span></span>

|<span data-ttu-id="66b8f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66b8f-118">**Element**</span></span>|<span data-ttu-id="66b8f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66b8f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66b8f-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="66b8f-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="66b8f-121">Especifica os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="66b8f-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="66b8f-122">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="66b8f-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="66b8f-123">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="66b8f-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="66b8f-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="66b8f-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="66b8f-125">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="66b8f-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="66b8f-126">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="66b8f-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="66b8f-127">Contém o resultado de uma única solicitação de [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="66b8f-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="66b8f-128">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="66b8f-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="66b8f-129">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="66b8f-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="66b8f-130">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="66b8f-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="66b8f-131">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="66b8f-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="66b8f-132">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="66b8f-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="66b8f-133">Contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="66b8f-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66b8f-134">Text value</span><span class="sxs-lookup"><span data-stu-id="66b8f-134">Text value</span></span>

<span data-ttu-id="66b8f-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="66b8f-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66b8f-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="66b8f-136">Remarks</span></span>

<span data-ttu-id="66b8f-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="66b8f-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66b8f-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="66b8f-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66b8f-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="66b8f-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66b8f-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="66b8f-140">Schema Name</span></span>  <br/> |<span data-ttu-id="66b8f-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="66b8f-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66b8f-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="66b8f-142">Validation File</span></span>  <br/> |<span data-ttu-id="66b8f-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66b8f-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66b8f-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="66b8f-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="66b8f-145">False</span><span class="sxs-lookup"><span data-stu-id="66b8f-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66b8f-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="66b8f-146">See also</span></span>

- [<span data-ttu-id="66b8f-147">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="66b8f-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="66b8f-148">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="66b8f-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="66b8f-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66b8f-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

