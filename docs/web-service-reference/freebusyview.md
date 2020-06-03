---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: O elemento FreeBusyView contém informações de disponibilidade para um usuário específico.
ms.openlocfilehash: e5cc3bea6b57d5c400dd9be44bf9f9aaf9e43eb9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456098"
---
# <a name="freebusyview"></a><span data-ttu-id="f2c6e-103">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f2c6e-103">FreeBusyView</span></span>

<span data-ttu-id="f2c6e-104">O elemento **FreeBusyView** contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-104">The **FreeBusyView** element contains availability information for a specific user.</span></span> 
  
[<span data-ttu-id="f2c6e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f2c6e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f2c6e-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="f2c6e-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f2c6e-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f2c6e-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f2c6e-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f2c6e-108">FreeBusyView</span></span>](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 <span data-ttu-id="f2c6e-109">**FreeBusyView**</span><span class="sxs-lookup"><span data-stu-id="f2c6e-109">**FreeBusyView**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2c6e-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f2c6e-110">Attributes and elements</span></span>

<span data-ttu-id="f2c6e-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2c6e-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="f2c6e-112">Attributes</span></span>

<span data-ttu-id="f2c6e-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2c6e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2c6e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f2c6e-114">Child elements</span></span>

|<span data-ttu-id="f2c6e-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f2c6e-115">**Element**</span></span>|<span data-ttu-id="f2c6e-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f2c6e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2c6e-117">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="f2c6e-117">FreeBusyViewType</span></span>](freebusyviewtype.md) <br/> |<span data-ttu-id="f2c6e-118">Representa o tipo de informações de disponibilidade solicitadas retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-118">Represents the type of requested free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="f2c6e-119">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="f2c6e-119">MergedFreeBusy</span></span>](mergedfreebusy.md) <br/> |<span data-ttu-id="f2c6e-120">Contém o fluxo de dados de disponibilidade mesclado.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-120">Contains the merged free/busy stream of data.</span></span>  <br/> |
|[<span data-ttu-id="f2c6e-121">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="f2c6e-121">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="f2c6e-122">Contém um conjunto de ocorrências de item de calendário exclusivo que representam a disponibilidade do usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-122">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> |
|[<span data-ttu-id="f2c6e-123">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="f2c6e-123">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f2c6e-124">Representa as configurações de fuso horário e as horas de trabalho do usuário de caixa de correio solicitado.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-124">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2c6e-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f2c6e-125">Parent elements</span></span>

|<span data-ttu-id="f2c6e-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f2c6e-126">**Element**</span></span>|<span data-ttu-id="f2c6e-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f2c6e-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2c6e-128">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f2c6e-128">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="f2c6e-129">Contém as informações de disponibilidade de um único usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-129">Contains the free/busy information for a single mailbox user.</span></span>  <br/> <span data-ttu-id="f2c6e-130">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f2c6e-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2c6e-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="f2c6e-131">Remarks</span></span>

<span data-ttu-id="f2c6e-132">Todos os elementos filho são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="f2c6e-133">O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="f2c6e-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f2c6e-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2c6e-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f2c6e-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2c6e-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2c6e-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2c6e-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f2c6e-137">Schema Name</span></span>  <br/> |<span data-ttu-id="f2c6e-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f2c6e-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2c6e-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f2c6e-139">Validation File</span></span>  <br/> |<span data-ttu-id="f2c6e-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f2c6e-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2c6e-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f2c6e-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2c6e-142">False</span><span class="sxs-lookup"><span data-stu-id="f2c6e-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2c6e-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="f2c6e-143">See also</span></span>



[<span data-ttu-id="f2c6e-144">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f2c6e-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f2c6e-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f2c6e-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f2c6e-146">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="f2c6e-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

