---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: O elemento MeetingWorkspaceUrl contém a URL para o espaço de trabalho de reunião que está incluído no item do calendário. Um espaço de trabalho de reunião é um site compartilhado para planejamento da reunião e controle dos resultados.
ms.openlocfilehash: 7d84547eafe4e77fb23a792fbf15633dbf93d775
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824436"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="d0fd6-104">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="d0fd6-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="d0fd6-105">O elemento **MeetingWorkspaceUrl** contém a URL para o espaço de trabalho de reunião que está incluído no item do calendário.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="d0fd6-106">Um espaço de trabalho de reunião é um site compartilhado para planejamento da reunião e controle dos resultados.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="d0fd6-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="d0fd6-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0fd6-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d0fd6-108">Attributes and elements</span></span>

<span data-ttu-id="d0fd6-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0fd6-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d0fd6-110">Attributes</span></span>

<span data-ttu-id="d0fd6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0fd6-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d0fd6-112">Child elements</span></span>

<span data-ttu-id="d0fd6-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0fd6-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d0fd6-114">Parent elements</span></span>

|<span data-ttu-id="d0fd6-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0fd6-115">**Element**</span></span>|<span data-ttu-id="d0fd6-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0fd6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0fd6-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d0fd6-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d0fd6-118">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d0fd6-119">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d0fd6-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d0fd6-120">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0fd6-121">Text value</span><span class="sxs-lookup"><span data-stu-id="d0fd6-121">Text value</span></span>

<span data-ttu-id="d0fd6-122">Se este elemento for usado, será necessário um valor de texto que representa uma URL.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0fd6-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d0fd6-123">Remarks</span></span>

<span data-ttu-id="d0fd6-124">A propriedade MeetingWorkspaceUrl é gravável de leitura para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="d0fd6-125">Ele é somente leitura para solicitações de reunião e itens de calendário dos participantes.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="d0fd6-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d0fd6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0fd6-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d0fd6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0fd6-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0fd6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0fd6-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d0fd6-129">Schema name</span></span>  <br/> |<span data-ttu-id="d0fd6-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d0fd6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0fd6-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d0fd6-131">Validation file</span></span>  <br/> |<span data-ttu-id="d0fd6-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0fd6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0fd6-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d0fd6-133">Can be empty</span></span>  <br/> |<span data-ttu-id="d0fd6-134">False</span><span class="sxs-lookup"><span data-stu-id="d0fd6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0fd6-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="d0fd6-135">See also</span></span>



- [<span data-ttu-id="d0fd6-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0fd6-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

