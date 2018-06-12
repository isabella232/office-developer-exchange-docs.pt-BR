---
title: RootAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootAddress
api_type:
- schema
ms.assetid: 1dbb130a-e4eb-4baf-ae07-2568a8375bff
description: O elemento RootAddress representa o primeiro endereço que inicia o evento para um evento RecipientTrackingEvent.
ms.openlocfilehash: afe544d6ee8dea4cb416ad033ed2cd68976ec087
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825250"
---
# <a name="rootaddress"></a><span data-ttu-id="f2745-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="f2745-103">RootAddress</span></span>

<span data-ttu-id="f2745-104">O elemento **RootAddress** representa o primeiro endereço que inicia o evento para um evento [RecipientTrackingEvent](recipienttrackingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f2745-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="f2745-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="f2745-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2745-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f2745-106">Attributes and elements</span></span>

<span data-ttu-id="f2745-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f2745-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2745-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f2745-108">Attributes</span></span>

<span data-ttu-id="f2745-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f2745-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2745-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f2745-110">Child elements</span></span>

<span data-ttu-id="f2745-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f2745-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2745-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f2745-112">Parent elements</span></span>

|<span data-ttu-id="f2745-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f2745-113">**Element**</span></span>|<span data-ttu-id="f2745-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f2745-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2745-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="f2745-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="f2745-116">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="f2745-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2745-117">Text value</span><span class="sxs-lookup"><span data-stu-id="f2745-117">Text value</span></span>

<span data-ttu-id="f2745-118">O valor de texto é o endereço que inicia o evento de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="f2745-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2745-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f2745-119">Remarks</span></span>

<span data-ttu-id="f2745-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f2745-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2745-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f2745-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2745-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2745-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2745-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f2745-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f2745-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f2745-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2745-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f2745-125">Validation File</span></span>  <br/> |<span data-ttu-id="f2745-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2745-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2745-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f2745-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2745-128">False</span><span class="sxs-lookup"><span data-stu-id="f2745-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2745-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="f2745-129">See also</span></span>



[<span data-ttu-id="f2745-130">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f2745-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f2745-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f2745-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

