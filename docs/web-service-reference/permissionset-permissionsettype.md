---
title: PermissionSet (PermissionSettype)
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
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: O elemento PermissionSet contém todas as permissões configuradas para uma pasta.
ms.openlocfilehash: 5639ee8ba64742f39c0274f4e3aaa76d75bea42b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468128"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="4ce18-103">PermissionSet (PermissionSettype)</span><span class="sxs-lookup"><span data-stu-id="4ce18-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="4ce18-104">O elemento **PermissionSet** contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4ce18-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="4ce18-105">**PermissionSettype**</span><span class="sxs-lookup"><span data-stu-id="4ce18-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ce18-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4ce18-106">Attributes and elements</span></span>

<span data-ttu-id="4ce18-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ce18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ce18-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ce18-108">Attributes</span></span>

<span data-ttu-id="4ce18-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ce18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ce18-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ce18-110">Child elements</span></span>

|<span data-ttu-id="4ce18-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ce18-111">**Element**</span></span>|<span data-ttu-id="4ce18-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ce18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ce18-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ce18-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="4ce18-114">Contém a coleção de permissões para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4ce18-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="4ce18-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4ce18-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4ce18-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="4ce18-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="4ce18-117">Contém uma matriz de entradas desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4ce18-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="4ce18-118">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4ce18-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ce18-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ce18-119">Parent elements</span></span>

|<span data-ttu-id="4ce18-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ce18-120">**Element**</span></span>|<span data-ttu-id="4ce18-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ce18-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ce18-122">Folder</span><span class="sxs-lookup"><span data-stu-id="4ce18-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="4ce18-123">Define uma pasta para criar, obter, localizar, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="4ce18-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="4ce18-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="4ce18-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="4ce18-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4ce18-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4ce18-126">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="4ce18-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="4ce18-127">Representa uma pasta de contatos que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4ce18-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="4ce18-128">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="4ce18-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="4ce18-129">Representa uma pasta tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4ce18-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ce18-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="4ce18-130">Remarks</span></span>

<span data-ttu-id="4ce18-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ce18-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="4ce18-132">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4ce18-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="4ce18-133">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="4ce18-133">Version differences</span></span>

<span data-ttu-id="4ce18-134">Para aplicativos direcionados para o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **myproperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4ce18-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="4ce18-135">Para recuperar permissões de pasta, adicione o elemento [PermissionSet (permissionsettype)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="4ce18-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4ce18-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4ce18-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ce18-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ce18-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ce18-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ce18-138">Schema Name</span></span>  <br/> |<span data-ttu-id="4ce18-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4ce18-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ce18-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ce18-140">Validation File</span></span>  <br/> |<span data-ttu-id="4ce18-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4ce18-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ce18-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4ce18-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ce18-143">False</span><span class="sxs-lookup"><span data-stu-id="4ce18-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ce18-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="4ce18-144">See also</span></span>



- [<span data-ttu-id="4ce18-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ce18-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4ce18-146">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="4ce18-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

