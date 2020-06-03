---
title: Excreateitems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateItems
api_type:
- schema
ms.assetid: c4574e9a-3c42-40a1-a5f9-79b6560e9b30
description: O elemento cancreateitems indica se um usuário tem permissão para criar itens em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 73d3d967774d9fcff53722d0936462025e02b659
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458779"
---
# <a name="cancreateitems"></a><span data-ttu-id="3af0c-104">Excreateitems</span><span class="sxs-lookup"><span data-stu-id="3af0c-104">CanCreateItems</span></span>

<span data-ttu-id="3af0c-105">O elemento **Cancreateitems** indica se um usuário tem permissão para criar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3af0c-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="3af0c-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3af0c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="3af0c-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3af0c-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3af0c-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3af0c-108">Attributes and elements</span></span>

<span data-ttu-id="3af0c-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3af0c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3af0c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3af0c-110">Attributes</span></span>

<span data-ttu-id="3af0c-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3af0c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3af0c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3af0c-112">Child elements</span></span>

<span data-ttu-id="3af0c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3af0c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3af0c-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3af0c-114">Parent elements</span></span>

|<span data-ttu-id="3af0c-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3af0c-115">**Element**</span></span>|<span data-ttu-id="3af0c-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3af0c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3af0c-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="3af0c-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="3af0c-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3af0c-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="3af0c-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="3af0c-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="3af0c-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="3af0c-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="3af0c-121">Define o acesso que um usuário tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="3af0c-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="3af0c-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="3af0c-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3af0c-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3af0c-123">Text value</span></span>

<span data-ttu-id="3af0c-124">Um valor de texto **true** indica que o usuário pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="3af0c-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="3af0c-125">Um valor **false** indica que o usuário não pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="3af0c-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3af0c-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="3af0c-126">Remarks</span></span>

<span data-ttu-id="3af0c-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3af0c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3af0c-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3af0c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3af0c-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3af0c-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3af0c-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3af0c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3af0c-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3af0c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3af0c-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3af0c-132">Validation File</span></span>  <br/> |<span data-ttu-id="3af0c-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3af0c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3af0c-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3af0c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3af0c-135">False</span><span class="sxs-lookup"><span data-stu-id="3af0c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3af0c-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="3af0c-136">See also</span></span>



- [<span data-ttu-id="3af0c-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3af0c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3af0c-138">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="3af0c-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

