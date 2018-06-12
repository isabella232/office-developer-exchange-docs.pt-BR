---
title: Tempo limite (duração)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: O elemento de Timeout Especifica o período de tempo antes de uma inscrição de recepção esgotado pelo servidor.
ms.openlocfilehash: 23b210dcdd87f2388aecec246068f12ec6c69a78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837722"
---
# <a name="timeout-duration"></a><span data-ttu-id="e311b-103">Tempo limite (duração)</span><span class="sxs-lookup"><span data-stu-id="e311b-103">Timeout (duration)</span></span>

<span data-ttu-id="e311b-104">O elemento de **Timeout** Especifica o período de tempo antes de uma inscrição de recepção esgotado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="e311b-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="e311b-105">**SubscriptionTimeoutType**</span><span class="sxs-lookup"><span data-stu-id="e311b-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e311b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e311b-106">Attributes and elements</span></span>

<span data-ttu-id="e311b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e311b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e311b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e311b-108">Attributes</span></span>

<span data-ttu-id="e311b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e311b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e311b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e311b-110">Child elements</span></span>

<span data-ttu-id="e311b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e311b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e311b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e311b-112">Parent elements</span></span>

[<span data-ttu-id="e311b-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="e311b-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="e311b-114">Text value</span><span class="sxs-lookup"><span data-stu-id="e311b-114">Text value</span></span>

<span data-ttu-id="e311b-115">O valor do elemento de **tempo limite** de texto é o período de tempo, em minutos, antes de uma inscrição de recepção esgotada pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="e311b-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="e311b-116">O valor mínimo é 1; o valor máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="e311b-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e311b-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e311b-117">Remarks</span></span>

<span data-ttu-id="e311b-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e311b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e311b-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e311b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e311b-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e311b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e311b-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="e311b-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e311b-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e311b-122">Schema name</span></span>  <br/> |<span data-ttu-id="e311b-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e311b-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e311b-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e311b-124">Validation file</span></span>  <br/> |<span data-ttu-id="e311b-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e311b-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e311b-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e311b-126">Can be empty</span></span>  <br/> ||
   

