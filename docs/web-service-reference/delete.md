---
title: Excluir
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: aa45f0c1-a80d-4b6c-8a85-375b6de515f4
description: O elemento delete indica se um cliente pode excluir uma pasta ou item.
ms.openlocfilehash: 5460f9e49b126ca6b039c6f11aaa3c6eb4a40544
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457351"
---
# <a name="delete"></a><span data-ttu-id="c0908-103">Excluir</span><span class="sxs-lookup"><span data-stu-id="c0908-103">Delete</span></span>

<span data-ttu-id="c0908-104">O elemento **delete** indica se um cliente pode excluir uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c0908-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="c0908-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="c0908-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c0908-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c0908-106">Attributes and elements</span></span>

<span data-ttu-id="c0908-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c0908-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0908-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c0908-108">Attributes</span></span>

<span data-ttu-id="c0908-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0908-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0908-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c0908-110">Child elements</span></span>

<span data-ttu-id="c0908-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c0908-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0908-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c0908-112">Parent elements</span></span>

|<span data-ttu-id="c0908-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0908-113">**Element**</span></span>|<span data-ttu-id="c0908-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0908-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0908-115">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c0908-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="c0908-116">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="c0908-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="c0908-117">Actions</span><span class="sxs-lookup"><span data-stu-id="c0908-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="c0908-118">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="c0908-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0908-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c0908-119">Text value</span></span>

<span data-ttu-id="c0908-120">Um valor **true** indica que um cliente pode excluir um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="c0908-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="c0908-121">Um valor **false** indica que um cliente não pode excluir um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="c0908-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c0908-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0908-122">Remarks</span></span>

<span data-ttu-id="c0908-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0908-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0908-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c0908-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0908-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0908-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0908-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c0908-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c0908-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c0908-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0908-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c0908-128">Validation File</span></span>  <br/> |<span data-ttu-id="c0908-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c0908-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0908-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c0908-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0908-131">False</span><span class="sxs-lookup"><span data-stu-id="c0908-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0908-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="c0908-132">See also</span></span>

- [<span data-ttu-id="c0908-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c0908-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c0908-134">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="c0908-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

