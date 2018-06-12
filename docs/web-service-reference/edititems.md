---
title: EditItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EditItems
api_type:
- schema
ms.assetid: 1cb14493-c999-4d66-b82c-ecb410dc1c00
description: O elemento EditItems indica quais itens em uma pasta, um usuário tem permissão para editar. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: bbcc103f171cca7c72967796284c6016d8e284e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751968"
---
# <a name="edititems"></a><span data-ttu-id="7ab28-104">EditItems</span><span class="sxs-lookup"><span data-stu-id="7ab28-104">EditItems</span></span>

<span data-ttu-id="7ab28-105">O elemento **EditItems** indica quais itens em uma pasta, um usuário tem permissão para editar.</span><span class="sxs-lookup"><span data-stu-id="7ab28-105">The **EditItems** element indicates which items in a folder a user has permission to edit.</span></span> <span data-ttu-id="7ab28-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7ab28-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 <span data-ttu-id="7ab28-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="7ab28-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ab28-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7ab28-108">Attributes and elements</span></span>

<span data-ttu-id="7ab28-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7ab28-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ab28-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7ab28-110">Attributes</span></span>

<span data-ttu-id="7ab28-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7ab28-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ab28-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7ab28-112">Child elements</span></span>

<span data-ttu-id="7ab28-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7ab28-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ab28-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7ab28-114">Parent elements</span></span>

|<span data-ttu-id="7ab28-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ab28-115">**Element**</span></span>|<span data-ttu-id="7ab28-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ab28-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ab28-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="7ab28-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="7ab28-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="7ab28-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="7ab28-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="7ab28-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="7ab28-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="7ab28-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="7ab28-121">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="7ab28-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="7ab28-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="7ab28-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ab28-123">Text value</span><span class="sxs-lookup"><span data-stu-id="7ab28-123">Text value</span></span>

<span data-ttu-id="7ab28-124">A tabela a seguir lista os valores possíveis para o elemento **EditItems** .</span><span class="sxs-lookup"><span data-stu-id="7ab28-124">The following table lists the possible values for the **EditItems** element.</span></span> 
  
<span data-ttu-id="7ab28-125">**Valores de texto do elemento EditItems**</span><span class="sxs-lookup"><span data-stu-id="7ab28-125">**EditItems element text values**</span></span>

|<span data-ttu-id="7ab28-126">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7ab28-126">**Value**</span></span>|<span data-ttu-id="7ab28-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ab28-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ab28-128">None</span><span class="sxs-lookup"><span data-stu-id="7ab28-128">None</span></span>  <br/> |<span data-ttu-id="7ab28-129">Indica que o usuário não tem permissão para editar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="7ab28-129">Indicates that the user does not have permission to edit items in the folder.</span></span>  <br/> |
|<span data-ttu-id="7ab28-130">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="7ab28-130">Owned</span></span>  <br/> |<span data-ttu-id="7ab28-131">Indica que o usuário tem permissão para editar os itens pertencentes ao usuário na pasta.</span><span class="sxs-lookup"><span data-stu-id="7ab28-131">Indicates that the user has permission to edit the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="7ab28-132">Todos</span><span class="sxs-lookup"><span data-stu-id="7ab28-132">All</span></span>  <br/> |<span data-ttu-id="7ab28-133">Indica que o usuário tem permissão para editar todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="7ab28-133">Indicates that the user has permission to edit all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ab28-134">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7ab28-134">Remarks</span></span>

<span data-ttu-id="7ab28-135">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="7ab28-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ab28-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7ab28-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ab28-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ab28-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ab28-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7ab28-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7ab28-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7ab28-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ab28-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7ab28-140">Validation File</span></span>  <br/> |<span data-ttu-id="7ab28-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ab28-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ab28-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7ab28-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7ab28-143">False</span><span class="sxs-lookup"><span data-stu-id="7ab28-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ab28-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="7ab28-144">See also</span></span>

- [<span data-ttu-id="7ab28-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ab28-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="7ab28-146">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="7ab28-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

