---
title: IsFolderOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderOwner
api_type:
- schema
ms.assetid: 6541ee78-d6e6-42a7-8e7a-d8736172b245
description: O elemento IsFolderOwner indica se um usuário é o proprietário de uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a8838b2a7ed1b16c1e332d34a38038ba8254fc3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824016"
---
# <a name="isfolderowner"></a><span data-ttu-id="c35de-104">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="c35de-104">IsFolderOwner</span></span>

<span data-ttu-id="c35de-105">O elemento **IsFolderOwner** indica se um usuário é o proprietário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c35de-105">The **IsFolderOwner** element indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="c35de-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c35de-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderOwner/>
```

 <span data-ttu-id="c35de-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c35de-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c35de-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c35de-108">Attributes and elements</span></span>

<span data-ttu-id="c35de-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c35de-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c35de-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c35de-110">Attributes</span></span>

<span data-ttu-id="c35de-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c35de-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c35de-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c35de-112">Child elements</span></span>

<span data-ttu-id="c35de-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c35de-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c35de-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c35de-114">Parent elements</span></span>

|<span data-ttu-id="c35de-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c35de-115">**Element**</span></span>|<span data-ttu-id="c35de-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c35de-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c35de-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="c35de-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="c35de-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c35de-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="c35de-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="c35de-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="c35de-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="c35de-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="c35de-121">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="c35de-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="c35de-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="c35de-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c35de-123">Text value</span><span class="sxs-lookup"><span data-stu-id="c35de-123">Text value</span></span>

<span data-ttu-id="c35de-124">Um valor de texto de **true** indica que o usuário é o proprietário da pasta.</span><span class="sxs-lookup"><span data-stu-id="c35de-124">A text value of **true** indicates that the user is the owner of the folder.</span></span> <span data-ttu-id="c35de-125">Um valor **false** indica que o usuário não é o proprietário da pasta.</span><span class="sxs-lookup"><span data-stu-id="c35de-125">A value of **false** indicates that the user is not the owner of the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c35de-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c35de-126">Remarks</span></span>

<span data-ttu-id="c35de-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c35de-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c35de-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c35de-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c35de-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="c35de-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c35de-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c35de-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c35de-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c35de-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="c35de-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c35de-132">Validation File</span></span>  <br/> |<span data-ttu-id="c35de-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c35de-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c35de-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c35de-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c35de-135">False</span><span class="sxs-lookup"><span data-stu-id="c35de-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c35de-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="c35de-136">See also</span></span>



- [<span data-ttu-id="c35de-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c35de-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c35de-138">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="c35de-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

