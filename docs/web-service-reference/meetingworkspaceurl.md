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
description: O elemento MeetingWorkspaceUrl contém a URL para o espaço de trabalho de reunião que é incluído no item de calendário. Um espaço de trabalho de reunião é um site compartilhado para planejamento da reunião e controle dos resultados.
ms.openlocfilehash: cd4396e590ab1471278bd44b9a4e0009fe326eaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466280"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="03a39-104">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="03a39-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="03a39-105">O elemento **MeetingWorkspaceUrl** contém a URL para o espaço de trabalho de reunião que é incluído no item de calendário.</span><span class="sxs-lookup"><span data-stu-id="03a39-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="03a39-106">Um espaço de trabalho de reunião é um site compartilhado para planejamento da reunião e controle dos resultados.</span><span class="sxs-lookup"><span data-stu-id="03a39-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="03a39-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="03a39-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03a39-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="03a39-108">Attributes and elements</span></span>

<span data-ttu-id="03a39-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="03a39-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03a39-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="03a39-110">Attributes</span></span>

<span data-ttu-id="03a39-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03a39-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03a39-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="03a39-112">Child elements</span></span>

<span data-ttu-id="03a39-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="03a39-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03a39-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="03a39-114">Parent elements</span></span>

|<span data-ttu-id="03a39-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="03a39-115">**Element**</span></span>|<span data-ttu-id="03a39-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="03a39-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03a39-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="03a39-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="03a39-118">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="03a39-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="03a39-119">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="03a39-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="03a39-120">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="03a39-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03a39-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="03a39-121">Text value</span></span>

<span data-ttu-id="03a39-122">Um valor de texto que representa uma URL será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="03a39-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03a39-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="03a39-123">Remarks</span></span>

<span data-ttu-id="03a39-124">A propriedade MeetingWorkspaceUrl é leitura/gravação para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="03a39-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="03a39-125">É somente leitura para solicitações de reunião e itens de calendário dos participantes.</span><span class="sxs-lookup"><span data-stu-id="03a39-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="03a39-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="03a39-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03a39-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="03a39-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03a39-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="03a39-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03a39-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="03a39-129">Schema name</span></span>  <br/> |<span data-ttu-id="03a39-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="03a39-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="03a39-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="03a39-131">Validation file</span></span>  <br/> |<span data-ttu-id="03a39-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="03a39-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03a39-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="03a39-133">Can be empty</span></span>  <br/> |<span data-ttu-id="03a39-134">False</span><span class="sxs-lookup"><span data-stu-id="03a39-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03a39-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="03a39-135">See also</span></span>



- [<span data-ttu-id="03a39-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03a39-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

