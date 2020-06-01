---
title: Ler
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Read
api_type:
- schema
ms.assetid: b14637e9-1695-4b7e-b078-ae527c2e4303
description: O elemento Read indica se um cliente pode ler uma pasta ou item. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d75285e0ab14c4f53d73cb7f4349196e07c3c521
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468310"
---
# <a name="read"></a><span data-ttu-id="e9d01-104">Ler</span><span class="sxs-lookup"><span data-stu-id="e9d01-104">Read</span></span>

<span data-ttu-id="e9d01-105">O elemento **Read** indica se um cliente pode ler uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="e9d01-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="e9d01-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e9d01-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="e9d01-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e9d01-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9d01-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e9d01-108">Attributes and elements</span></span>

<span data-ttu-id="e9d01-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e9d01-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9d01-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e9d01-110">Attributes</span></span>

<span data-ttu-id="e9d01-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9d01-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9d01-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e9d01-112">Child elements</span></span>

<span data-ttu-id="e9d01-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9d01-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9d01-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e9d01-114">Parent elements</span></span>

|<span data-ttu-id="e9d01-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e9d01-115">**Element**</span></span>|<span data-ttu-id="e9d01-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e9d01-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9d01-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e9d01-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e9d01-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="e9d01-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="e9d01-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="e9d01-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9d01-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e9d01-120">Text value</span></span>

<span data-ttu-id="e9d01-121">Um valor **true** indica que um cliente pode ler um item de pasta.</span><span class="sxs-lookup"><span data-stu-id="e9d01-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e9d01-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="e9d01-122">Remarks</span></span>

<span data-ttu-id="e9d01-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e9d01-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9d01-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e9d01-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9d01-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9d01-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9d01-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e9d01-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e9d01-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e9d01-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9d01-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e9d01-128">Validation File</span></span>  <br/> |<span data-ttu-id="e9d01-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e9d01-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9d01-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e9d01-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9d01-131">False</span><span class="sxs-lookup"><span data-stu-id="e9d01-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9d01-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="e9d01-132">See also</span></span>



- [<span data-ttu-id="e9d01-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e9d01-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e9d01-134">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="e9d01-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

