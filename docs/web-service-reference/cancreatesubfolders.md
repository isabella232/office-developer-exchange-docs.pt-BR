---
title: CanCreateSubFolders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateSubFolders
api_type:
- schema
ms.assetid: 4404a1cc-6d3f-4996-9647-58a740e8f883
description: O elemento CanCreateSubFolders indica se um usuário tem permissão para criar subpastas em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 234cbf604a3f0f5aa6e7fa896b7b6735516bd9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751377"
---
# <a name="cancreatesubfolders"></a><span data-ttu-id="3053c-104">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="3053c-104">CanCreateSubFolders</span></span>

<span data-ttu-id="3053c-105">O elemento **CanCreateSubFolders** indica se um usuário tem permissão para criar subpastas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3053c-105">The **CanCreateSubFolders** element indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="3053c-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3053c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateSubFolders/>
```

 <span data-ttu-id="3053c-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3053c-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3053c-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3053c-108">Attributes and elements</span></span>

<span data-ttu-id="3053c-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3053c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3053c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3053c-110">Attributes</span></span>

<span data-ttu-id="3053c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3053c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3053c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3053c-112">Child elements</span></span>

<span data-ttu-id="3053c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3053c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3053c-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3053c-114">Parent elements</span></span>

|<span data-ttu-id="3053c-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3053c-115">**Element**</span></span>|<span data-ttu-id="3053c-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3053c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3053c-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="3053c-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="3053c-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3053c-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="3053c-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="3053c-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="3053c-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="3053c-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="3053c-121">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="3053c-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="3053c-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="3053c-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3053c-123">Text value</span><span class="sxs-lookup"><span data-stu-id="3053c-123">Text value</span></span>

<span data-ttu-id="3053c-124">Um valor de texto de **true** indica que o usuário pode criar subpastas na pasta.</span><span class="sxs-lookup"><span data-stu-id="3053c-124">A text value of **true** indicates that the user can create subfolders in the folder.</span></span> <span data-ttu-id="3053c-125">Um valor **false** indica que o usuário não é possível criar subpastas na pasta.</span><span class="sxs-lookup"><span data-stu-id="3053c-125">A value of **false** indicates that the user cannot create subfolders in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3053c-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3053c-126">Remarks</span></span>

<span data-ttu-id="3053c-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3053c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3053c-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3053c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3053c-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3053c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3053c-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3053c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3053c-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3053c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3053c-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3053c-132">Validation File</span></span>  <br/> |<span data-ttu-id="3053c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3053c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3053c-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3053c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3053c-135">False</span><span class="sxs-lookup"><span data-stu-id="3053c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3053c-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="3053c-136">See also</span></span>



- [<span data-ttu-id="3053c-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3053c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3053c-138">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="3053c-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

