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
description: O elemento ReadItems indica se um usuário tem permissão para ler itens dentro de uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: bf266c77106f25b90ffd174e25fb0c3972ab91cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824961"
---
# <a name="readitems-permissiontype"></a><span data-ttu-id="3980c-104">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="3980c-104">ReadItems (PermissionType)</span></span>

<span data-ttu-id="3980c-105">O elemento **ReadItems** indica se um usuário tem permissão para ler itens dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3980c-105">The **ReadItems** element indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="3980c-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3980c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or FullDetails</ReadItems>
```

 <span data-ttu-id="3980c-107">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="3980c-107">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3980c-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3980c-108">Attributes and elements</span></span>

<span data-ttu-id="3980c-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3980c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3980c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3980c-110">Attributes</span></span>

<span data-ttu-id="3980c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3980c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3980c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3980c-112">Child elements</span></span>

<span data-ttu-id="3980c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3980c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3980c-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3980c-114">Parent elements</span></span>

|<span data-ttu-id="3980c-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3980c-115">**Element**</span></span>|<span data-ttu-id="3980c-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3980c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3980c-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="3980c-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="3980c-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3980c-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="3980c-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="3980c-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3980c-120">Text value</span><span class="sxs-lookup"><span data-stu-id="3980c-120">Text value</span></span>

<span data-ttu-id="3980c-121">A tabela a seguir lista os valores possíveis para o elemento **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="3980c-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="3980c-122">**Valores de texto do elemento ReadItems**</span><span class="sxs-lookup"><span data-stu-id="3980c-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="3980c-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="3980c-123">**Value**</span></span>|<span data-ttu-id="3980c-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3980c-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3980c-125">None</span><span class="sxs-lookup"><span data-stu-id="3980c-125">None</span></span>  <br/> |<span data-ttu-id="3980c-126">Indica que o usuário não tem permissão para ler itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="3980c-126">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="3980c-127">FullDetails</span><span class="sxs-lookup"><span data-stu-id="3980c-127">FullDetails</span></span>  <br/> |<span data-ttu-id="3980c-128">Indica que o usuário tem permissão para ler todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="3980c-128">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3980c-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="3980c-129">Remarks</span></span>

<span data-ttu-id="3980c-130">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3980c-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3980c-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3980c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3980c-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="3980c-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3980c-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3980c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="3980c-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3980c-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="3980c-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3980c-135">Validation File</span></span>  <br/> |<span data-ttu-id="3980c-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3980c-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3980c-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3980c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="3980c-138">False</span><span class="sxs-lookup"><span data-stu-id="3980c-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3980c-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="3980c-139">See also</span></span>



- [<span data-ttu-id="3980c-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3980c-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3980c-141">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="3980c-141">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

