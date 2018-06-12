---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: O elemento UnknownEntries contém uma matriz de entradas de permissão desconhecido que não pode ser resolvido em relação ao serviço de diretório do Active Directory. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 306e5f226a56694bb1ff32362f77e7dff80865ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837856"
---
# <a name="unknownentries"></a><span data-ttu-id="07353-104">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="07353-104">UnknownEntries</span></span>

<span data-ttu-id="07353-105">O elemento **UnknownEntries** contém uma matriz de entradas de permissão desconhecido que não pode ser resolvido em relação ao serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="07353-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="07353-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="07353-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="07353-107">**ArrayOfUnknownEntriesType**</span><span class="sxs-lookup"><span data-stu-id="07353-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07353-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="07353-108">Attributes and elements</span></span>

<span data-ttu-id="07353-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="07353-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07353-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="07353-110">Attributes</span></span>

<span data-ttu-id="07353-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="07353-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07353-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="07353-112">Child elements</span></span>

|<span data-ttu-id="07353-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="07353-113">**Element**</span></span>|<span data-ttu-id="07353-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="07353-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07353-115">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="07353-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="07353-116">Representa uma entrada de permissão desconhecido único que não pode ser resolvida em relação ao Active Directory.</span><span class="sxs-lookup"><span data-stu-id="07353-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="07353-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="07353-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07353-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="07353-118">Parent elements</span></span>

|<span data-ttu-id="07353-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="07353-119">**Element**</span></span>|<span data-ttu-id="07353-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="07353-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07353-121">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="07353-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="07353-122">Contém todas as permissões que estão configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="07353-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="07353-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="07353-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="07353-124">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="07353-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="07353-125">Contém todas as permissões que estão configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="07353-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="07353-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="07353-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07353-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="07353-127">Remarks</span></span>

<span data-ttu-id="07353-128">Você pode excluir entradas desconhecidas de uma pasta usando a operação UpdateFolder com o elemento [SetFolderField](setfolderfield.md) .</span><span class="sxs-lookup"><span data-stu-id="07353-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="07353-129">As entradas desconhecidas são excluídas quando você reinicia o PermissionSet usando a opção SetFolderField da operação UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="07353-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="07353-130">Serviços Web do Exchange não oferece suporte a exclusão de entradas individuais.</span><span class="sxs-lookup"><span data-stu-id="07353-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="07353-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="07353-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07353-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="07353-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07353-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="07353-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07353-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="07353-134">Schema Name</span></span>  <br/> |<span data-ttu-id="07353-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="07353-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="07353-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="07353-136">Validation File</span></span>  <br/> |<span data-ttu-id="07353-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07353-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07353-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="07353-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="07353-139">False</span><span class="sxs-lookup"><span data-stu-id="07353-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07353-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="07353-140">See also</span></span>



[<span data-ttu-id="07353-141">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="07353-141">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="07353-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="07353-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="07353-143">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="07353-143">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

