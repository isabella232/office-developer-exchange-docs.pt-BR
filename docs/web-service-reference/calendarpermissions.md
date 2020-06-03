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
description: O elemento CalendarPermissions contém uma matriz de permissões de calendário para uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: f072339212d0fdff3983fbfb6bc8f53c272350c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529466"
---
# <a name="calendarpermissions"></a><span data-ttu-id="ca939-104">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="ca939-104">CalendarPermissions</span></span>

<span data-ttu-id="ca939-105">O elemento **CalendarPermissions** contém uma matriz de permissões de calendário para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ca939-105">The **CalendarPermissions** element contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="ca939-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ca939-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 <span data-ttu-id="ca939-107">**ArrayOfCalendarPermissionsType**</span><span class="sxs-lookup"><span data-stu-id="ca939-107">**ArrayOfCalendarPermissionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca939-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ca939-108">Attributes and elements</span></span>

<span data-ttu-id="ca939-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ca939-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca939-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ca939-110">Attributes</span></span>

<span data-ttu-id="ca939-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca939-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca939-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ca939-112">Child elements</span></span>

|<span data-ttu-id="ca939-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca939-113">**Element**</span></span>|<span data-ttu-id="ca939-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca939-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca939-115">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="ca939-115">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="ca939-116">Define o acesso que um usuário delegado tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="ca939-116">Defines the access that a delegate user has to a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca939-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ca939-117">Parent elements</span></span>

|<span data-ttu-id="ca939-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca939-118">**Element**</span></span>|<span data-ttu-id="ca939-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca939-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca939-120">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="ca939-120">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="ca939-121">Contém todas as permissões configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="ca939-121">Contains all the configured permissions for a calendar folder.</span></span> <span data-ttu-id="ca939-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ca939-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ca939-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ca939-123">Remarks</span></span>

<span data-ttu-id="ca939-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ca939-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca939-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ca939-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca939-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="ca939-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca939-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ca939-127">Schema Name</span></span>  <br/> |<span data-ttu-id="ca939-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ca939-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca939-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ca939-129">Validation File</span></span>  <br/> |<span data-ttu-id="ca939-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ca939-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca939-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ca939-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca939-132">False</span><span class="sxs-lookup"><span data-stu-id="ca939-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca939-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca939-133">See also</span></span>



- [<span data-ttu-id="ca939-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ca939-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ca939-135">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="ca939-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

