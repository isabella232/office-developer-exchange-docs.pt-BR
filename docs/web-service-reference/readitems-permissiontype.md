---
title: ReadItems (PermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: 0a11a802-28e2-436b-b5a9-30fd064675a6
description: O elemento ReadItems indica se um usuário tem permissão para ler itens em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: af6ef5107b5e4f2b3071c0bc9b4b528efea6dcca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468268"
---
# <a name="readitems-permissiontype"></a><span data-ttu-id="153ed-104">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="153ed-104">ReadItems (PermissionType)</span></span>

<span data-ttu-id="153ed-105">O elemento **ReadItems** indica se um usuário tem permissão para ler itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="153ed-105">The **ReadItems** element indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="153ed-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="153ed-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or FullDetails</ReadItems>
```

 <span data-ttu-id="153ed-107">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="153ed-107">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="153ed-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="153ed-108">Attributes and elements</span></span>

<span data-ttu-id="153ed-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="153ed-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="153ed-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="153ed-110">Attributes</span></span>

<span data-ttu-id="153ed-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="153ed-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="153ed-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="153ed-112">Child elements</span></span>

<span data-ttu-id="153ed-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="153ed-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="153ed-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="153ed-114">Parent elements</span></span>

|<span data-ttu-id="153ed-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="153ed-115">**Element**</span></span>|<span data-ttu-id="153ed-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="153ed-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="153ed-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="153ed-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="153ed-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="153ed-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="153ed-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="153ed-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="153ed-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="153ed-120">Text value</span></span>

<span data-ttu-id="153ed-121">A tabela a seguir lista os valores possíveis para o elemento **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="153ed-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="153ed-122">**Valores de texto do elemento ReadItems**</span><span class="sxs-lookup"><span data-stu-id="153ed-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="153ed-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="153ed-123">**Value**</span></span>|<span data-ttu-id="153ed-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="153ed-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="153ed-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="153ed-125">None</span></span>  <br/> |<span data-ttu-id="153ed-126">Indica que o usuário não tem permissão para ler itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="153ed-126">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="153ed-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="153ed-127">FullDetails</span></span>  <br/> |<span data-ttu-id="153ed-128">Indica que o usuário tem permissão para ler todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="153ed-128">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="153ed-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="153ed-129">Remarks</span></span>

<span data-ttu-id="153ed-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="153ed-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="153ed-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="153ed-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="153ed-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="153ed-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="153ed-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="153ed-133">Schema Name</span></span>  <br/> |<span data-ttu-id="153ed-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="153ed-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="153ed-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="153ed-135">Validation File</span></span>  <br/> |<span data-ttu-id="153ed-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="153ed-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="153ed-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="153ed-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="153ed-138">False</span><span class="sxs-lookup"><span data-stu-id="153ed-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="153ed-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="153ed-139">See also</span></span>



- [<span data-ttu-id="153ed-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="153ed-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="153ed-141">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="153ed-141">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

