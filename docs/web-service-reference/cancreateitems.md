---
title: CanCreateItems
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
description: O elemento CanCreateItems indica se um usuário tem permissão para criar itens em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 313699a15ef3038dd9114c18b76b29aba15e5ab7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751379"
---
# <a name="cancreateitems"></a><span data-ttu-id="638af-104">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="638af-104">CanCreateItems</span></span>

<span data-ttu-id="638af-105">O elemento **CanCreateItems** indica se um usuário tem permissão para criar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="638af-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="638af-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="638af-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="638af-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="638af-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="638af-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="638af-108">Attributes and elements</span></span>

<span data-ttu-id="638af-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="638af-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="638af-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="638af-110">Attributes</span></span>

<span data-ttu-id="638af-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="638af-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="638af-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="638af-112">Child elements</span></span>

<span data-ttu-id="638af-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="638af-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="638af-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="638af-114">Parent elements</span></span>

|<span data-ttu-id="638af-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="638af-115">**Element**</span></span>|<span data-ttu-id="638af-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="638af-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="638af-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="638af-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="638af-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="638af-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="638af-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="638af-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="638af-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="638af-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="638af-121">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="638af-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="638af-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="638af-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="638af-123">Text value</span><span class="sxs-lookup"><span data-stu-id="638af-123">Text value</span></span>

<span data-ttu-id="638af-124">Um valor de texto de **true** indica que o usuário pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="638af-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="638af-125">Um valor **false** indica que o usuário não pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="638af-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="638af-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="638af-126">Remarks</span></span>

<span data-ttu-id="638af-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="638af-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="638af-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="638af-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="638af-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="638af-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="638af-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="638af-130">Schema Name</span></span>  <br/> |<span data-ttu-id="638af-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="638af-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="638af-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="638af-132">Validation File</span></span>  <br/> |<span data-ttu-id="638af-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="638af-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="638af-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="638af-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="638af-135">False</span><span class="sxs-lookup"><span data-stu-id="638af-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="638af-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="638af-136">See also</span></span>



- [<span data-ttu-id="638af-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="638af-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="638af-138">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="638af-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

