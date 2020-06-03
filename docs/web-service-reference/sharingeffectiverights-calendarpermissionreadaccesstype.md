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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458576"
---
# <a name="sharingeffectiverights-calendarpermissionreadaccesstype"></a><span data-ttu-id="765fb-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="765fb-103">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>

<span data-ttu-id="765fb-104">O elemento **SharingEffectiveRights** indica as permissões que o usuário tem para os dados do calendário que estão sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="765fb-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the calendar data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | TimeOnly | TimeAndSubjectAndLocation | FullDetails</SharingEffectiveRights>
```

 <span data-ttu-id="765fb-105">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="765fb-105">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="765fb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="765fb-106">Attributes and elements</span></span>

<span data-ttu-id="765fb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="765fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="765fb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="765fb-108">Attributes</span></span>

<span data-ttu-id="765fb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="765fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="765fb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="765fb-110">Child elements</span></span>

<span data-ttu-id="765fb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="765fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="765fb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="765fb-112">Parent elements</span></span>

|<span data-ttu-id="765fb-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="765fb-113">**Element**</span></span>|<span data-ttu-id="765fb-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="765fb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="765fb-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="765fb-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="765fb-116">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="765fb-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="765fb-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="765fb-117">Text value</span></span>

<span data-ttu-id="765fb-118">A tabela a seguir lista os valores possíveis para o elemento **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="765fb-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
|<span data-ttu-id="765fb-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="765fb-119">**Value**</span></span>|<span data-ttu-id="765fb-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="765fb-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="765fb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="765fb-121">None</span></span>  <br/> |<span data-ttu-id="765fb-122">Indica que o usuário não tem permissão para exibir itens no calendário.</span><span class="sxs-lookup"><span data-stu-id="765fb-122">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="765fb-123">Somente timeficado</span><span class="sxs-lookup"><span data-stu-id="765fb-123">TimeOnly</span></span>  <br/> |<span data-ttu-id="765fb-124">Indica que o usuário tem permissão para exibir somente o horário disponível/ocupado no calendário.</span><span class="sxs-lookup"><span data-stu-id="765fb-124">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="765fb-125">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="765fb-125">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="765fb-126">Indica que o usuário tem permissão para exibir o horário de disponibilidade no calendário e o assunto e a localização dos compromissos.</span><span class="sxs-lookup"><span data-stu-id="765fb-126">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="765fb-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="765fb-127">FullDetails</span></span>  <br/> |<span data-ttu-id="765fb-128">Indica que o usuário tem permissão para exibir todos os itens no calendário, incluindo o tempo de disponibilidade e assunto, local e detalhes dos compromissos.</span><span class="sxs-lookup"><span data-stu-id="765fb-128">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="765fb-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="765fb-129">Remarks</span></span>

<span data-ttu-id="765fb-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="765fb-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="765fb-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="765fb-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="765fb-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="765fb-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="765fb-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="765fb-133">Schema Name</span></span>  <br/> |<span data-ttu-id="765fb-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="765fb-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="765fb-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="765fb-135">Validation File</span></span>  <br/> |<span data-ttu-id="765fb-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="765fb-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="765fb-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="765fb-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="765fb-138">False</span><span class="sxs-lookup"><span data-stu-id="765fb-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="765fb-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="765fb-139">See also</span></span>



- [<span data-ttu-id="765fb-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="765fb-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

