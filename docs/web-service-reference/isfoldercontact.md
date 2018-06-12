---
title: IsFolderContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderContact
api_type:
- schema
ms.assetid: 8b456255-f4ae-4ca0-845a-13c195f1c867
description: O elemento IsFolderContact indica se um usuário é um contato para uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 51a79b4535667685517ff55ef9f6c2b2aaea564c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824015"
---
# <a name="isfoldercontact"></a><span data-ttu-id="e6b69-104">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="e6b69-104">IsFolderContact</span></span>

<span data-ttu-id="e6b69-105">O elemento **IsFolderContact** indica se um usuário é um contato para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e6b69-105">The **IsFolderContact** element indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="e6b69-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e6b69-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderContact/>
```

 <span data-ttu-id="e6b69-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e6b69-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6b69-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e6b69-108">Attributes and elements</span></span>

<span data-ttu-id="e6b69-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e6b69-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6b69-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e6b69-110">Attributes</span></span>

<span data-ttu-id="e6b69-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e6b69-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6b69-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e6b69-112">Child elements</span></span>

<span data-ttu-id="e6b69-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e6b69-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e6b69-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e6b69-114">Parent elements</span></span>

|<span data-ttu-id="e6b69-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e6b69-115">**Element**</span></span>|<span data-ttu-id="e6b69-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6b69-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6b69-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="e6b69-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="e6b69-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e6b69-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="e6b69-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="e6b69-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="e6b69-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="e6b69-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="e6b69-121">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="e6b69-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="e6b69-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="e6b69-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e6b69-123">Text value</span><span class="sxs-lookup"><span data-stu-id="e6b69-123">Text value</span></span>

<span data-ttu-id="e6b69-124">Um valor de texto de **true** indica que o usuário é um contato da pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="e6b69-124">A text value of **true** indicates that the user is a contact for the specified folder.</span></span> <span data-ttu-id="e6b69-125">Um valor **false** indica que o usuário não é um contato da pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="e6b69-125">A value of **false** indicates that the user is not a contact for the specified folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e6b69-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e6b69-126">Remarks</span></span>

<span data-ttu-id="e6b69-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e6b69-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6b69-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e6b69-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6b69-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e6b69-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6b69-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e6b69-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e6b69-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e6b69-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6b69-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e6b69-132">Validation File</span></span>  <br/> |<span data-ttu-id="e6b69-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e6b69-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6b69-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e6b69-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6b69-135">False</span><span class="sxs-lookup"><span data-stu-id="e6b69-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6b69-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="e6b69-136">See also</span></span>



- [<span data-ttu-id="e6b69-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e6b69-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e6b69-138">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="e6b69-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

