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
description: O elemento de excluir indica se um cliente pode excluir uma pasta ou item.
ms.openlocfilehash: 8a00a24ea63fa564ecefb96a5caed3a9199690eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751727"
---
# <a name="delete"></a><span data-ttu-id="637ca-103">Excluir</span><span class="sxs-lookup"><span data-stu-id="637ca-103">Delete</span></span>

<span data-ttu-id="637ca-104">O elemento **Excluir** indica se um cliente pode excluir uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="637ca-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="637ca-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="637ca-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="637ca-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="637ca-106">Attributes and elements</span></span>

<span data-ttu-id="637ca-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="637ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="637ca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="637ca-108">Attributes</span></span>

<span data-ttu-id="637ca-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="637ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="637ca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="637ca-110">Child elements</span></span>

<span data-ttu-id="637ca-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="637ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="637ca-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="637ca-112">Parent elements</span></span>

|<span data-ttu-id="637ca-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="637ca-113">**Element**</span></span>|<span data-ttu-id="637ca-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="637ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="637ca-115">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="637ca-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="637ca-116">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="637ca-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="637ca-117">Ações</span><span class="sxs-lookup"><span data-stu-id="637ca-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="637ca-118">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="637ca-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="637ca-119">Text value</span><span class="sxs-lookup"><span data-stu-id="637ca-119">Text value</span></span>

<span data-ttu-id="637ca-120">Um valor de texto de **true** indica que um cliente pode excluir um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="637ca-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="637ca-121">Um valor **false** indica que um cliente não é possível excluir um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="637ca-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="637ca-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="637ca-122">Remarks</span></span>

<span data-ttu-id="637ca-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="637ca-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="637ca-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="637ca-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="637ca-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="637ca-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="637ca-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="637ca-126">Schema Name</span></span>  <br/> |<span data-ttu-id="637ca-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="637ca-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="637ca-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="637ca-128">Validation File</span></span>  <br/> |<span data-ttu-id="637ca-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="637ca-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="637ca-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="637ca-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="637ca-131">False</span><span class="sxs-lookup"><span data-stu-id="637ca-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="637ca-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="637ca-132">See also</span></span>

- [<span data-ttu-id="637ca-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="637ca-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="637ca-134">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="637ca-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

