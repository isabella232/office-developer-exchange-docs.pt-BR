---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: O elemento ExceptionFieldURI identifica erros específicos em uma solicitação. Este elemento é usado apenas como parte de uma resposta de erro no nó MessageXml.
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454341"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="ba67b-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="ba67b-104">ExceptionFieldURI</span></span>

<span data-ttu-id="ba67b-105">O elemento **ExceptionFieldURI** identifica erros específicos em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba67b-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="ba67b-106">Este elemento é usado apenas como parte de uma resposta de erro no nó [MessageXml](messagexml.md) .</span><span class="sxs-lookup"><span data-stu-id="ba67b-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="ba67b-107">**ExceptionPropertyURIType**</span><span class="sxs-lookup"><span data-stu-id="ba67b-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba67b-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ba67b-108">Attributes and elements</span></span>

<span data-ttu-id="ba67b-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ba67b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba67b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ba67b-110">Attributes</span></span>

|<span data-ttu-id="ba67b-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ba67b-111">**Attribute**</span></span>|<span data-ttu-id="ba67b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ba67b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba67b-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="ba67b-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="ba67b-114">Identifica uma propriedade de uma ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="ba67b-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="ba67b-115">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="ba67b-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="ba67b-116">Atributo FieldURI</span><span class="sxs-lookup"><span data-stu-id="ba67b-116">FieldURI Attribute</span></span>

|<span data-ttu-id="ba67b-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ba67b-117">**Value**</span></span>|<span data-ttu-id="ba67b-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ba67b-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba67b-119">Anexo: nome</span><span class="sxs-lookup"><span data-stu-id="ba67b-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="ba67b-120">Identifica o nome do anexo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-121">Anexo: ContentType</span><span class="sxs-lookup"><span data-stu-id="ba67b-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="ba67b-122">Identifica o tipo de conteúdo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-123">Anexo: conteúdo</span><span class="sxs-lookup"><span data-stu-id="ba67b-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="ba67b-124">Identifica o conteúdo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-125">recorrência: mês</span><span class="sxs-lookup"><span data-stu-id="ba67b-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="ba67b-126">Identifica o campo month como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-127">recorrência: DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="ba67b-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="ba67b-128">Identifica o índice de dia da semana como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-129">recorrência: DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="ba67b-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="ba67b-130">Identifica a Propriedade DaysOfWeek como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-131">recorrência: DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="ba67b-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="ba67b-132">Identifica o DayOfMonth como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-133">recorrência: intervalo</span><span class="sxs-lookup"><span data-stu-id="ba67b-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="ba67b-134">Identifica o intervalo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="ba67b-135">recorrência: NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="ba67b-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="ba67b-136">Identifica o número de ocorrências como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ba67b-137">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ba67b-137">Child elements</span></span>

<span data-ttu-id="ba67b-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ba67b-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba67b-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ba67b-139">Parent elements</span></span>

|<span data-ttu-id="ba67b-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ba67b-140">**Element**</span></span>|<span data-ttu-id="ba67b-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ba67b-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba67b-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ba67b-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ba67b-143">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="ba67b-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ba67b-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="ba67b-144">Remarks</span></span>

<span data-ttu-id="ba67b-145">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ba67b-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba67b-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ba67b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba67b-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba67b-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba67b-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ba67b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="ba67b-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ba67b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba67b-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ba67b-150">Validation File</span></span>  <br/> |<span data-ttu-id="ba67b-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ba67b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba67b-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ba67b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba67b-153">False</span><span class="sxs-lookup"><span data-stu-id="ba67b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba67b-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="ba67b-154">See also</span></span>



- [<span data-ttu-id="ba67b-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ba67b-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

