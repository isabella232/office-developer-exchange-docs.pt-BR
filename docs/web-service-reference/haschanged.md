---
title: HasChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 15ff513d-f39e-44ed-a13f-ab3f86fa37e1
description: O elemento HasChanged indica se a foto de um usuário foi alterada.
ms.openlocfilehash: d777220f55d33cde548d8257cf249b57481a43f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462784"
---
# <a name="haschanged"></a><span data-ttu-id="3d314-103">HasChanged</span><span class="sxs-lookup"><span data-stu-id="3d314-103">HasChanged</span></span>

<span data-ttu-id="3d314-104">O elemento **HasChanged** indica se a foto de um usuário foi alterada.</span><span class="sxs-lookup"><span data-stu-id="3d314-104">The **HasChanged** element indicates whether a user's photo has changed.</span></span> 
  
```XML
<HasChanged> true | false </HasChanged>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="3d314-105">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3d314-105">Attributes and elements</span></span>

<span data-ttu-id="3d314-106">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3d314-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d314-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="3d314-107">Attributes</span></span>

<span data-ttu-id="3d314-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d314-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d314-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3d314-109">Child elements</span></span>

<span data-ttu-id="3d314-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3d314-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3d314-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3d314-111">Parent elements</span></span>

[<span data-ttu-id="3d314-112">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="3d314-112">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
  
## <a name="text-value"></a><span data-ttu-id="3d314-113">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3d314-113">Text value</span></span>

<span data-ttu-id="3d314-114">Um valor de texto **true** para o elemento **HasChanged** indica que a foto foi alterada desde a última vez que foi retornada.</span><span class="sxs-lookup"><span data-stu-id="3d314-114">A text value of **true** for the **HasChanged** element indicates that the photo has changed since the last time it was returned.</span></span> <span data-ttu-id="3d314-115">Um valor **false** indica que a foto não foi alterada desde a última vez que foi retornada.</span><span class="sxs-lookup"><span data-stu-id="3d314-115">A value of **false** indicates that the photo has not changed since the last time it was returned.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3d314-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="3d314-116">Remarks</span></span>

<span data-ttu-id="3d314-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3d314-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3d314-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d314-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d314-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3d314-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d314-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d314-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3d314-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3d314-121">Schema name</span></span>  <br/> |<span data-ttu-id="3d314-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3d314-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="3d314-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3d314-123">Validation file</span></span>  <br/> |<span data-ttu-id="3d314-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3d314-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3d314-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3d314-125">Can be empty</span></span>  <br/> ||
   

