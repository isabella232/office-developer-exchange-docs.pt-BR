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
description: Elemento PermissionSet contém todas as permissões que estão configuradas para uma pasta de calendário.
ms.openlocfilehash: b2e642fd2ee8ded4d0d4c67509a5587f7b1efa8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824728"
---
# <a name="permissionset-calendarpermissionsettype"></a><span data-ttu-id="5b95b-103">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="5b95b-103">PermissionSet (CalendarPermissionSetType)</span></span>

<span data-ttu-id="5b95b-104">Elemento **PermissionSet** contém todas as permissões que estão configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="5b95b-104">The **PermissionSet** element contains all the permissions that are configured for a calendar folder.</span></span> 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="5b95b-105">**CalendarPermissonSetType**</span><span class="sxs-lookup"><span data-stu-id="5b95b-105">**CalendarPermissonSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b95b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5b95b-106">Attributes and elements</span></span>

<span data-ttu-id="5b95b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5b95b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b95b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5b95b-108">Attributes</span></span>

<span data-ttu-id="5b95b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5b95b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b95b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5b95b-110">Child elements</span></span>

|<span data-ttu-id="5b95b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5b95b-111">**Element**</span></span>|<span data-ttu-id="5b95b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5b95b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b95b-113">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="5b95b-113">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="5b95b-114">Contém uma matriz de permissões de calendário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5b95b-114">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="5b95b-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="5b95b-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="5b95b-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="5b95b-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="5b95b-117">Contém uma matriz de entradas de desconhecido que não pode ser resolvido em relação ao serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5b95b-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="5b95b-118">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="5b95b-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b95b-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5b95b-119">Parent elements</span></span>

|<span data-ttu-id="5b95b-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5b95b-120">**Element**</span></span>|<span data-ttu-id="5b95b-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5b95b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b95b-122">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="5b95b-122">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="5b95b-123">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="5b95b-123">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5b95b-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="5b95b-124">Remarks</span></span>

<span data-ttu-id="5b95b-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b95b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="5b95b-126">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5b95b-126">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="5b95b-127">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="5b95b-127">Version differences</span></span>

<span data-ttu-id="5b95b-128">Para aplicativos de destino Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013, permissões de pasta não serão retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **AllProperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5b95b-128">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="5b95b-129">Para recuperar as permissões da pasta, adicione o elemento [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="5b95b-129">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5b95b-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5b95b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b95b-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="5b95b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b95b-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5b95b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5b95b-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5b95b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b95b-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5b95b-134">Validation File</span></span>  <br/> |<span data-ttu-id="5b95b-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5b95b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b95b-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5b95b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b95b-137">False</span><span class="sxs-lookup"><span data-stu-id="5b95b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b95b-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="5b95b-138">See also</span></span>



- [<span data-ttu-id="5b95b-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5b95b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5b95b-140">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="5b95b-140">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

