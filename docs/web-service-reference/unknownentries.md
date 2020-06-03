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
description: O elemento UnknownEntries contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 68cb2518b895ca0a74e6b9ed649ee92b7502ab05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459416"
---
# <a name="unknownentries"></a><span data-ttu-id="2f62a-104">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="2f62a-104">UnknownEntries</span></span>

<span data-ttu-id="2f62a-105">O elemento **UnknownEntries** contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f62a-105">The **UnknownEntries** element contains an array of unknown permission entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="2f62a-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2f62a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 <span data-ttu-id="2f62a-107">**ArrayOfUnknownEntriesType**</span><span class="sxs-lookup"><span data-stu-id="2f62a-107">**ArrayOfUnknownEntriesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f62a-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2f62a-108">Attributes and elements</span></span>

<span data-ttu-id="2f62a-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2f62a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f62a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="2f62a-110">Attributes</span></span>

<span data-ttu-id="2f62a-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f62a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f62a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2f62a-112">Child elements</span></span>

|<span data-ttu-id="2f62a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2f62a-113">**Element**</span></span>|<span data-ttu-id="2f62a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2f62a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f62a-115">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="2f62a-115">UnknownEntry</span></span>](unknownentry.md) <br/> |<span data-ttu-id="2f62a-116">Representa uma única entrada de permissão desconhecida que não pode ser resolvida no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f62a-116">Represents a single unknown permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="2f62a-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f62a-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f62a-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2f62a-118">Parent elements</span></span>

|<span data-ttu-id="2f62a-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2f62a-119">**Element**</span></span>|<span data-ttu-id="2f62a-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2f62a-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f62a-121">PermissionSet (PermissionSettype)</span><span class="sxs-lookup"><span data-stu-id="2f62a-121">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="2f62a-122">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="2f62a-122">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="2f62a-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f62a-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2f62a-124">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="2f62a-124">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="2f62a-125">Contém todas as permissões configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="2f62a-125">Contains all the permissions that are configured for a calendar folder.</span></span> <span data-ttu-id="2f62a-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="2f62a-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2f62a-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="2f62a-127">Remarks</span></span>

<span data-ttu-id="2f62a-128">Você pode excluir entradas desconhecidas de uma pasta usando a operação UpdateFolder com o elemento [Setfolderfield](setfolderfield.md) .</span><span class="sxs-lookup"><span data-stu-id="2f62a-128">You can delete unknown entries from a folder by using the UpdateFolder operation with the [SetFolderField](setfolderfield.md) element.</span></span> <span data-ttu-id="2f62a-129">As entradas desconhecidas são excluídas quando você redefine o PermissionSet usando a opção setfolderfield da operação UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="2f62a-129">The unknown entries are deleted when you reset the PermissionSet by using the SetFolderField option of the UpdateFolder operation.</span></span> <span data-ttu-id="2f62a-130">Os serviços Web do Exchange não oferecem suporte à exclusão de entradas individuais.</span><span class="sxs-lookup"><span data-stu-id="2f62a-130">Exchange Web Services does not support the deletion of individual entries.</span></span> 
  
<span data-ttu-id="2f62a-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2f62a-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f62a-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2f62a-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f62a-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="2f62a-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f62a-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2f62a-134">Schema Name</span></span>  <br/> |<span data-ttu-id="2f62a-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2f62a-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f62a-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2f62a-136">Validation File</span></span>  <br/> |<span data-ttu-id="2f62a-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2f62a-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f62a-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2f62a-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f62a-139">False</span><span class="sxs-lookup"><span data-stu-id="2f62a-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f62a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="2f62a-140">See also</span></span>



[<span data-ttu-id="2f62a-141">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="2f62a-141">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="2f62a-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2f62a-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2f62a-143">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="2f62a-143">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

