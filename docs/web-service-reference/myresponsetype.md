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
description: O elemento MyResponseType contém o status ou a resposta a um item de calendário.
ms.openlocfilehash: 640b0595ac039cc3c119aa52aa6e791e5b695e87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466623"
---
# <a name="myresponsetype"></a><span data-ttu-id="b867c-103">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="b867c-103">MyResponseType</span></span>

<span data-ttu-id="b867c-104">O elemento **MyResponseType** contém o status ou a resposta a um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="b867c-104">The **MyResponseType** element contains the status of or response to a calendar item.</span></span> 
  
```xml
<MyResponseType/>
```

 <span data-ttu-id="b867c-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="b867c-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b867c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b867c-106">Attributes and elements</span></span>

<span data-ttu-id="b867c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b867c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b867c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b867c-108">Attributes</span></span>

<span data-ttu-id="b867c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b867c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b867c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b867c-110">Child elements</span></span>

<span data-ttu-id="b867c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b867c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b867c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b867c-112">Parent elements</span></span>

|<span data-ttu-id="b867c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b867c-113">**Element**</span></span>|<span data-ttu-id="b867c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b867c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b867c-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b867c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b867c-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b867c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b867c-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b867c-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b867c-118">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b867c-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b867c-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b867c-119">Text value</span></span>

<span data-ttu-id="b867c-120">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b867c-120">A text value is required.</span></span> <span data-ttu-id="b867c-121">Estes são os valores de texto possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="b867c-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="b867c-122">Desconhecido</span><span class="sxs-lookup"><span data-stu-id="b867c-122">Unknown</span></span>
    
- <span data-ttu-id="b867c-123">Organizador</span><span class="sxs-lookup"><span data-stu-id="b867c-123">Organizer</span></span>
    
- <span data-ttu-id="b867c-124">Provisória</span><span class="sxs-lookup"><span data-stu-id="b867c-124">Tentative</span></span>
    
- <span data-ttu-id="b867c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b867c-125">Accept</span></span>
    
- <span data-ttu-id="b867c-126">Aceito</span><span class="sxs-lookup"><span data-stu-id="b867c-126">Decline</span></span>
    
- <span data-ttu-id="b867c-127">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="b867c-127">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b867c-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="b867c-128">Remarks</span></span>

<span data-ttu-id="b867c-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b867c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b867c-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b867c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b867c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="b867c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b867c-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b867c-132">Schema name</span></span>  <br/> |<span data-ttu-id="b867c-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b867c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="b867c-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b867c-134">Validation file</span></span>  <br/> |<span data-ttu-id="b867c-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b867c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b867c-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b867c-136">Can be empty</span></span>  <br/> |<span data-ttu-id="b867c-137">False</span><span class="sxs-lookup"><span data-stu-id="b867c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b867c-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="b867c-138">See also</span></span>



- [<span data-ttu-id="b867c-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b867c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

