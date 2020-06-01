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
ms.openlocfilehash: e020ff07f271bdde6c2a4172141097dcba66f64e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465090"
---
# <a name="rootaddress"></a><span data-ttu-id="f066d-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="f066d-103">RootAddress</span></span>

<span data-ttu-id="f066d-104">O elemento **RootAddress** representa o primeiro endereço que inicia o evento para um evento [RecipientTrackingEvent](recipienttrackingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="f066d-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="f066d-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="f066d-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f066d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f066d-106">Attributes and elements</span></span>

<span data-ttu-id="f066d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f066d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f066d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f066d-108">Attributes</span></span>

<span data-ttu-id="f066d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f066d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f066d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f066d-110">Child elements</span></span>

<span data-ttu-id="f066d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f066d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f066d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f066d-112">Parent elements</span></span>

|<span data-ttu-id="f066d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f066d-113">**Element**</span></span>|<span data-ttu-id="f066d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f066d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f066d-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="f066d-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="f066d-116">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="f066d-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f066d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f066d-117">Text value</span></span>

<span data-ttu-id="f066d-118">O valor de texto é o endereço que inicia o evento de controle.</span><span class="sxs-lookup"><span data-stu-id="f066d-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f066d-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="f066d-119">Remarks</span></span>

<span data-ttu-id="f066d-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f066d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f066d-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f066d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f066d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="f066d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f066d-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f066d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f066d-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f066d-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f066d-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f066d-125">Validation File</span></span>  <br/> |<span data-ttu-id="f066d-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f066d-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f066d-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f066d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f066d-128">False</span><span class="sxs-lookup"><span data-stu-id="f066d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f066d-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="f066d-129">See also</span></span>



[<span data-ttu-id="f066d-130">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f066d-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f066d-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f066d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

