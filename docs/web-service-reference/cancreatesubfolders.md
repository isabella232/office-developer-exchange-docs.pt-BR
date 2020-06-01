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
ms.openlocfilehash: d8e89c7a07ef1788717f5012840f5b8f79d319e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461594"
---
# <a name="cancreatesubfolders"></a><span data-ttu-id="5dec9-104">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="5dec9-104">CanCreateSubFolders</span></span>

<span data-ttu-id="5dec9-105">O elemento **CanCreateSubFolders** indica se um usuário tem permissão para criar subpastas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5dec9-105">The **CanCreateSubFolders** element indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="5dec9-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5dec9-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateSubFolders/>
```

 <span data-ttu-id="5dec9-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5dec9-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dec9-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5dec9-108">Attributes and elements</span></span>

<span data-ttu-id="5dec9-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5dec9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dec9-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="5dec9-110">Attributes</span></span>

<span data-ttu-id="5dec9-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dec9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dec9-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5dec9-112">Child elements</span></span>

<span data-ttu-id="5dec9-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5dec9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5dec9-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5dec9-114">Parent elements</span></span>

|<span data-ttu-id="5dec9-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5dec9-115">**Element**</span></span>|<span data-ttu-id="5dec9-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5dec9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dec9-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="5dec9-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="5dec9-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5dec9-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="5dec9-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="5dec9-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="5dec9-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="5dec9-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="5dec9-121">Define o acesso que um usuário tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="5dec9-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="5dec9-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="5dec9-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5dec9-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5dec9-123">Text value</span></span>

<span data-ttu-id="5dec9-124">Um valor **true** indica que o usuário pode criar subpastas na pasta.</span><span class="sxs-lookup"><span data-stu-id="5dec9-124">A text value of **true** indicates that the user can create subfolders in the folder.</span></span> <span data-ttu-id="5dec9-125">Um valor **false** indica que o usuário não pode criar subpastas na pasta.</span><span class="sxs-lookup"><span data-stu-id="5dec9-125">A value of **false** indicates that the user cannot create subfolders in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5dec9-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="5dec9-126">Remarks</span></span>

<span data-ttu-id="5dec9-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5dec9-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dec9-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5dec9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dec9-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="5dec9-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5dec9-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5dec9-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5dec9-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5dec9-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5dec9-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5dec9-132">Validation File</span></span>  <br/> |<span data-ttu-id="5dec9-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5dec9-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5dec9-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5dec9-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5dec9-135">False</span><span class="sxs-lookup"><span data-stu-id="5dec9-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dec9-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="5dec9-136">See also</span></span>



- [<span data-ttu-id="5dec9-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5dec9-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5dec9-138">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="5dec9-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

