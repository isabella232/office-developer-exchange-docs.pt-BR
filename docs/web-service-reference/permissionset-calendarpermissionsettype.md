---
title: PermissionSet (CalendarPermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: O elemento PermissionSet contém todas as permissões configuradas para uma pasta de calendário.
ms.openlocfilehash: 9564608397ac8a5ab0ddd4508eacd8cad665d76e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458030"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="de74c-103">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="de74c-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="de74c-104">O elemento **PermissionSet** contém todas as permissões configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="de74c-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="de74c-105">**CalendarPermissonSetType**</span><span class="sxs-lookup"><span data-stu-id="de74c-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de74c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="de74c-106">Attributes and elements</span></span>

<span data-ttu-id="de74c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="de74c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de74c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="de74c-108">Attributes</span></span>

<span data-ttu-id="de74c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de74c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de74c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="de74c-110">Child elements</span></span>

|<span data-ttu-id="de74c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de74c-111">**Element**</span></span>|<span data-ttu-id="de74c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de74c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de74c-113">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="de74c-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="de74c-114">Contém uma matriz de permissões de calendário para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="de74c-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="de74c-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="de74c-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="de74c-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="de74c-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="de74c-117">Contém uma matriz de entradas desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de74c-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="de74c-118">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="de74c-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de74c-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="de74c-119">Parent elements</span></span>

|<span data-ttu-id="de74c-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de74c-120">**Element**</span></span>|<span data-ttu-id="de74c-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de74c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de74c-122">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="de74c-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="de74c-123">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="de74c-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="de74c-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="de74c-124">Remarks</span></span>

<span data-ttu-id="de74c-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="de74c-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="de74c-126">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="de74c-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="de74c-127">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="de74c-127">Version differences</span></span>

<span data-ttu-id="de74c-128">Para aplicativos direcionados para o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **myproperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="de74c-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="de74c-129">Para recuperar permissões de pasta, adicione o elemento [PermissionSet (permissionsettype)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="de74c-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="de74c-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="de74c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de74c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="de74c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de74c-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="de74c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="de74c-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="de74c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="de74c-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="de74c-134">Validation File</span></span>  <br/> |<span data-ttu-id="de74c-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="de74c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de74c-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="de74c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="de74c-137">False</span><span class="sxs-lookup"><span data-stu-id="de74c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de74c-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="de74c-138">See also</span></span>



- [<span data-ttu-id="de74c-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de74c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="de74c-140">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="de74c-140">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

