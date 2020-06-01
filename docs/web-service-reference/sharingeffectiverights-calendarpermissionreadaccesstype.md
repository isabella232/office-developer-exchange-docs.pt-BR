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
description: O elemento SharingEffectiveRights indica as permissões que o usuário tem para os dados do calendário que estão sendo compartilhados.
ms.openlocfilehash: 5581e9cc001608a124ae94e69eba836f6fd98520
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458576"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="14f52-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="14f52-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="14f52-104">O elemento **SharingEffectiveRights** indica as permissões que o usuário tem para os dados do calendário que estão sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="14f52-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="14f52-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="14f52-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14f52-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="14f52-106">Attributes and elements</span></span>

<span data-ttu-id="14f52-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="14f52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14f52-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="14f52-108">Attributes</span></span>

<span data-ttu-id="14f52-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14f52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14f52-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="14f52-110">Child elements</span></span>

<span data-ttu-id="14f52-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="14f52-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14f52-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="14f52-112">Parent elements</span></span>

|<span data-ttu-id="14f52-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="14f52-113">**Element**</span></span>|<span data-ttu-id="14f52-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14f52-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14f52-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="14f52-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="14f52-116">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="14f52-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14f52-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="14f52-117">Text value</span></span>

<span data-ttu-id="14f52-118">A tabela a seguir lista os valores possíveis para o elemento **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="14f52-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="14f52-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="14f52-119">**Value**</span></span>|<span data-ttu-id="14f52-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14f52-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="14f52-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14f52-121">None</span></span>  <br/> |<span data-ttu-id="14f52-122">Indica que o usuário não tem permissão para exibir itens no calendário.</span><span class="sxs-lookup"><span data-stu-id="14f52-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="14f52-123">Somente timeficado</span><span class="sxs-lookup"><span data-stu-id="14f52-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="14f52-124">Indica que o usuário tem permissão para exibir somente o horário disponível/ocupado no calendário.</span><span class="sxs-lookup"><span data-stu-id="14f52-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="14f52-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="14f52-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="14f52-126">Indica que o usuário tem permissão para exibir o horário de disponibilidade no calendário e o assunto e a localização dos compromissos.</span><span class="sxs-lookup"><span data-stu-id="14f52-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="14f52-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="14f52-127">FullDetails</span></span>  <br/> |<span data-ttu-id="14f52-128">Indica que o usuário tem permissão para exibir todos os itens no calendário, incluindo o tempo de disponibilidade e assunto, local e detalhes dos compromissos.</span><span class="sxs-lookup"><span data-stu-id="14f52-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="14f52-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="14f52-129">Remarks</span></span>

<span data-ttu-id="14f52-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="14f52-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14f52-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="14f52-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14f52-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="14f52-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="14f52-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="14f52-133">Schema Name</span></span>  <br/> |<span data-ttu-id="14f52-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="14f52-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="14f52-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="14f52-135">Validation File</span></span>  <br/> |<span data-ttu-id="14f52-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="14f52-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="14f52-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="14f52-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="14f52-138">False</span><span class="sxs-lookup"><span data-stu-id="14f52-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14f52-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="14f52-139">See also</span></span>



- [<span data-ttu-id="14f52-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="14f52-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

