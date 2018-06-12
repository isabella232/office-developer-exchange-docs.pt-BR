---
title: SharingEffectiveRights (CalendarPermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: b519f642-a9ef-4300-92e6-ed8202855fde
description: O elemento SharingEffectiveRights indica as permissões que o usuário tem para os dados do calendário que está sendo compartilhados.
ms.openlocfilehash: e7d2aa061650c33d27de042ae8a6348f9a7d3430
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825480"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="b45e9-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="b45e9-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="b45e9-104">O elemento **SharingEffectiveRights** indica as permissões que o usuário tem para os dados do calendário que está sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="b45e9-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="b45e9-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="b45e9-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b45e9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b45e9-106">Attributes and elements</span></span>

<span data-ttu-id="b45e9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b45e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b45e9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b45e9-108">Attributes</span></span>

<span data-ttu-id="b45e9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b45e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b45e9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b45e9-110">Child elements</span></span>

<span data-ttu-id="b45e9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b45e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b45e9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b45e9-112">Parent elements</span></span>

|<span data-ttu-id="b45e9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b45e9-113">**Element**</span></span>|<span data-ttu-id="b45e9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b45e9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b45e9-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="b45e9-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="b45e9-116">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="b45e9-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b45e9-117">Text value</span><span class="sxs-lookup"><span data-stu-id="b45e9-117">Text value</span></span>

<span data-ttu-id="b45e9-118">A tabela a seguir lista os valores possíveis para o elemento **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="b45e9-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="b45e9-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b45e9-119">**Value**</span></span>|<span data-ttu-id="b45e9-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b45e9-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b45e9-121">None</span><span class="sxs-lookup"><span data-stu-id="b45e9-121">None</span></span>  <br/> |<span data-ttu-id="b45e9-122">Indica que o usuário não tem permissão para exibir itens do calendário.</span><span class="sxs-lookup"><span data-stu-id="b45e9-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="b45e9-123">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="b45e9-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="b45e9-124">Indica que o usuário tem permissão para exibir o tempo de disponibilidade apenas no calendário.</span><span class="sxs-lookup"><span data-stu-id="b45e9-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="b45e9-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="b45e9-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="b45e9-126">Indica que o usuário tem permissão para exibir o tempo de disponibilidade no calendário e o assunto e o local de compromissos.</span><span class="sxs-lookup"><span data-stu-id="b45e9-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="b45e9-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b45e9-127">FullDetails</span></span>  <br/> |<span data-ttu-id="b45e9-128">Indica que o usuário tem permissão para exibir todos os itens do calendário, incluindo o tempo de livre/ocupado e assunto, local e detalhes dos compromissos.</span><span class="sxs-lookup"><span data-stu-id="b45e9-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b45e9-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="b45e9-129">Remarks</span></span>

<span data-ttu-id="b45e9-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b45e9-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b45e9-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b45e9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b45e9-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="b45e9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b45e9-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b45e9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b45e9-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b45e9-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b45e9-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b45e9-135">Validation File</span></span>  <br/> |<span data-ttu-id="b45e9-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b45e9-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b45e9-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b45e9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="b45e9-138">False</span><span class="sxs-lookup"><span data-stu-id="b45e9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b45e9-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="b45e9-139">See also</span></span>



- [<span data-ttu-id="b45e9-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b45e9-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

