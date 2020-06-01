---
title: ConnectionTimeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionTimeout
api_type:
- schema
ms.assetid: 14da68a0-bcca-4281-a774-47644baa4ee9
description: O elemento ConnectionTimeout especifica o número de minutos para manter uma conexão aberta.
ms.openlocfilehash: 671e3cf5466ee8b3543036811708bd7f54afdcce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463850"
---
# <a name="connectiontimeout"></a><span data-ttu-id="bd14d-103">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="bd14d-103">ConnectionTimeout</span></span>

<span data-ttu-id="bd14d-104">O elemento **connectionTimeout** especifica o número de minutos para manter uma conexão aberta.</span><span class="sxs-lookup"><span data-stu-id="bd14d-104">The **ConnectionTimeout** element specifies the number of minutes to keep a connection open.</span></span> 
  
[<span data-ttu-id="bd14d-105">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="bd14d-105">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="bd14d-106">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="bd14d-106">ConnectionTimeout</span></span>](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 <span data-ttu-id="bd14d-107">**int**</span><span class="sxs-lookup"><span data-stu-id="bd14d-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd14d-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bd14d-108">Attributes and elements</span></span>

<span data-ttu-id="bd14d-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bd14d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd14d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="bd14d-110">Attributes</span></span>

<span data-ttu-id="bd14d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd14d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd14d-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bd14d-112">Child elements</span></span>

<span data-ttu-id="bd14d-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bd14d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd14d-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bd14d-114">Parent elements</span></span>

|<span data-ttu-id="bd14d-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bd14d-115">**Element**</span></span>|<span data-ttu-id="bd14d-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bd14d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd14d-117">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="bd14d-117">GetStreamingEvents</span></span>](getstreamingevents.md) <br/> |<span data-ttu-id="bd14d-118">Define uma solicitação para obter notificações de eventos de uma conexão de streaming.</span><span class="sxs-lookup"><span data-stu-id="bd14d-118">Defines a request to get event notifications from a streaming connection.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd14d-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bd14d-119">Text value</span></span>

<span data-ttu-id="bd14d-120">O valor de texto representa um inteiro que descreve o número máximo de minutos para manter uma conexão de streaming aberta.</span><span class="sxs-lookup"><span data-stu-id="bd14d-120">The text value represents an integer that describes the maximum number of minutes to keep a streaming connection open.</span></span> <span data-ttu-id="bd14d-121">O valor deve estar entre 1 e 30, inclusive.</span><span class="sxs-lookup"><span data-stu-id="bd14d-121">The value must be between 1 and 30, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd14d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="bd14d-122">Remarks</span></span>

<span data-ttu-id="bd14d-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bd14d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd14d-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bd14d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd14d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="bd14d-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd14d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bd14d-126">Schema name</span></span>  <br/> |<span data-ttu-id="bd14d-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bd14d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd14d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bd14d-128">Validation file</span></span>  <br/> |<span data-ttu-id="bd14d-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bd14d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd14d-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bd14d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="bd14d-131">False</span><span class="sxs-lookup"><span data-stu-id="bd14d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd14d-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="bd14d-132">See also</span></span>



[<span data-ttu-id="bd14d-133">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="bd14d-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="bd14d-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bd14d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

