---
title: SubmitTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: O elemento SubmitTime representa a hora em que a mensagem foi enviada para o servidor.
ms.openlocfilehash: 3f19e2ac14b412ef8d1ab59eb069f0223cf782ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825617"
---
# <a name="submittime"></a><span data-ttu-id="18bb6-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="18bb6-103">SubmitTime</span></span>

<span data-ttu-id="18bb6-104">O elemento **SubmitTime** representa a hora em que a mensagem foi enviada para o servidor.</span><span class="sxs-lookup"><span data-stu-id="18bb6-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="18bb6-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="18bb6-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18bb6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="18bb6-106">Attributes and elements</span></span>

<span data-ttu-id="18bb6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="18bb6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18bb6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="18bb6-108">Attributes</span></span>

<span data-ttu-id="18bb6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="18bb6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18bb6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="18bb6-110">Child elements</span></span>

<span data-ttu-id="18bb6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="18bb6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18bb6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="18bb6-112">Parent elements</span></span>

|<span data-ttu-id="18bb6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18bb6-113">**Element**</span></span>|<span data-ttu-id="18bb6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18bb6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18bb6-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="18bb6-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="18bb6-116">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="18bb6-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18bb6-117">Text value</span><span class="sxs-lookup"><span data-stu-id="18bb6-117">Text value</span></span>

<span data-ttu-id="18bb6-118">Se este elemento for usado, será necessário um valor de texto que representa um valor de data/hora.</span><span class="sxs-lookup"><span data-stu-id="18bb6-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18bb6-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="18bb6-119">Remarks</span></span>

<span data-ttu-id="18bb6-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="18bb6-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18bb6-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="18bb6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18bb6-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="18bb6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18bb6-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="18bb6-123">Schema Name</span></span>  <br/> |<span data-ttu-id="18bb6-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="18bb6-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="18bb6-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="18bb6-125">Validation File</span></span>  <br/> |<span data-ttu-id="18bb6-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18bb6-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18bb6-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="18bb6-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="18bb6-128">False</span><span class="sxs-lookup"><span data-stu-id="18bb6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18bb6-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="18bb6-129">See also</span></span>



[<span data-ttu-id="18bb6-130">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="18bb6-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="18bb6-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="18bb6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

