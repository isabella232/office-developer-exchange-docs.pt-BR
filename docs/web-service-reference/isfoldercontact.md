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
ms.openlocfilehash: b7830a94237b721d02409e2d93b27c2c5ef015e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455279"
---
# <a name="isfoldercontact"></a><span data-ttu-id="482a3-104">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="482a3-104">IsFolderContact</span></span>

<span data-ttu-id="482a3-105">O elemento **IsFolderContact** indica se um usuário é um contato para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="482a3-105">The **IsFolderContact** element indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="482a3-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="482a3-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderContact/>
```

 <span data-ttu-id="482a3-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="482a3-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="482a3-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="482a3-108">Attributes and elements</span></span>

<span data-ttu-id="482a3-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="482a3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="482a3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="482a3-110">Attributes</span></span>

<span data-ttu-id="482a3-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="482a3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="482a3-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="482a3-112">Child elements</span></span>

<span data-ttu-id="482a3-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="482a3-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="482a3-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="482a3-114">Parent elements</span></span>

|<span data-ttu-id="482a3-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="482a3-115">**Element**</span></span>|<span data-ttu-id="482a3-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="482a3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="482a3-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="482a3-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="482a3-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="482a3-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="482a3-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="482a3-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="482a3-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="482a3-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="482a3-121">Define o acesso que um usuário tem a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="482a3-121">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="482a3-122">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="482a3-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="482a3-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="482a3-123">Text value</span></span>

<span data-ttu-id="482a3-124">Um valor de texto **true** indica que o usuário é um contato para a pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="482a3-124">A text value of **true** indicates that the user is a contact for the specified folder.</span></span> <span data-ttu-id="482a3-125">Um valor **false** indica que o usuário não é um contato para a pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="482a3-125">A value of **false** indicates that the user is not a contact for the specified folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="482a3-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="482a3-126">Remarks</span></span>

<span data-ttu-id="482a3-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="482a3-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="482a3-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="482a3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="482a3-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="482a3-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="482a3-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="482a3-130">Schema Name</span></span>  <br/> |<span data-ttu-id="482a3-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="482a3-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="482a3-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="482a3-132">Validation File</span></span>  <br/> |<span data-ttu-id="482a3-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="482a3-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="482a3-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="482a3-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="482a3-135">False</span><span class="sxs-lookup"><span data-stu-id="482a3-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="482a3-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="482a3-136">See also</span></span>



- [<span data-ttu-id="482a3-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="482a3-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="482a3-138">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="482a3-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

