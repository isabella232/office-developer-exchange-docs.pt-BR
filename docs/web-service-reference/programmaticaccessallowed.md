---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: O elemento ProgrammaticAccessAllowed especifica se o acesso programático está habilitado para dados gerenciados por direitos.
ms.openlocfilehash: 8a5cf4e57a97807e5940a0402768d7123b9912d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465636"
---
# <a name="programmaticaccessallowed"></a><span data-ttu-id="a1cd3-103">ProgrammaticAccessAllowed</span><span class="sxs-lookup"><span data-stu-id="a1cd3-103">ProgrammaticAccessAllowed</span></span>

<span data-ttu-id="a1cd3-104">O elemento **ProgrammaticAccessAllowed** especifica se o acesso programático está habilitado para dados gerenciados por direitos.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-104">The **ProgrammaticAccessAllowed** element specifies whether programmatic access is enabled for rights managed data.</span></span> 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 <span data-ttu-id="a1cd3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a1cd3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1cd3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a1cd3-106">Attributes and elements</span></span>

<span data-ttu-id="a1cd3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1cd3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a1cd3-108">Attributes</span></span>

<span data-ttu-id="a1cd3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1cd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1cd3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a1cd3-110">Child elements</span></span>

<span data-ttu-id="a1cd3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1cd3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a1cd3-112">Parent elements</span></span>

[<span data-ttu-id="a1cd3-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="a1cd3-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="a1cd3-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a1cd3-114">Text value</span></span>

<span data-ttu-id="a1cd3-115">Um valor de texto **true** para o elemento **ProgrammaticAccessAllowed** indica que os dados estão acessíveis programaticamente.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-115">A text value of **true** for the **ProgrammaticAccessAllowed** element indicates that the data is programmatically accessible.</span></span> <span data-ttu-id="a1cd3-116">Um valor **false** indica que os dados não são acessíveis programaticamente.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-116">A value of **false** indicates that the data is not programmatically accessible.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a1cd3-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="a1cd3-117">Remarks</span></span>

<span data-ttu-id="a1cd3-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a1cd3-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1cd3-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1cd3-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a1cd3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1cd3-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1cd3-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1cd3-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a1cd3-122">Schema name</span></span>  <br/> |<span data-ttu-id="a1cd3-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a1cd3-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1cd3-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a1cd3-124">Validation file</span></span>  <br/> |<span data-ttu-id="a1cd3-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a1cd3-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1cd3-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a1cd3-126">Can be empty</span></span>  <br/> |<span data-ttu-id="a1cd3-127">falso</span><span class="sxs-lookup"><span data-stu-id="a1cd3-127">false</span></span>  <br/> |
   

