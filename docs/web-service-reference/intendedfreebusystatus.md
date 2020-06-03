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
description: O elemento IntendedFreeBusyStatus representa o status pretendido para o item de calendário que está associado à solicitação de reunião.
ms.openlocfilehash: c5502bcfb308aa2f02a9575ab43f80261b5fa4ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465615"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="3c071-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="3c071-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="3c071-104">O elemento **IntendedFreeBusyStatus** representa o status pretendido para o item de calendário que está associado à solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="3c071-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="3c071-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="3c071-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c071-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3c071-106">Attributes and elements</span></span>

<span data-ttu-id="3c071-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3c071-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c071-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3c071-108">Attributes</span></span>

<span data-ttu-id="3c071-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c071-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c071-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3c071-110">Child elements</span></span>

<span data-ttu-id="3c071-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c071-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c071-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3c071-112">Parent elements</span></span>

|<span data-ttu-id="3c071-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3c071-113">**Element**</span></span>|<span data-ttu-id="3c071-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3c071-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c071-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3c071-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3c071-116">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c071-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c071-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3c071-117">Text value</span></span>

<span data-ttu-id="3c071-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c071-118">A text value is required.</span></span> <span data-ttu-id="3c071-119">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3c071-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="3c071-120">Disponível</span><span class="sxs-lookup"><span data-stu-id="3c071-120">Free</span></span>
    
- <span data-ttu-id="3c071-121">Provisória</span><span class="sxs-lookup"><span data-stu-id="3c071-121">Tentative</span></span>
    
- <span data-ttu-id="3c071-122">Ocupado</span><span class="sxs-lookup"><span data-stu-id="3c071-122">Busy</span></span>
    
- <span data-ttu-id="3c071-123">TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="3c071-123">OOF</span></span>
    
- <span data-ttu-id="3c071-124">NoData</span><span class="sxs-lookup"><span data-stu-id="3c071-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="3c071-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="3c071-125">Remarks</span></span>

<span data-ttu-id="3c071-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3c071-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c071-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3c071-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c071-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c071-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c071-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3c071-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3c071-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3c071-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c071-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3c071-131">Validation File</span></span>  <br/> |<span data-ttu-id="3c071-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3c071-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c071-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3c071-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c071-134">False</span><span class="sxs-lookup"><span data-stu-id="3c071-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c071-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="3c071-135">See also</span></span>



- [<span data-ttu-id="3c071-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3c071-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

