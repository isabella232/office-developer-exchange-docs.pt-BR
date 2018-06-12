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
description: O elemento de permissões contém o conjunto de permissões para uma pasta.
ms.openlocfilehash: 08d015c3b1afb58fce0fb4b99466965cc5c29fc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824727"
---
# <a name="permissions"></a><span data-ttu-id="eb7b4-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb7b4-103">Permissions</span></span>

<span data-ttu-id="eb7b4-104">O elemento de **permissões** contém o conjunto de permissões para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-104">The **Permissions** element contains the collection of permissions for a folder.</span></span> 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 <span data-ttu-id="eb7b4-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="eb7b4-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb7b4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="eb7b4-106">Attributes and elements</span></span>

<span data-ttu-id="eb7b4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb7b4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb7b4-108">Attributes</span></span>

<span data-ttu-id="eb7b4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb7b4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb7b4-110">Child elements</span></span>

|<span data-ttu-id="eb7b4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb7b4-111">**Element**</span></span>|<span data-ttu-id="eb7b4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb7b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb7b4-113">Permissão</span><span class="sxs-lookup"><span data-stu-id="eb7b4-113">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="eb7b4-114">Define o acesso que tem um representante para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-114">Defines the access that a delegate has to a folder.</span></span> <span data-ttu-id="eb7b4-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb7b4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb7b4-116">Parent elements</span></span>

|<span data-ttu-id="eb7b4-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb7b4-117">**Element**</span></span>|<span data-ttu-id="eb7b4-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb7b4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb7b4-119">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="eb7b4-119">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="eb7b4-120">Contém todas as permissões que estão configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-120">Contains all the permissions that are configured for a folder.</span></span> <span data-ttu-id="eb7b4-121">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb7b4-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb7b4-122">Remarks</span></span>

<span data-ttu-id="eb7b4-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb7b4-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="eb7b4-124">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="eb7b4-124">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="eb7b4-125">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="eb7b4-125">Version differences</span></span>

<span data-ttu-id="eb7b4-126">Para aplicativos de destino Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013, permissões de pasta não serão retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **AllProperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="eb7b4-126">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="eb7b4-127">Para recuperar as permissões da pasta, adicione o elemento [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="eb7b4-127">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="eb7b4-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="eb7b4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb7b4-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb7b4-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb7b4-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb7b4-130">Schema Name</span></span>  <br/> |<span data-ttu-id="eb7b4-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eb7b4-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb7b4-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb7b4-132">Validation File</span></span>  <br/> |<span data-ttu-id="eb7b4-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eb7b4-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb7b4-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eb7b4-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb7b4-135">False</span><span class="sxs-lookup"><span data-stu-id="eb7b4-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb7b4-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="eb7b4-136">See also</span></span>



- [<span data-ttu-id="eb7b4-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="eb7b4-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="eb7b4-138">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="eb7b4-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

