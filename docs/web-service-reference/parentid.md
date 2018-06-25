---
title: ParentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb7aaa46-3a04-4197-aebb-8881ff10603f
description: O elemento ParentId Especifica o identificador do item pai em uma visualização de pesquisa.
ms.openlocfilehash: ddc76320b1c482e3518a98fb63fc2296143d163c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824698"
---
# <a name="parentid"></a><span data-ttu-id="2913b-103">ParentId</span><span class="sxs-lookup"><span data-stu-id="2913b-103">ParentId</span></span>

<span data-ttu-id="2913b-104">O elemento **ParentId** Especifica o identificador do item pai em uma visualização de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2913b-104">The **ParentId** element specifies the identifier of the parent item in a search preview.</span></span> 
  
```XML
<ParentId Id="" ChangeKey=""/>
```

<span data-ttu-id="2913b-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="2913b-105">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2913b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2913b-106">Attributes and elements</span></span>

<span data-ttu-id="2913b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2913b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2913b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2913b-108">Attributes</span></span>

|<span data-ttu-id="2913b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="2913b-109">**Attribute**</span></span>|<span data-ttu-id="2913b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2913b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2913b-111">Id</span><span class="sxs-lookup"><span data-stu-id="2913b-111">Id</span></span>  <br/> |<span data-ttu-id="2913b-112">O valor de texto do atributo **Id** é o identificador do item pai.</span><span class="sxs-lookup"><span data-stu-id="2913b-112">The text value of the **Id** attribute is the identifier of the parent item.</span></span>  <br/> |
|<span data-ttu-id="2913b-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="2913b-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="2913b-114">O valor de texto do atributo **ChangeKey** é a chave de alteração do item pai.</span><span class="sxs-lookup"><span data-stu-id="2913b-114">The text value of the **ChangeKey** attribute is the change key of the parent item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2913b-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2913b-115">Child elements</span></span>

<span data-ttu-id="2913b-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2913b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2913b-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2913b-117">Parent elements</span></span>

[<span data-ttu-id="2913b-118">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="2913b-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="2913b-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="2913b-119">Remarks</span></span>

<span data-ttu-id="2913b-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2913b-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2913b-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2913b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2913b-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2913b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2913b-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="2913b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2913b-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2913b-124">Schema name</span></span>  <br/> |<span data-ttu-id="2913b-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2913b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2913b-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2913b-126">Validation file</span></span>  <br/> |<span data-ttu-id="2913b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2913b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2913b-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2913b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="2913b-129">true</span><span class="sxs-lookup"><span data-stu-id="2913b-129">true</span></span>  <br/> |
   

