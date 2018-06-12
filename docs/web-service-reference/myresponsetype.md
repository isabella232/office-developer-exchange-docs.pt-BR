---
title: MyResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MyResponseType
api_type:
- schema
ms.assetid: 9741b71d-a310-4520-81d5-3787a1ee630f
description: O elemento MyResponseType contém o status da ou uma resposta a um item de calendário.
ms.openlocfilehash: 3be900ed6d2932699e3e83a0bca2918c016eb689
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824497"
---
# <a name="myresponsetype"></a><span data-ttu-id="be80c-103">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="be80c-103">MyResponseType</span></span>

<span data-ttu-id="be80c-104">O elemento **MyResponseType** contém o status da ou uma resposta a um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="be80c-104">The **MyResponseType** element contains the status of or response to a calendar item.</span></span> 
  
```xml
<MyResponseType/>
```

 <span data-ttu-id="be80c-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="be80c-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be80c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="be80c-106">Attributes and elements</span></span>

<span data-ttu-id="be80c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="be80c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be80c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="be80c-108">Attributes</span></span>

<span data-ttu-id="be80c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be80c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be80c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="be80c-110">Child elements</span></span>

<span data-ttu-id="be80c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be80c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be80c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="be80c-112">Parent elements</span></span>

|<span data-ttu-id="be80c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="be80c-113">**Element**</span></span>|<span data-ttu-id="be80c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be80c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be80c-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="be80c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="be80c-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be80c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="be80c-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="be80c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="be80c-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be80c-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be80c-119">Text value</span><span class="sxs-lookup"><span data-stu-id="be80c-119">Text value</span></span>

<span data-ttu-id="be80c-120">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="be80c-120">A text value is required.</span></span> <span data-ttu-id="be80c-121">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="be80c-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="be80c-122">Desconhecida</span><span class="sxs-lookup"><span data-stu-id="be80c-122">Unknown</span></span>
    
- <span data-ttu-id="be80c-123">Organizador</span><span class="sxs-lookup"><span data-stu-id="be80c-123">Organizer</span></span>
    
- <span data-ttu-id="be80c-124">Provisório</span><span class="sxs-lookup"><span data-stu-id="be80c-124">Tentative</span></span>
    
- <span data-ttu-id="be80c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be80c-125">Accept</span></span>
    
- <span data-ttu-id="be80c-126">Recusar</span><span class="sxs-lookup"><span data-stu-id="be80c-126">Decline</span></span>
    
- <span data-ttu-id="be80c-127">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="be80c-127">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="be80c-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="be80c-128">Remarks</span></span>

<span data-ttu-id="be80c-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="be80c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be80c-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="be80c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be80c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="be80c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be80c-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="be80c-132">Schema name</span></span>  <br/> |<span data-ttu-id="be80c-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="be80c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="be80c-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="be80c-134">Validation file</span></span>  <br/> |<span data-ttu-id="be80c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="be80c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be80c-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="be80c-136">Can be empty</span></span>  <br/> |<span data-ttu-id="be80c-137">False</span><span class="sxs-lookup"><span data-stu-id="be80c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be80c-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="be80c-138">See also</span></span>



- [<span data-ttu-id="be80c-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be80c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

