---
title: IsCancelled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsCancelled
api_type:
- schema
ms.assetid: 50c1e97f-2913-47a1-8457-60428a3c5b92
description: O elemento IsCancelled indica se um compromisso ou reunião foi cancelada.
ms.openlocfilehash: 594b8a9ccb535f074a8cf1da060373f640231a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823993"
---
# <a name="iscancelled"></a><span data-ttu-id="3ba05-103">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="3ba05-103">IsCancelled</span></span>

<span data-ttu-id="3ba05-104">O elemento **IsCancelled** indica se um compromisso ou reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="3ba05-104">The **IsCancelled** element indicates whether an appointment or meeting has been canceled.</span></span> 
  
```xml
<IsCancelled/>
```

 <span data-ttu-id="3ba05-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3ba05-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ba05-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3ba05-106">Attributes and elements</span></span>

<span data-ttu-id="3ba05-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3ba05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ba05-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3ba05-108">Attributes</span></span>

<span data-ttu-id="3ba05-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3ba05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ba05-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3ba05-110">Child elements</span></span>

<span data-ttu-id="3ba05-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3ba05-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3ba05-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3ba05-112">Parent elements</span></span>

|<span data-ttu-id="3ba05-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3ba05-113">**Element**</span></span>|<span data-ttu-id="3ba05-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3ba05-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ba05-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3ba05-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3ba05-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ba05-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3ba05-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3ba05-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3ba05-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ba05-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3ba05-119">Text value</span><span class="sxs-lookup"><span data-stu-id="3ba05-119">Text value</span></span>

<span data-ttu-id="3ba05-120">Um valor de texto que representa um valor booleano é necessário se este elemento é incluído.</span><span class="sxs-lookup"><span data-stu-id="3ba05-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="3ba05-121">Um valor **true** indica que o item do calendário foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="3ba05-121">A value of **true** indicates that the calendar item has been canceled.</span></span> <span data-ttu-id="3ba05-122">Um valor **false** indica que um item de calendário não foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="3ba05-122">A value of **false** indicates that a calendar item has not been canceled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3ba05-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="3ba05-123">Remarks</span></span>

<span data-ttu-id="3ba05-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3ba05-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ba05-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3ba05-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ba05-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="3ba05-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ba05-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3ba05-127">Schema name</span></span>  <br/> |<span data-ttu-id="3ba05-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3ba05-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="3ba05-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3ba05-129">Validation file</span></span>  <br/> |<span data-ttu-id="3ba05-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3ba05-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ba05-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3ba05-131">Can be empty</span></span>  <br/> |<span data-ttu-id="3ba05-132">False</span><span class="sxs-lookup"><span data-stu-id="3ba05-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ba05-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="3ba05-133">See also</span></span>



- [<span data-ttu-id="3ba05-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3ba05-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

