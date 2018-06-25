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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825617"
---
# <a name="submittime"></a><span data-ttu-id="517e0-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="517e0-103">SubmitTime</span></span>

<span data-ttu-id="517e0-104">O elemento **SubmitTime** representa a hora em que a mensagem foi enviada para o servidor.</span><span class="sxs-lookup"><span data-stu-id="517e0-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="517e0-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="517e0-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="517e0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="517e0-106">Attributes and elements</span></span>

<span data-ttu-id="517e0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="517e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="517e0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="517e0-108">Attributes</span></span>

<span data-ttu-id="517e0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="517e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="517e0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="517e0-110">Child elements</span></span>

<span data-ttu-id="517e0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="517e0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="517e0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="517e0-112">Parent elements</span></span>

|<span data-ttu-id="517e0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="517e0-113">**Element**</span></span>|<span data-ttu-id="517e0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="517e0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="517e0-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="517e0-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="517e0-116">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="517e0-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="517e0-117">Text value</span><span class="sxs-lookup"><span data-stu-id="517e0-117">Text value</span></span>

<span data-ttu-id="517e0-118">Se este elemento for usado, será necessário um valor de texto que representa um valor de data/hora.</span><span class="sxs-lookup"><span data-stu-id="517e0-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="517e0-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="517e0-119">Remarks</span></span>

<span data-ttu-id="517e0-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="517e0-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="517e0-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="517e0-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="517e0-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="517e0-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="517e0-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="517e0-123">Schema Name</span></span>  <br/> |<span data-ttu-id="517e0-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="517e0-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="517e0-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="517e0-125">Validation File</span></span>  <br/> |<span data-ttu-id="517e0-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="517e0-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="517e0-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="517e0-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="517e0-128">False</span><span class="sxs-lookup"><span data-stu-id="517e0-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="517e0-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="517e0-129">See also</span></span>



[<span data-ttu-id="517e0-130">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="517e0-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="517e0-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="517e0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

