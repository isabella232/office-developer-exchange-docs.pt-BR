---
title: HasBlockedImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddeb11db-797d-4939-91d5-3e44be5f0778
description: O elemento HasBlockedImages Especifica um valor Boolean que indica se o item bloqueou imagens.
ms.openlocfilehash: fbe9967c898016aeef27e3c86e8a1cf603bd87fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823795"
---
# <a name="hasblockedimages"></a><span data-ttu-id="fe25c-103">HasBlockedImages</span><span class="sxs-lookup"><span data-stu-id="fe25c-103">HasBlockedImages</span></span>

<span data-ttu-id="fe25c-104">O elemento **HasBlockedImages** Especifica um valor Boolean que indica se o item bloqueou imagens.</span><span class="sxs-lookup"><span data-stu-id="fe25c-104">The **HasBlockedImages** element specifies a Boolean value that indicates whether the item has blocked images.</span></span> 
  
```XML
<HasBlockedImages> true | false </HasBlockedImages>
```

 <span data-ttu-id="fe25c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fe25c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe25c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fe25c-106">Attributes and elements</span></span>

<span data-ttu-id="fe25c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fe25c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe25c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fe25c-108">Attributes</span></span>

<span data-ttu-id="fe25c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fe25c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe25c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fe25c-110">Child elements</span></span>

<span data-ttu-id="fe25c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fe25c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe25c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fe25c-112">Parent elements</span></span>

|<span data-ttu-id="fe25c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fe25c-113">**Element**</span></span>|<span data-ttu-id="fe25c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fe25c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe25c-115">Item</span><span class="sxs-lookup"><span data-stu-id="fe25c-115">Item</span></span>](item.md) <br/> |<span data-ttu-id="fe25c-116">Representa um item genérico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe25c-116">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe25c-117">Text value</span><span class="sxs-lookup"><span data-stu-id="fe25c-117">Text value</span></span>

<span data-ttu-id="fe25c-118">Um valor de texto de **true** para o elemento **HasBlockedImages** indica que o item bloqueou imagens.</span><span class="sxs-lookup"><span data-stu-id="fe25c-118">A text value of **true** for the **HasBlockedImages** element indicates that the item has blocked images.</span></span> <span data-ttu-id="fe25c-119">Um valor **false** indica que o item não tem quaisquer imagens bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="fe25c-119">A value of **false** indicates that the item does not have any blocked images.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fe25c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="fe25c-120">Remarks</span></span>

<span data-ttu-id="fe25c-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fe25c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fe25c-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe25c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe25c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fe25c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe25c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="fe25c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe25c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fe25c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fe25c-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="fe25c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="fe25c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fe25c-127">Validation File</span></span>  <br/> |<span data-ttu-id="fe25c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fe25c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe25c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fe25c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fe25c-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="fe25c-130">See also</span></span>



- [<span data-ttu-id="fe25c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fe25c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

