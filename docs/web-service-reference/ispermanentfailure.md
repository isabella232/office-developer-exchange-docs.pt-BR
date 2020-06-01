---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: O elemento IsPermanentFailure indica se uma tentativa anterior de indexar o item não foi bem sucedida.
ms.openlocfilehash: 48a13eebfa16c538c1b10d92f080d51f1b318d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460390"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="27ab8-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="27ab8-103">IsPermanentFailure</span></span>

<span data-ttu-id="27ab8-104">O elemento **IsPermanentFailure** indica se uma tentativa anterior de indexar o item não foi bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="27ab8-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="27ab8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="27ab8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27ab8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="27ab8-106">Attributes and elements</span></span>

<span data-ttu-id="27ab8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="27ab8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27ab8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="27ab8-108">Attributes</span></span>

<span data-ttu-id="27ab8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27ab8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27ab8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="27ab8-110">Child elements</span></span>

<span data-ttu-id="27ab8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="27ab8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27ab8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="27ab8-112">Parent elements</span></span>

[<span data-ttu-id="27ab8-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="27ab8-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="27ab8-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="27ab8-114">Text value</span></span>

<span data-ttu-id="27ab8-115">Um valor de texto **true** para o elemento **IsPermanentFailure** indica que uma tentativa anterior de indexar o item da caixa de correio não foi bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="27ab8-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="27ab8-116">Um valor **false** indica que uma tentativa anterior de indexar o item da caixa de correio foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="27ab8-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="27ab8-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="27ab8-117">Remarks</span></span>

<span data-ttu-id="27ab8-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="27ab8-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="27ab8-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="27ab8-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27ab8-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="27ab8-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27ab8-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="27ab8-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27ab8-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="27ab8-122">Schema name</span></span>  <br/> |<span data-ttu-id="27ab8-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="27ab8-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="27ab8-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="27ab8-124">Validation file</span></span>  <br/> |<span data-ttu-id="27ab8-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="27ab8-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27ab8-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="27ab8-126">Can be empty</span></span>  <br/> |<span data-ttu-id="27ab8-127">falso</span><span class="sxs-lookup"><span data-stu-id="27ab8-127">false</span></span>  <br/> |
   

