---
title: Diagnósticos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: O elemento de diagnóstico fornece informações de tempo e de desempenho que são usadas para relatórios em um DataCenter.
ms.openlocfilehash: 2b9cac54a683967ec274b8681fb9a0c8a844205e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751796"
---
# <a name="diagnostics"></a><span data-ttu-id="075b7-103">Diagnósticos</span><span class="sxs-lookup"><span data-stu-id="075b7-103">Diagnostics</span></span>

<span data-ttu-id="075b7-104">O elemento de **Diagnóstico** fornece informações de tempo e de desempenho que são usadas para relatórios em um DataCenter.</span><span class="sxs-lookup"><span data-stu-id="075b7-104">The **Diagnostics** element provides timing and performance information that is used for reporting in a DataCenter.</span></span> 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 <span data-ttu-id="075b7-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="075b7-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="075b7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="075b7-106">Attributes and elements</span></span>

<span data-ttu-id="075b7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="075b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="075b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="075b7-108">Attributes</span></span>

<span data-ttu-id="075b7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="075b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="075b7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="075b7-110">Child elements</span></span>

|<span data-ttu-id="075b7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="075b7-111">**Element**</span></span>|<span data-ttu-id="075b7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="075b7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="075b7-113">String</span><span class="sxs-lookup"><span data-stu-id="075b7-113">String</span></span>](string.md) <br/> |<span data-ttu-id="075b7-114">Contém uma cadeia de caracteres que é usada pelo itens, contatos, tarefas e conversas.</span><span class="sxs-lookup"><span data-stu-id="075b7-114">Contains a string that is used by items, contacts, tasks, and conversations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="075b7-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="075b7-115">Parent elements</span></span>

|<span data-ttu-id="075b7-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="075b7-116">**Element**</span></span>|<span data-ttu-id="075b7-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="075b7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="075b7-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="075b7-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="075b7-119">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="075b7-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="075b7-120">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="075b7-120">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="075b7-121">Contém a resposta para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="075b7-121">Contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="075b7-122">Text value</span><span class="sxs-lookup"><span data-stu-id="075b7-122">Text value</span></span>

<span data-ttu-id="075b7-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="075b7-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="075b7-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="075b7-124">Remarks</span></span>

<span data-ttu-id="075b7-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="075b7-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="075b7-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="075b7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="075b7-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="075b7-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="075b7-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="075b7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="075b7-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="075b7-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="075b7-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="075b7-130">Validation File</span></span>  <br/> |<span data-ttu-id="075b7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="075b7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="075b7-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="075b7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="075b7-133">False</span><span class="sxs-lookup"><span data-stu-id="075b7-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="075b7-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="075b7-134">See also</span></span>

- [<span data-ttu-id="075b7-135">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="075b7-135">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="075b7-136">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="075b7-136">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="075b7-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="075b7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

