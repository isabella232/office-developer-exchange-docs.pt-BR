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
description: O elemento EditItems indica quais itens em uma pasta um usuário tem permissão para editar. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 0c3800b4d242dccb7455e0d0dea74e766db22854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459248"
---
# <a name="edititems"></a><span data-ttu-id="18a40-104">EditItems</span><span class="sxs-lookup"><span data-stu-id="18a40-104">EditItems</span></span>

<span data-ttu-id="18a40-105">O elemento **EditItems** indica quais itens em uma pasta um usuário tem permissão para editar.</span><span class="sxs-lookup"><span data-stu-id="18a40-105">The **EditItems** element indicates which items in a folder a user has permission to edit.</span></span> <span data-ttu-id="18a40-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="18a40-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 <span data-ttu-id="18a40-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="18a40-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18a40-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="18a40-108">Attributes and elements</span></span>

<span data-ttu-id="18a40-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="18a40-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18a40-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="18a40-110">Attributes</span></span>

<span data-ttu-id="18a40-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a40-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18a40-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="18a40-112">Child elements</span></span>

<span data-ttu-id="18a40-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="18a40-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18a40-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="18a40-114">Parent elements</span></span>

|<span data-ttu-id="18a40-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18a40-115">**Element**</span></span>|<span data-ttu-id="18a40-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18a40-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18a40-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="18a40-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="18a40-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="18a40-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="18a40-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="18a40-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="18a40-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="18a40-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="18a40-121">Define o acesso que um usuário tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="18a40-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="18a40-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="18a40-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18a40-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="18a40-123">Text value</span></span>

<span data-ttu-id="18a40-124">A tabela a seguir lista os valores possíveis para o elemento **EditItems** .</span><span class="sxs-lookup"><span data-stu-id="18a40-124">The following table lists the possible values for the **EditItems** element.</span></span> 
  
<span data-ttu-id="18a40-125">**Valores de texto do elemento EditItems**</span><span class="sxs-lookup"><span data-stu-id="18a40-125">**EditItems element text values**</span></span>

|<span data-ttu-id="18a40-126">**Valor**</span><span class="sxs-lookup"><span data-stu-id="18a40-126">**Value**</span></span>|<span data-ttu-id="18a40-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18a40-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18a40-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a40-128">None</span></span>  <br/> |<span data-ttu-id="18a40-129">Indica que o usuário não tem permissão para editar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="18a40-129">Indicates that the user does not have permission to edit items in the folder.</span></span>  <br/> |
|<span data-ttu-id="18a40-130">Possuir</span><span class="sxs-lookup"><span data-stu-id="18a40-130">Owned</span></span>  <br/> |<span data-ttu-id="18a40-131">Indica que o usuário tem permissão para editar os itens que o usuário possui na pasta.</span><span class="sxs-lookup"><span data-stu-id="18a40-131">Indicates that the user has permission to edit the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="18a40-132">Todos</span><span class="sxs-lookup"><span data-stu-id="18a40-132">All</span></span>  <br/> |<span data-ttu-id="18a40-133">Indica que o usuário tem permissão para editar todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="18a40-133">Indicates that the user has permission to edit all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18a40-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="18a40-134">Remarks</span></span>

<span data-ttu-id="18a40-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="18a40-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18a40-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="18a40-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18a40-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="18a40-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18a40-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="18a40-138">Schema Name</span></span>  <br/> |<span data-ttu-id="18a40-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="18a40-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="18a40-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="18a40-140">Validation File</span></span>  <br/> |<span data-ttu-id="18a40-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="18a40-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18a40-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="18a40-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="18a40-143">False</span><span class="sxs-lookup"><span data-stu-id="18a40-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18a40-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="18a40-144">See also</span></span>

- [<span data-ttu-id="18a40-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="18a40-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="18a40-146">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="18a40-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

