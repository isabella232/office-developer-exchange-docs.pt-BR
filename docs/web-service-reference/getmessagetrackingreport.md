---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: O elemento GetMessageTrackingReport contém a solicitação para a operação GetMessageTrackingReport recuperar o relatório completo de controle de mensagens para a ID especificada.
ms.openlocfilehash: 30596acd209580147e0f03e12a7868502159b29c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44466574"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="1cab8-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1cab8-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="1cab8-104">O elemento **GetMessageTrackingReport** contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar o relatório completo de controle de mensagens para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="1cab8-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 <span data-ttu-id="1cab8-105">**GetMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="1cab8-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cab8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1cab8-106">Attributes and elements</span></span>

<span data-ttu-id="1cab8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1cab8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cab8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1cab8-108">Attributes</span></span>

<span data-ttu-id="1cab8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cab8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cab8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1cab8-110">Child elements</span></span>

|<span data-ttu-id="1cab8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1cab8-111">**Element**</span></span>|<span data-ttu-id="1cab8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1cab8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cab8-113">Escopo (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="1cab8-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="1cab8-114">Especifica onde executar a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="1cab8-114">Specifies where to perform the search.</span></span> <span data-ttu-id="1cab8-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cab8-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1cab8-116">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="1cab8-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="1cab8-117">Especifica o tipo de relatório de controle a ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="1cab8-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="1cab8-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cab8-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1cab8-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="1cab8-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="1cab8-120">Especifica um endereço de destinatário a ser usado com o relatório de acompanhamento especificado.</span><span class="sxs-lookup"><span data-stu-id="1cab8-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="1cab8-121">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1cab8-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1cab8-122">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="1cab8-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="1cab8-123">Especifica uma cadeia de caracteres de identidade obtida da operação **FindMessageTrackingReport** .</span><span class="sxs-lookup"><span data-stu-id="1cab8-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="1cab8-124">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cab8-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1cab8-125">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="1cab8-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="1cab8-126">Especifica que a pessoa que está executando a tarefa tem uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="1cab8-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="1cab8-127">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1cab8-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1cab8-128">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="1cab8-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="1cab8-129">Especifica as informações de tempo e desempenho que serão usadas para derivar o relatório de controle.</span><span class="sxs-lookup"><span data-stu-id="1cab8-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="1cab8-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1cab8-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1cab8-131">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="1cab8-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="1cab8-132">Especifica uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="1cab8-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="1cab8-133">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1cab8-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cab8-134">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1cab8-134">Parent elements</span></span>

<span data-ttu-id="1cab8-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cab8-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1cab8-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="1cab8-136">Remarks</span></span>

<span data-ttu-id="1cab8-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1cab8-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cab8-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1cab8-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cab8-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="1cab8-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cab8-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1cab8-140">Schema Name</span></span>  <br/> |<span data-ttu-id="1cab8-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1cab8-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1cab8-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1cab8-142">Validation File</span></span>  <br/> |<span data-ttu-id="1cab8-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cab8-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cab8-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1cab8-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cab8-145">False</span><span class="sxs-lookup"><span data-stu-id="1cab8-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cab8-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="1cab8-146">See also</span></span>



[<span data-ttu-id="1cab8-147">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1cab8-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="1cab8-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1cab8-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

