---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: O elemento DeleteItems indica quais itens em uma pasta um usuário tem permissão para excluir. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a0bbefc8b021d047bb2e001669c3e92a6e2536ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454404"
---
# <a name="deleteitems"></a><span data-ttu-id="b8a91-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="b8a91-104">DeleteItems</span></span>

<span data-ttu-id="b8a91-105">O elemento **DeleteItems** indica quais itens em uma pasta um usuário tem permissão para excluir.</span><span class="sxs-lookup"><span data-stu-id="b8a91-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="b8a91-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b8a91-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="b8a91-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="b8a91-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8a91-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b8a91-108">Attributes and elements</span></span>

<span data-ttu-id="b8a91-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b8a91-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8a91-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b8a91-110">Attributes</span></span>

<span data-ttu-id="b8a91-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8a91-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8a91-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b8a91-112">Child elements</span></span>

<span data-ttu-id="b8a91-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8a91-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8a91-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b8a91-114">Parent elements</span></span>

|<span data-ttu-id="b8a91-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8a91-115">**Element**</span></span>|<span data-ttu-id="b8a91-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8a91-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8a91-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="b8a91-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="b8a91-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="b8a91-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="b8a91-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="b8a91-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b8a91-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="b8a91-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="b8a91-121">Define o acesso que um usuário tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="b8a91-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="b8a91-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="b8a91-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8a91-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b8a91-123">Text value</span></span>

<span data-ttu-id="b8a91-124">A tabela a seguir lista os valores possíveis para o elemento **DeleteItems** .</span><span class="sxs-lookup"><span data-stu-id="b8a91-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="b8a91-125">**Valores de texto do elemento DeleteItems**</span><span class="sxs-lookup"><span data-stu-id="b8a91-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="b8a91-126">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b8a91-126">**Value**</span></span>|<span data-ttu-id="b8a91-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8a91-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b8a91-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8a91-128">None</span></span>  <br/> |<span data-ttu-id="b8a91-129">Indica que o usuário não tem permissão para excluir itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="b8a91-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="b8a91-130">Possuir</span><span class="sxs-lookup"><span data-stu-id="b8a91-130">Owned</span></span>  <br/> |<span data-ttu-id="b8a91-131">Indica que o usuário tem permissão para excluir os itens que o usuário possui na pasta.</span><span class="sxs-lookup"><span data-stu-id="b8a91-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="b8a91-132">Todos</span><span class="sxs-lookup"><span data-stu-id="b8a91-132">All</span></span>  <br/> |<span data-ttu-id="b8a91-133">Indica que o usuário tem permissão para excluir todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="b8a91-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8a91-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="b8a91-134">Remarks</span></span>

<span data-ttu-id="b8a91-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b8a91-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8a91-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b8a91-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8a91-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8a91-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8a91-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b8a91-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b8a91-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b8a91-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8a91-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b8a91-140">Validation File</span></span>  <br/> |<span data-ttu-id="b8a91-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b8a91-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8a91-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b8a91-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8a91-143">False</span><span class="sxs-lookup"><span data-stu-id="b8a91-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8a91-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="b8a91-144">See also</span></span>

- [<span data-ttu-id="b8a91-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b8a91-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b8a91-146">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="b8a91-146">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

