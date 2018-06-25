---
title: Erros
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Errors
api_type:
- schema
ms.assetid: ea37a2b5-e2d1-4089-960f-7014b9535a50
description: O elemento de erros contém um recipiente de propriedades para armazenar os erros são retornados pelo serviço Web.
ms.openlocfilehash: a029492c1e3c11cc31d3501bd4ea0024ef8ecb91
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752101"
---
# <a name="errors"></a><span data-ttu-id="96553-103">Erros</span><span class="sxs-lookup"><span data-stu-id="96553-103">Errors</span></span>

<span data-ttu-id="96553-104">O elemento de **erros** contém um recipiente de propriedades para armazenar os erros são retornados pelo serviço Web.</span><span class="sxs-lookup"><span data-stu-id="96553-104">The **Errors** element contains a property bag to store errors that are returned through the Web service.</span></span> 
  
[<span data-ttu-id="96553-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="96553-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
[<span data-ttu-id="96553-106">Erros</span><span class="sxs-lookup"><span data-stu-id="96553-106">Errors</span></span>](errors-ex15websvcsotherref.md)
  
```xml
<Errors>
   <Properties/>
</Errors>
```

 <span data-ttu-id="96553-107">**ArrayOfArraysOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="96553-107">**ArrayOfArraysOfTrackingPropertiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96553-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="96553-108">Attributes and elements</span></span>

<span data-ttu-id="96553-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96553-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96553-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="96553-110">Attributes</span></span>

<span data-ttu-id="96553-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96553-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96553-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96553-112">Child elements</span></span>

|<span data-ttu-id="96553-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96553-113">**Element**</span></span>|<span data-ttu-id="96553-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96553-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96553-115">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="96553-115">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="96553-116">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="96553-116">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96553-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96553-117">Parent elements</span></span>

|<span data-ttu-id="96553-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96553-118">**Element**</span></span>|<span data-ttu-id="96553-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96553-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96553-120">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="96553-120">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="96553-121">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="96553-121">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="96553-122">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="96553-122">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="96553-123">Contém o resultado de uma única solicitação de [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="96553-123">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96553-124">Text value</span><span class="sxs-lookup"><span data-stu-id="96553-124">Text value</span></span>

<span data-ttu-id="96553-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96553-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96553-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="96553-126">Remarks</span></span>

<span data-ttu-id="96553-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="96553-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96553-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="96553-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96553-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="96553-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96553-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96553-130">Schema Name</span></span>  <br/> |<span data-ttu-id="96553-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="96553-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96553-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96553-132">Validation File</span></span>  <br/> |<span data-ttu-id="96553-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96553-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96553-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96553-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="96553-135">False</span><span class="sxs-lookup"><span data-stu-id="96553-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96553-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="96553-136">See also</span></span>



[<span data-ttu-id="96553-137">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="96553-137">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="96553-138">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="96553-138">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="96553-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96553-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

