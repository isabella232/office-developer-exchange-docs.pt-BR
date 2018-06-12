---
title: PermissionSet (PermissionSetType)
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
description: Elemento PermissionSet contém todas as permissões que estão configuradas para uma pasta.
ms.openlocfilehash: 0fa0ac78a0db2bf382ad413cbb8bd072aa88c6fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824732"
---
# <a name="permissionset-permissionsettype"></a><span data-ttu-id="6d275-103">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="6d275-103">PermissionSet (PermissionSetType)</span></span>

<span data-ttu-id="6d275-104">Elemento **PermissionSet** contém todas as permissões que estão configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6d275-104">The **PermissionSet** element contains all the permissions that are configured for a folder.</span></span> 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 <span data-ttu-id="6d275-105">**PermissionSetType**</span><span class="sxs-lookup"><span data-stu-id="6d275-105">**PermissionSetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d275-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6d275-106">Attributes and elements</span></span>

<span data-ttu-id="6d275-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6d275-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d275-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6d275-108">Attributes</span></span>

<span data-ttu-id="6d275-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d275-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d275-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6d275-110">Child elements</span></span>

|<span data-ttu-id="6d275-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d275-111">**Element**</span></span>|<span data-ttu-id="6d275-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d275-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d275-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d275-113">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="6d275-114">Contém o conjunto de permissões para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6d275-114">Contains the collection of permissions for a folder.</span></span> <span data-ttu-id="6d275-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6d275-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="6d275-116">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="6d275-116">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="6d275-117">Contém uma matriz de entradas de desconhecido que não pode ser resolvido em relação ao serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6d275-117">Contains an array of unknown entries that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="6d275-118">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6d275-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d275-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6d275-119">Parent elements</span></span>

|<span data-ttu-id="6d275-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d275-120">**Element**</span></span>|<span data-ttu-id="6d275-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d275-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d275-122">Folder</span><span class="sxs-lookup"><span data-stu-id="6d275-122">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6d275-123">Define uma pasta para criar, obter, encontre, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="6d275-123">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="6d275-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6d275-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6d275-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6d275-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6d275-126">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="6d275-126">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6d275-127">Representa uma pasta de contatos que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6d275-127">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6d275-128">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="6d275-128">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6d275-129">Representa uma pasta de tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6d275-129">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d275-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="6d275-130">Remarks</span></span>

<span data-ttu-id="6d275-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d275-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="6d275-132">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6d275-132">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="6d275-133">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="6d275-133">Version differences</span></span>

<span data-ttu-id="6d275-134">Para aplicativos de destino Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013, permissões de pasta não serão retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **AllProperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6d275-134">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="6d275-135">Para recuperar as permissões da pasta, adicione o elemento [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="6d275-135">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6d275-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6d275-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d275-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d275-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d275-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6d275-138">Schema Name</span></span>  <br/> |<span data-ttu-id="6d275-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6d275-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d275-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6d275-140">Validation File</span></span>  <br/> |<span data-ttu-id="6d275-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d275-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d275-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6d275-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d275-143">False</span><span class="sxs-lookup"><span data-stu-id="6d275-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d275-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="6d275-144">See also</span></span>



- [<span data-ttu-id="6d275-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6d275-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6d275-146">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="6d275-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

