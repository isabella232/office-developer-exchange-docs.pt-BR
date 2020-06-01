---
title: Permissões
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: O elemento Permissions contém a coleção de permissões para uma pasta.
ms.openlocfilehash: b8616cefdb8c453106753fb0788a6c7d6a0ded79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459213"
---
# <a name="permissions"></a><span data-ttu-id="fd360-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd360-103">Permissions</span></span>

<span data-ttu-id="fd360-104">O elemento **Permissions** contém a coleção de permissões para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="fd360-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="fd360-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="fd360-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd360-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fd360-106">Attributes and elements</span></span>

<span data-ttu-id="fd360-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fd360-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd360-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fd360-108">Attributes</span></span>

<span data-ttu-id="fd360-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd360-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd360-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fd360-110">Child elements</span></span>

|<span data-ttu-id="fd360-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fd360-111">**Element**</span></span>|<span data-ttu-id="fd360-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd360-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd360-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="fd360-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="fd360-114">Define o acesso que um representante tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="fd360-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="fd360-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="fd360-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd360-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fd360-116">Parent elements</span></span>

|<span data-ttu-id="fd360-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fd360-117">**Element**</span></span>|<span data-ttu-id="fd360-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd360-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd360-119">PermissionSet (PermissionSettype)</span><span class="sxs-lookup"><span data-stu-id="fd360-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="fd360-120">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="fd360-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="fd360-121">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="fd360-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd360-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="fd360-122">Remarks</span></span>

<span data-ttu-id="fd360-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd360-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="fd360-124">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fd360-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="fd360-125">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="fd360-125">Version differences</span></span>

<span data-ttu-id="fd360-126">Para aplicativos direcionados para o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **myproperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fd360-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="fd360-127">Para recuperar permissões de pasta, adicione o elemento [PermissionSet (permissionsettype)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="fd360-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fd360-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fd360-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd360-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd360-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd360-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fd360-130">Schema Name</span></span>  <br/> |<span data-ttu-id="fd360-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fd360-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd360-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fd360-132">Validation File</span></span>  <br/> |<span data-ttu-id="fd360-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fd360-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd360-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fd360-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd360-135">False</span><span class="sxs-lookup"><span data-stu-id="fd360-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd360-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="fd360-136">See also</span></span>



- [<span data-ttu-id="fd360-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fd360-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fd360-138">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="fd360-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

