---
title: GetStreamingEventsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponse
api_type:
- schema
ms.assetid: ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2
description: O elemento GetStreamingEventsResponse representa uma resposta a uma solicitação de elemento GetStreamingEvents.
ms.openlocfilehash: 84cd4f0099ab0fda1c1fe771dca0d9ef932b132b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457722"
---
# <a name="getstreamingeventsresponse"></a><span data-ttu-id="55d24-103">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="55d24-103">GetStreamingEventsResponse</span></span>

<span data-ttu-id="55d24-104">O elemento **GetStreamingEventsResponse** representa uma resposta a uma solicitação de elemento [GetStreamingEvents](getstreamingevents.md) .</span><span class="sxs-lookup"><span data-stu-id="55d24-104">The **GetStreamingEventsResponse** element represents a response to a [GetStreamingEvents](getstreamingevents.md) element request.</span></span> 
  
```xml
<GetStreamingEventsResponse>
   <ResponseMessages/>
</GetStreamingEventsResponse>
```

 <span data-ttu-id="55d24-105">**GetStreamingEventsResponseType**</span><span class="sxs-lookup"><span data-stu-id="55d24-105">**GetStreamingEventsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55d24-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="55d24-106">Attributes and elements</span></span>

<span data-ttu-id="55d24-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="55d24-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55d24-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="55d24-108">Attributes</span></span>

<span data-ttu-id="55d24-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55d24-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55d24-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="55d24-110">Child elements</span></span>

|<span data-ttu-id="55d24-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55d24-111">**Element**</span></span>|<span data-ttu-id="55d24-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55d24-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55d24-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="55d24-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="55d24-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="55d24-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55d24-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="55d24-115">Parent elements</span></span>

<span data-ttu-id="55d24-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55d24-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="55d24-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="55d24-117">Text value</span></span>

<span data-ttu-id="55d24-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="55d24-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55d24-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="55d24-119">Remarks</span></span>

<span data-ttu-id="55d24-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="55d24-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55d24-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="55d24-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55d24-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="55d24-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55d24-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="55d24-123">Schema name</span></span>  <br/> |<span data-ttu-id="55d24-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="55d24-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55d24-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="55d24-125">Validation file</span></span>  <br/> |<span data-ttu-id="55d24-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="55d24-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55d24-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="55d24-127">Can be empty</span></span>  <br/> |<span data-ttu-id="55d24-128">False</span><span class="sxs-lookup"><span data-stu-id="55d24-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55d24-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="55d24-129">See also</span></span>



[<span data-ttu-id="55d24-130">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="55d24-130">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="55d24-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="55d24-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

