---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: O elemento NetShowUrl Especifica a URL de uma reunião online do Microsoft NetShow.
ms.openlocfilehash: 2440e6c1501331d715d0e5ceb31b3b928122f927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824519"
---
# <a name="netshowurl"></a><span data-ttu-id="31997-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="31997-103">NetShowUrl</span></span>

<span data-ttu-id="31997-104">O elemento **NetShowUrl** Especifica a URL de uma reunião online do Microsoft NetShow.</span><span class="sxs-lookup"><span data-stu-id="31997-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="31997-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="31997-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31997-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="31997-106">Attributes and elements</span></span>

<span data-ttu-id="31997-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="31997-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31997-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="31997-108">Attributes</span></span>

<span data-ttu-id="31997-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31997-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31997-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="31997-110">Child elements</span></span>

<span data-ttu-id="31997-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31997-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31997-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="31997-112">Parent elements</span></span>

|<span data-ttu-id="31997-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31997-113">**Element**</span></span>|<span data-ttu-id="31997-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31997-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31997-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="31997-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="31997-116">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="31997-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="31997-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="31997-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="31997-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="31997-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31997-119">Text value</span><span class="sxs-lookup"><span data-stu-id="31997-119">Text value</span></span>

<span data-ttu-id="31997-120">Se este elemento for usado, será necessário um valor de texto que representa uma URL.</span><span class="sxs-lookup"><span data-stu-id="31997-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31997-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="31997-121">Remarks</span></span>

<span data-ttu-id="31997-122">Essa propriedade NetShowUrl é gravável de leitura para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="31997-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="31997-123">Ele é somente leitura para solicitações de reunião e para os participantes.</span><span class="sxs-lookup"><span data-stu-id="31997-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="31997-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="31997-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31997-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="31997-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31997-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="31997-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31997-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="31997-127">Schema name</span></span>  <br/> |<span data-ttu-id="31997-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="31997-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="31997-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="31997-129">Validation file</span></span>  <br/> |<span data-ttu-id="31997-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31997-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31997-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="31997-131">Can be empty</span></span>  <br/> |<span data-ttu-id="31997-132">False</span><span class="sxs-lookup"><span data-stu-id="31997-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31997-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="31997-133">See also</span></span>



- [<span data-ttu-id="31997-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="31997-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

