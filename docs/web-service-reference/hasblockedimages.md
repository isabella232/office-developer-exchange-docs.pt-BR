---
title: HasBlockedImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddeb11db-797d-4939-91d5-3e44be5f0778
description: O elemento HasBlockedImages especifica um valor Boolean que indica se o item tem imagens bloqueadas.
ms.openlocfilehash: 370ab4b12ae841815faa344b2fd3a6d3ddc16bcb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462791"
---
# <a name="hasblockedimages"></a><span data-ttu-id="23dde-103">HasBlockedImages</span><span class="sxs-lookup"><span data-stu-id="23dde-103">HasBlockedImages</span></span>

<span data-ttu-id="23dde-104">O elemento **HasBlockedImages** especifica um valor Boolean que indica se o item tem imagens bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="23dde-104">The **HasBlockedImages** element specifies a Boolean value that indicates whether the item has blocked images.</span></span> 
  
```XML
<HasBlockedImages> true | false </HasBlockedImages>
```

 <span data-ttu-id="23dde-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="23dde-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23dde-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="23dde-106">Attributes and elements</span></span>

<span data-ttu-id="23dde-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="23dde-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23dde-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="23dde-108">Attributes</span></span>

<span data-ttu-id="23dde-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23dde-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23dde-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="23dde-110">Child elements</span></span>

<span data-ttu-id="23dde-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="23dde-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23dde-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="23dde-112">Parent elements</span></span>

|<span data-ttu-id="23dde-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="23dde-113">**Element**</span></span>|<span data-ttu-id="23dde-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23dde-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23dde-115">Item</span><span class="sxs-lookup"><span data-stu-id="23dde-115">Item</span></span>](item.md) <br/> |<span data-ttu-id="23dde-116">Representa um item genérico no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="23dde-116">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="23dde-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="23dde-117">Text value</span></span>

<span data-ttu-id="23dde-118">Um valor de texto **true** para o elemento **HasBlockedImages** indica que o item tem imagens bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="23dde-118">A text value of **true** for the **HasBlockedImages** element indicates that the item has blocked images.</span></span> <span data-ttu-id="23dde-119">Um valor **false** indica que o item não tem nenhuma imagem bloqueada.</span><span class="sxs-lookup"><span data-stu-id="23dde-119">A value of **false** indicates that the item does not have any blocked images.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="23dde-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="23dde-120">Remarks</span></span>

<span data-ttu-id="23dde-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="23dde-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23dde-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="23dde-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23dde-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="23dde-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23dde-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="23dde-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23dde-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="23dde-125">Schema Name</span></span>  <br/> |<span data-ttu-id="23dde-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="23dde-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="23dde-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="23dde-127">Validation File</span></span>  <br/> |<span data-ttu-id="23dde-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="23dde-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="23dde-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="23dde-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="23dde-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="23dde-130">See also</span></span>



- [<span data-ttu-id="23dde-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="23dde-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

