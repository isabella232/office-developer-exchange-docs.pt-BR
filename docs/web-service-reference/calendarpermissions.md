---
title: CalendarPermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissions
api_type:
- schema
ms.assetid: 9b659d83-45fb-42a2-b052-5bc4dbe3854d
description: O elemento CalendarPermissions contém uma matriz de permissões de calendário de uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 3dee635e4449cbb3717f5d2fab8838f3e43102a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751363"
---
# <a name="calendarpermissions"></a><span data-ttu-id="32507-104">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="32507-104">CalendarPermissions</span></span>

<span data-ttu-id="32507-105">O elemento **CalendarPermissions** contém uma matriz de permissões de calendário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="32507-105">The **CalendarPermissions** element contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="32507-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="32507-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 <span data-ttu-id="32507-107">**ArrayOfCalendarPermissionsType**</span><span class="sxs-lookup"><span data-stu-id="32507-107">**ArrayOfCalendarPermissionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32507-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="32507-108">Attributes and elements</span></span>

<span data-ttu-id="32507-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="32507-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32507-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="32507-110">Attributes</span></span>

<span data-ttu-id="32507-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32507-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32507-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="32507-112">Child elements</span></span>

|<span data-ttu-id="32507-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="32507-113">**Element**</span></span>|<span data-ttu-id="32507-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="32507-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32507-115">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="32507-115">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="32507-116">Define o acesso que um usuário delegado tem para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="32507-116">Defines the access that a delegate user has to a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32507-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="32507-117">Parent elements</span></span>

|<span data-ttu-id="32507-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="32507-118">**Element**</span></span>|<span data-ttu-id="32507-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="32507-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32507-120">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="32507-120">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="32507-121">Contém todas as permissões configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="32507-121">Contains all the configured permissions for a calendar folder.</span></span> <span data-ttu-id="32507-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="32507-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="32507-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="32507-123">Remarks</span></span>

<span data-ttu-id="32507-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="32507-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32507-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="32507-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32507-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="32507-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32507-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="32507-127">Schema Name</span></span>  <br/> |<span data-ttu-id="32507-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="32507-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="32507-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="32507-129">Validation File</span></span>  <br/> |<span data-ttu-id="32507-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32507-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32507-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="32507-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="32507-132">False</span><span class="sxs-lookup"><span data-stu-id="32507-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32507-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="32507-133">See also</span></span>



- [<span data-ttu-id="32507-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="32507-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="32507-135">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="32507-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

