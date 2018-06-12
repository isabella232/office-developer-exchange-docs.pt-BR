---
title: Modificar
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Modify
api_type:
- schema
ms.assetid: 7a51e9e1-addb-4343-8a22-78f23763c0a8
description: O elemento de modificar indica se um cliente pode modificar uma pasta ou item. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 29fd2184e83f66a9b7e7db4173a765cee2922be8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824514"
---
# <a name="modify"></a><span data-ttu-id="0ffc9-104">Modificar</span><span class="sxs-lookup"><span data-stu-id="0ffc9-104">Modify</span></span>

<span data-ttu-id="0ffc9-105">O elemento de **Modificar** indica se um cliente pode modificar uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-105">The **Modify** element indicates whether a client can modify a folder or item.</span></span> <span data-ttu-id="0ffc9-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0ffc9-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Modify>true or false</Modify>
```

 <span data-ttu-id="0ffc9-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0ffc9-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ffc9-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0ffc9-108">Attributes and elements</span></span>

<span data-ttu-id="0ffc9-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ffc9-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0ffc9-110">Attributes</span></span>

<span data-ttu-id="0ffc9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ffc9-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0ffc9-112">Child elements</span></span>

<span data-ttu-id="0ffc9-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ffc9-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0ffc9-114">Parent elements</span></span>

|<span data-ttu-id="0ffc9-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0ffc9-115">**Element**</span></span>|<span data-ttu-id="0ffc9-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ffc9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ffc9-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="0ffc9-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="0ffc9-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="0ffc9-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ffc9-120">Text value</span><span class="sxs-lookup"><span data-stu-id="0ffc9-120">Text value</span></span>

<span data-ttu-id="0ffc9-121">Um valor de texto de **true** indica que um cliente pode modificar um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-121">A text value of **true** indicates that a client can modify an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0ffc9-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0ffc9-122">Remarks</span></span>

<span data-ttu-id="0ffc9-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ffc9-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0ffc9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ffc9-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="0ffc9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ffc9-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0ffc9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0ffc9-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0ffc9-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ffc9-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0ffc9-128">Validation File</span></span>  <br/> |<span data-ttu-id="0ffc9-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ffc9-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ffc9-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0ffc9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ffc9-131">False</span><span class="sxs-lookup"><span data-stu-id="0ffc9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ffc9-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="0ffc9-132">See also</span></span>



- [<span data-ttu-id="0ffc9-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0ffc9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0ffc9-134">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="0ffc9-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

