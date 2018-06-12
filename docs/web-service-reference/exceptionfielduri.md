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
description: O elemento ExceptionFieldURI identifica erros específicos em uma solicitação. Esse elemento é usado apenas como parte de uma resposta de erro no nó MessageXml.
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752118"
---
# <a name="exceptionfielduri"></a><span data-ttu-id="a98fe-104">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="a98fe-104">ExceptionFieldURI</span></span>

<span data-ttu-id="a98fe-105">O elemento **ExceptionFieldURI** identifica erros específicos em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a98fe-105">The **ExceptionFieldURI** element identifies particular errors in a request.</span></span> <span data-ttu-id="a98fe-106">Esse elemento é usado apenas como parte de uma resposta de erro no nó [MessageXml](messagexml.md) .</span><span class="sxs-lookup"><span data-stu-id="a98fe-106">This element is only used as part of an error response in the [MessageXml](messagexml.md) node.</span></span> 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 <span data-ttu-id="a98fe-107">**ExceptionPropertyURIType**</span><span class="sxs-lookup"><span data-stu-id="a98fe-107">**ExceptionPropertyURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a98fe-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a98fe-108">Attributes and elements</span></span>

<span data-ttu-id="a98fe-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a98fe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a98fe-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a98fe-110">Attributes</span></span>

|<span data-ttu-id="a98fe-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a98fe-111">**Attribute**</span></span>|<span data-ttu-id="a98fe-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a98fe-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a98fe-113">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="a98fe-113">**FieldURI**</span></span> <br/> |<span data-ttu-id="a98fe-114">Identifica uma propriedade de uma ocorrência de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="a98fe-114">Identifies a property of an occurrence of a recurring item.</span></span> <span data-ttu-id="a98fe-115">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="a98fe-115">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="a98fe-116">Atributo FieldURI</span><span class="sxs-lookup"><span data-stu-id="a98fe-116">FieldURI Attribute</span></span>

|<span data-ttu-id="a98fe-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a98fe-117">**Value**</span></span>|<span data-ttu-id="a98fe-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a98fe-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a98fe-119">Nome do anexo:</span><span class="sxs-lookup"><span data-stu-id="a98fe-119">attachment:Name</span></span>  <br/> |<span data-ttu-id="a98fe-120">Identifica o nome do anexo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-120">Identifies the attachment name as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-121">anexo: ContentType</span><span class="sxs-lookup"><span data-stu-id="a98fe-121">attachment:ContentType</span></span>  <br/> |<span data-ttu-id="a98fe-122">Identifica o tipo de conteúdo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-122">Identifies the content type as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-123">Conteúdo de anexo:</span><span class="sxs-lookup"><span data-stu-id="a98fe-123">attachment:Content</span></span>  <br/> |<span data-ttu-id="a98fe-124">Identifica o conteúdo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-124">Identifies the content as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-125">Recorrência: mês</span><span class="sxs-lookup"><span data-stu-id="a98fe-125">recurrence:Month</span></span>  <br/> |<span data-ttu-id="a98fe-126">Identifica o campo de mês como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-126">Identifies the month field as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-127">Recorrência: DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="a98fe-127">recurrence:DayOfWeekIndex</span></span>  <br/> |<span data-ttu-id="a98fe-128">Identifica o dia do índice de semana como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-128">Identifies the day of week index as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-129">Recorrência: DaysOfWeek</span><span class="sxs-lookup"><span data-stu-id="a98fe-129">recurrence:DaysOfWeek</span></span>  <br/> |<span data-ttu-id="a98fe-130">Identifica a propriedade DaysOfWeek como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-130">Identifies the DaysOfWeek property as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-131">Recorrência: DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="a98fe-131">recurrence:DayOfMonth</span></span>  <br/> |<span data-ttu-id="a98fe-132">Identifica o DayOfMonth como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-132">Identifies the DayOfMonth as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-133">Intervalo de recorrência:</span><span class="sxs-lookup"><span data-stu-id="a98fe-133">recurrence:Interval</span></span>  <br/> |<span data-ttu-id="a98fe-134">Identifica o intervalo como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-134">Identifies the interval as containing an error.</span></span>  <br/> |
|<span data-ttu-id="a98fe-135">Recorrência: NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="a98fe-135">recurrence:NumberOfOccurrences</span></span>  <br/> |<span data-ttu-id="a98fe-136">Identifica o número de ocorrências como contendo um erro.</span><span class="sxs-lookup"><span data-stu-id="a98fe-136">Identifies the number of occurrences as containing an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a98fe-137">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a98fe-137">Child elements</span></span>

<span data-ttu-id="a98fe-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a98fe-138">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a98fe-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a98fe-139">Parent elements</span></span>

|<span data-ttu-id="a98fe-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a98fe-140">**Element**</span></span>|<span data-ttu-id="a98fe-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a98fe-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a98fe-142">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a98fe-142">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a98fe-143">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="a98fe-143">Provides additional error response information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a98fe-144">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a98fe-144">Remarks</span></span>

<span data-ttu-id="a98fe-145">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a98fe-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a98fe-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a98fe-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a98fe-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="a98fe-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a98fe-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a98fe-148">Schema Name</span></span>  <br/> |<span data-ttu-id="a98fe-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a98fe-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="a98fe-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a98fe-150">Validation File</span></span>  <br/> |<span data-ttu-id="a98fe-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a98fe-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a98fe-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a98fe-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="a98fe-153">False</span><span class="sxs-lookup"><span data-stu-id="a98fe-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a98fe-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="a98fe-154">See also</span></span>



- [<span data-ttu-id="a98fe-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a98fe-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

