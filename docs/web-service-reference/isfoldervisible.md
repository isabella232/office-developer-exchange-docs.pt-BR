---
title: IsFolderVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderVisible
api_type:
- schema
ms.assetid: dd611fb5-9424-4ff9-bb27-c882c73c0c74
description: O elemento IsFolderVisible indica se um usuário pode exibir uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 27a6bca9ae71bc93de6c22cb87c8d582025144e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824019"
---
# <a name="isfoldervisible"></a><span data-ttu-id="d9b77-104">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="d9b77-104">IsFolderVisible</span></span>

<span data-ttu-id="d9b77-105">O elemento **IsFolderVisible** indica se um usuário pode exibir uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d9b77-105">The **IsFolderVisible** element indicates whether a user can view a folder.</span></span> <span data-ttu-id="d9b77-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d9b77-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderVisible/>
```

 <span data-ttu-id="d9b77-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d9b77-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9b77-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d9b77-108">Attributes and elements</span></span>

<span data-ttu-id="d9b77-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9b77-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9b77-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9b77-110">Attributes</span></span>

<span data-ttu-id="d9b77-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9b77-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9b77-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9b77-112">Child elements</span></span>

<span data-ttu-id="d9b77-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9b77-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9b77-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9b77-114">Parent elements</span></span>

|<span data-ttu-id="d9b77-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9b77-115">**Element**</span></span>|<span data-ttu-id="d9b77-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9b77-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9b77-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="d9b77-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="d9b77-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d9b77-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="d9b77-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d9b77-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d9b77-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="d9b77-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="d9b77-121">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="d9b77-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="d9b77-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d9b77-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9b77-123">Text value</span><span class="sxs-lookup"><span data-stu-id="d9b77-123">Text value</span></span>

<span data-ttu-id="d9b77-124">Um valor de texto de **true** indica que o usuário pode exibir a pasta.</span><span class="sxs-lookup"><span data-stu-id="d9b77-124">A text value of **true** indicates that the user can view the folder.</span></span> <span data-ttu-id="d9b77-125">Um valor **false** indica que o usuário não pode exibir a pasta.</span><span class="sxs-lookup"><span data-stu-id="d9b77-125">A value of **false** indicates that the user cannot view the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d9b77-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d9b77-126">Remarks</span></span>

<span data-ttu-id="d9b77-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d9b77-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9b77-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d9b77-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9b77-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9b77-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9b77-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9b77-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d9b77-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d9b77-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9b77-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9b77-132">Validation File</span></span>  <br/> |<span data-ttu-id="d9b77-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9b77-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9b77-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9b77-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9b77-135">False</span><span class="sxs-lookup"><span data-stu-id="d9b77-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9b77-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="d9b77-136">See also</span></span>



- [<span data-ttu-id="d9b77-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9b77-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d9b77-138">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="d9b77-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

