---
title: IsOutOfDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOutOfDate
api_type:
- schema
ms.assetid: 2b6005a6-56a9-4848-b998-32908c13e2e2
description: O elemento IsOutOfDate indica se uma mensagem de reunião, solicitação, resposta ou cancelamento está desatualizado.
ms.openlocfilehash: 0a6b2670cc3eb260002821bab31d652177902de1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824110"
---
# <a name="isoutofdate"></a><span data-ttu-id="eccd3-103">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="eccd3-103">IsOutOfDate</span></span>

<span data-ttu-id="eccd3-104">O elemento **IsOutOfDate** indica se uma mensagem de reunião, solicitação, resposta ou cancelamento está desatualizado.</span><span class="sxs-lookup"><span data-stu-id="eccd3-104">The **IsOutOfDate** element indicates whether a meeting message, request, response, or cancellation is out-of-date.</span></span> 
  
```xml
<IsOutOfDate/>
```

 <span data-ttu-id="eccd3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="eccd3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eccd3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="eccd3-106">Attributes and elements</span></span>

<span data-ttu-id="eccd3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eccd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eccd3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="eccd3-108">Attributes</span></span>

<span data-ttu-id="eccd3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eccd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eccd3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eccd3-110">Child elements</span></span>

<span data-ttu-id="eccd3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eccd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eccd3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eccd3-112">Parent elements</span></span>

|<span data-ttu-id="eccd3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eccd3-113">**Element**</span></span>|<span data-ttu-id="eccd3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eccd3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eccd3-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="eccd3-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="eccd3-116">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eccd3-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="eccd3-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="eccd3-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="eccd3-118">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eccd3-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="eccd3-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="eccd3-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="eccd3-120">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eccd3-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="eccd3-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="eccd3-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="eccd3-122">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eccd3-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eccd3-123">Text value</span><span class="sxs-lookup"><span data-stu-id="eccd3-123">Text value</span></span>

<span data-ttu-id="eccd3-124">Um valor de texto de **true** indica que o item de reunião está desatualizado.</span><span class="sxs-lookup"><span data-stu-id="eccd3-124">A text value of **true** indicates that the meeting item is out-of-date.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="eccd3-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="eccd3-125">Remarks</span></span>

<span data-ttu-id="eccd3-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="eccd3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eccd3-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="eccd3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eccd3-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="eccd3-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eccd3-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eccd3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="eccd3-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eccd3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="eccd3-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eccd3-131">Validation File</span></span>  <br/> |<span data-ttu-id="eccd3-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eccd3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eccd3-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eccd3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="eccd3-134">False</span><span class="sxs-lookup"><span data-stu-id="eccd3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eccd3-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="eccd3-135">See also</span></span>



- [<span data-ttu-id="eccd3-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="eccd3-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

