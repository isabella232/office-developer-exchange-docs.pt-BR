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
description: O elemento Properties contém uma lista de uma ou mais propriedades de controle.
ms.openlocfilehash: 007a4dc14c84c47ea7af8ccacc554c134d563e44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465629"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="03e2c-103">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="03e2c-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="03e2c-104">O elemento **Properties** contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="03e2c-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="03e2c-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="03e2c-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="03e2c-106">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="03e2c-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="03e2c-107">**ArrayOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="03e2c-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="03e2c-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="03e2c-108">Attributes and elements</span></span>

<span data-ttu-id="03e2c-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="03e2c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03e2c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="03e2c-110">Attributes</span></span>

<span data-ttu-id="03e2c-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03e2c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03e2c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="03e2c-112">Child elements</span></span>

|<span data-ttu-id="03e2c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="03e2c-113">**Element**</span></span>|<span data-ttu-id="03e2c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="03e2c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03e2c-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="03e2c-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="03e2c-116">Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="03e2c-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="03e2c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="03e2c-117">Parent elements</span></span>

|<span data-ttu-id="03e2c-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="03e2c-118">**Element**</span></span>|<span data-ttu-id="03e2c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="03e2c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03e2c-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="03e2c-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="03e2c-121">Especifica critérios para os tipos de mensagens a serem encontradas.</span><span class="sxs-lookup"><span data-stu-id="03e2c-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="03e2c-122">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="03e2c-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="03e2c-123">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="03e2c-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="03e2c-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="03e2c-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="03e2c-125">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) para recuperar o relatório de acompanhamento de mensagens completo da ID especificada.</span><span class="sxs-lookup"><span data-stu-id="03e2c-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="03e2c-126">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="03e2c-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="03e2c-127">Contém o resultado de uma única solicitação de [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="03e2c-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="03e2c-128">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="03e2c-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="03e2c-129">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="03e2c-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="03e2c-130">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="03e2c-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="03e2c-131">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="03e2c-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="03e2c-132">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="03e2c-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="03e2c-133">Contém um único resultado de mensagem para um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="03e2c-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03e2c-134">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="03e2c-134">Text value</span></span>

<span data-ttu-id="03e2c-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="03e2c-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03e2c-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="03e2c-136">Remarks</span></span>

<span data-ttu-id="03e2c-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="03e2c-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03e2c-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="03e2c-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03e2c-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="03e2c-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03e2c-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="03e2c-140">Schema Name</span></span>  <br/> |<span data-ttu-id="03e2c-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="03e2c-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03e2c-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="03e2c-142">Validation File</span></span>  <br/> |<span data-ttu-id="03e2c-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="03e2c-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03e2c-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="03e2c-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="03e2c-145">False</span><span class="sxs-lookup"><span data-stu-id="03e2c-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03e2c-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="03e2c-146">See also</span></span>

- [<span data-ttu-id="03e2c-147">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="03e2c-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="03e2c-148">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="03e2c-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="03e2c-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03e2c-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

