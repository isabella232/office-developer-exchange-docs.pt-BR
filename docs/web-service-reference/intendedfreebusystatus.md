---
title: IntendedFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IntendedFreeBusyStatus
api_type:
- schema
ms.assetid: 0e0fa898-69a4-4c57-8bb2-52f716b5b478
description: O elemento IntendedFreeBusyStatus representa o status desejado para o item de calendário que está associado à solicitação de reunião.
ms.openlocfilehash: 3254becf8c6885f7d6dc401ecf31da149e7de2d4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823945"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="f91ea-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="f91ea-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="f91ea-104">O elemento **IntendedFreeBusyStatus** representa o status desejado para o item de calendário que está associado à solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="f91ea-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="f91ea-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="f91ea-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f91ea-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f91ea-106">Attributes and elements</span></span>

<span data-ttu-id="f91ea-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f91ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f91ea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f91ea-108">Attributes</span></span>

<span data-ttu-id="f91ea-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f91ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f91ea-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f91ea-110">Child elements</span></span>

<span data-ttu-id="f91ea-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f91ea-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f91ea-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f91ea-112">Parent elements</span></span>

|<span data-ttu-id="f91ea-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f91ea-113">**Element**</span></span>|<span data-ttu-id="f91ea-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f91ea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f91ea-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f91ea-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f91ea-116">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f91ea-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f91ea-117">Text value</span><span class="sxs-lookup"><span data-stu-id="f91ea-117">Text value</span></span>

<span data-ttu-id="f91ea-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="f91ea-118">A text value is required.</span></span> <span data-ttu-id="f91ea-119">Estes são os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="f91ea-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="f91ea-120">Disponível</span><span class="sxs-lookup"><span data-stu-id="f91ea-120">Free</span></span>
    
- <span data-ttu-id="f91ea-121">Provisório</span><span class="sxs-lookup"><span data-stu-id="f91ea-121">Tentative</span></span>
    
- <span data-ttu-id="f91ea-122">Ocupado</span><span class="sxs-lookup"><span data-stu-id="f91ea-122">Busy</span></span>
    
- <span data-ttu-id="f91ea-123">AUSÊNCIA TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="f91ea-123">OOF</span></span>
    
- <span data-ttu-id="f91ea-124">NoData</span><span class="sxs-lookup"><span data-stu-id="f91ea-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f91ea-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="f91ea-125">Remarks</span></span>

<span data-ttu-id="f91ea-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f91ea-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f91ea-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f91ea-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f91ea-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="f91ea-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f91ea-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f91ea-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f91ea-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f91ea-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f91ea-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f91ea-131">Validation File</span></span>  <br/> |<span data-ttu-id="f91ea-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f91ea-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f91ea-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f91ea-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f91ea-134">False</span><span class="sxs-lookup"><span data-stu-id="f91ea-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f91ea-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="f91ea-135">See also</span></span>



- [<span data-ttu-id="f91ea-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f91ea-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

