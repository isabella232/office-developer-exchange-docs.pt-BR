---
title: Createhierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateHierarchy
api_type:
- schema
ms.assetid: 630b5610-1c19-4d4a-a5df-8cebb9afd2f4
description: O elemento createhierarchy indica se um cliente pode criar uma tabela de hierarquia. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 3fb0c34a8a148cc8336c70d643a21ecb6fef30b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457519"
---
# <a name="createhierarchy"></a><span data-ttu-id="ee5dd-104">Createhierarchy</span><span class="sxs-lookup"><span data-stu-id="ee5dd-104">CreateHierarchy</span></span>

<span data-ttu-id="ee5dd-105">O elemento **createhierarchy** indica se um cliente pode criar uma tabela de hierarquia.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-105">The **CreateHierarchy** element indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="ee5dd-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ee5dd-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateHierarchy>true or false</CreateHierarchy>
```

 <span data-ttu-id="ee5dd-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="ee5dd-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee5dd-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ee5dd-108">Attributes and elements</span></span>

<span data-ttu-id="ee5dd-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee5dd-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ee5dd-110">Attributes</span></span>

<span data-ttu-id="ee5dd-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee5dd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee5dd-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ee5dd-112">Child elements</span></span>

<span data-ttu-id="ee5dd-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ee5dd-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ee5dd-114">Parent elements</span></span>

|<span data-ttu-id="ee5dd-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee5dd-115">**Element**</span></span>|<span data-ttu-id="ee5dd-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee5dd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee5dd-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ee5dd-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ee5dd-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ee5dd-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ee5dd-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ee5dd-120">Text value</span></span>

<span data-ttu-id="ee5dd-121">Um valor **true** indica que um cliente pode criar uma tabela de hierarquia.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-121">A text value of **true** indicates that a client can create a hierarchy table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ee5dd-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee5dd-122">Remarks</span></span>

<span data-ttu-id="ee5dd-123">Esta propriedade só é usada em objetos Folder.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="ee5dd-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ee5dd-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee5dd-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ee5dd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee5dd-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="ee5dd-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee5dd-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ee5dd-127">Schema Name</span></span>  <br/> |<span data-ttu-id="ee5dd-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ee5dd-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ee5dd-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ee5dd-129">Validation File</span></span>  <br/> |<span data-ttu-id="ee5dd-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ee5dd-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee5dd-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ee5dd-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee5dd-132">False</span><span class="sxs-lookup"><span data-stu-id="ee5dd-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee5dd-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="ee5dd-133">See also</span></span>



- [<span data-ttu-id="ee5dd-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ee5dd-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ee5dd-135">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="ee5dd-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

