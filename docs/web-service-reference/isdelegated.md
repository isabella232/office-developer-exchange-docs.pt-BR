---
title: IsDelegated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDelegated
api_type:
- schema
ms.assetid: c12907db-be80-4924-9469-8e58612cf42c
description: O elemento IsDelegated indica se uma reunião foi tratada por uma conta que tenha acesso de representante.
ms.openlocfilehash: a6f42a57b2d0fdb760e4c36d3211ba57289a3c7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824005"
---
# <a name="isdelegated"></a><span data-ttu-id="e90d4-103">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="e90d4-103">IsDelegated</span></span>

<span data-ttu-id="e90d4-104">O elemento **IsDelegated** indica se uma reunião foi tratada por uma conta que tenha acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="e90d4-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="e90d4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e90d4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e90d4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e90d4-106">Attributes and elements</span></span>

<span data-ttu-id="e90d4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e90d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e90d4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e90d4-108">Attributes</span></span>

<span data-ttu-id="e90d4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e90d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e90d4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e90d4-110">Child elements</span></span>

<span data-ttu-id="e90d4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e90d4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e90d4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e90d4-112">Parent elements</span></span>

|<span data-ttu-id="e90d4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e90d4-113">**Element**</span></span>|<span data-ttu-id="e90d4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e90d4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e90d4-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e90d4-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e90d4-116">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e90d4-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e90d4-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e90d4-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e90d4-118">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e90d4-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e90d4-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e90d4-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e90d4-120">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e90d4-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e90d4-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e90d4-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e90d4-122">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e90d4-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e90d4-123">Text value</span><span class="sxs-lookup"><span data-stu-id="e90d4-123">Text value</span></span>

<span data-ttu-id="e90d4-124">Um valor de texto de **true** indica que a reunião foi manipulada por uma conta que tenha acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="e90d4-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e90d4-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e90d4-125">Remarks</span></span>

<span data-ttu-id="e90d4-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e90d4-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e90d4-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e90d4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e90d4-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="e90d4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e90d4-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e90d4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e90d4-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e90d4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e90d4-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e90d4-131">Validation File</span></span>  <br/> |<span data-ttu-id="e90d4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e90d4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e90d4-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e90d4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e90d4-134">False</span><span class="sxs-lookup"><span data-stu-id="e90d4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e90d4-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="e90d4-135">See also</span></span>



- [<span data-ttu-id="e90d4-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e90d4-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

