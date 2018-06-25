---
title: CreateContents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateContents
api_type:
- schema
ms.assetid: 8a9cd241-0d73-4be8-a563-a945898d1a0e
description: O elemento CreateContents indica se um cliente pode criar uma tabela de conteúdo. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: f84ffdd2e6b485436d9e4ccd5f03a6e2c57fcfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751573"
---
# <a name="createcontents"></a><span data-ttu-id="600a3-104">CreateContents</span><span class="sxs-lookup"><span data-stu-id="600a3-104">CreateContents</span></span>

<span data-ttu-id="600a3-105">O elemento **CreateContents** indica se um cliente pode criar uma tabela de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="600a3-105">The **CreateContents** element indicates whether a client can create a contents table.</span></span> <span data-ttu-id="600a3-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="600a3-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateContents>true or false</CreateContents>
```

 <span data-ttu-id="600a3-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="600a3-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="600a3-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="600a3-108">Attributes and elements</span></span>

<span data-ttu-id="600a3-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="600a3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="600a3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="600a3-110">Attributes</span></span>

<span data-ttu-id="600a3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="600a3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="600a3-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="600a3-112">Child elements</span></span>

<span data-ttu-id="600a3-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="600a3-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="600a3-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="600a3-114">Parent elements</span></span>

|<span data-ttu-id="600a3-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="600a3-115">**Element**</span></span>|<span data-ttu-id="600a3-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="600a3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="600a3-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="600a3-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="600a3-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="600a3-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="600a3-119">Este elemento foi introduzido inExchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="600a3-119">This element was introduced inExchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="600a3-120">Text value</span><span class="sxs-lookup"><span data-stu-id="600a3-120">Text value</span></span>

<span data-ttu-id="600a3-121">Um valor de texto de **true** indica que um cliente pode criar uma tabela de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="600a3-121">A text value of **true** indicates that a client can create a contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="600a3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="600a3-122">Remarks</span></span>

<span data-ttu-id="600a3-123">Essa propriedade é usada somente em objetos de pasta.</span><span class="sxs-lookup"><span data-stu-id="600a3-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="600a3-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="600a3-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="600a3-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="600a3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="600a3-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="600a3-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="600a3-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="600a3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="600a3-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="600a3-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="600a3-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="600a3-129">Validation File</span></span>  <br/> |<span data-ttu-id="600a3-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="600a3-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="600a3-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="600a3-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="600a3-132">False</span><span class="sxs-lookup"><span data-stu-id="600a3-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="600a3-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="600a3-133">See also</span></span>



- [<span data-ttu-id="600a3-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="600a3-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="600a3-135">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="600a3-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

