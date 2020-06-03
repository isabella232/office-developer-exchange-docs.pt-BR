---
title: Tempo limite (duração)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: O elemento timeout especifica o período de tempo antes de o tempo limite de uma assinatura pull ter expirado pelo servidor.
ms.openlocfilehash: b5b0e77d794080cd8e0da1e14acf4cb059b80b08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460278"
---
# <a name="timeout-duration"></a><span data-ttu-id="9e4b5-103">Tempo limite (duração)</span><span class="sxs-lookup"><span data-stu-id="9e4b5-103">Timeout (duration)</span></span>

<span data-ttu-id="9e4b5-104">O elemento **Timeout** especifica o período de tempo antes de o tempo limite de uma assinatura pull ter expirado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="9e4b5-105">**SubscriptionTimeoutType**</span><span class="sxs-lookup"><span data-stu-id="9e4b5-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e4b5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9e4b5-106">Attributes and elements</span></span>

<span data-ttu-id="9e4b5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e4b5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9e4b5-108">Attributes</span></span>

<span data-ttu-id="9e4b5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e4b5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e4b5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9e4b5-110">Child elements</span></span>

<span data-ttu-id="9e4b5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e4b5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9e4b5-112">Parent elements</span></span>

[<span data-ttu-id="9e4b5-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="9e4b5-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="9e4b5-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9e4b5-114">Text value</span></span>

<span data-ttu-id="9e4b5-115">O valor de texto do elemento **Timeout** é o período de tempo, em minutos, antes que uma assinatura pull seja esgotada pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="9e4b5-116">O valor mínimo é 1; o valor máximo é 1440.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9e4b5-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e4b5-117">Remarks</span></span>

<span data-ttu-id="9e4b5-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e4b5-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e4b5-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e4b5-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9e4b5-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e4b5-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e4b5-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e4b5-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9e4b5-122">Schema name</span></span>  <br/> |<span data-ttu-id="9e4b5-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9e4b5-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e4b5-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9e4b5-124">Validation file</span></span>  <br/> |<span data-ttu-id="9e4b5-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9e4b5-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e4b5-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9e4b5-126">Can be empty</span></span>  <br/> ||
   

