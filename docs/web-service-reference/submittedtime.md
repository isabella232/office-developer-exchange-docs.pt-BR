---
title: SubmittedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmittedTime
api_type:
- schema
ms.assetid: 45c8fa36-c539-42ca-99dc-1ac33cc54afc
description: O elemento SubmittedTime representa o tempo que a mensagem inserida no servidor.
ms.openlocfilehash: 89fc6400914495b8f1bd3994f17421d0ab079460
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825613"
---
# <a name="submittedtime"></a><span data-ttu-id="99ed8-103">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="99ed8-103">SubmittedTime</span></span>

<span data-ttu-id="99ed8-104">O elemento **SubmittedTime** representa o tempo que a mensagem inserida no servidor.</span><span class="sxs-lookup"><span data-stu-id="99ed8-104">The **SubmittedTime** element represents the time that the message entered the server.</span></span> 
  
```XML
<SubmittedTime/>
```

 <span data-ttu-id="99ed8-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="99ed8-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99ed8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="99ed8-106">Attributes and elements</span></span>

<span data-ttu-id="99ed8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="99ed8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99ed8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="99ed8-108">Attributes</span></span>

<span data-ttu-id="99ed8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="99ed8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99ed8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="99ed8-110">Child elements</span></span>

<span data-ttu-id="99ed8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="99ed8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99ed8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="99ed8-112">Parent elements</span></span>

|<span data-ttu-id="99ed8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="99ed8-113">**Element**</span></span>|<span data-ttu-id="99ed8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99ed8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99ed8-115">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="99ed8-115">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="99ed8-116">Contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="99ed8-116">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99ed8-117">Text value</span><span class="sxs-lookup"><span data-stu-id="99ed8-117">Text value</span></span>

 <span data-ttu-id="99ed8-118">Se este elemento for usado, será necessário um valor de texto que representa um valor de data/hora.</span><span class="sxs-lookup"><span data-stu-id="99ed8-118">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="99ed8-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="99ed8-119">Remarks</span></span>

<span data-ttu-id="99ed8-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="99ed8-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99ed8-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="99ed8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99ed8-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="99ed8-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99ed8-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="99ed8-123">Schema Name</span></span>  <br/> |<span data-ttu-id="99ed8-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="99ed8-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="99ed8-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="99ed8-125">Validation File</span></span>  <br/> |<span data-ttu-id="99ed8-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="99ed8-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99ed8-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="99ed8-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="99ed8-128">False</span><span class="sxs-lookup"><span data-stu-id="99ed8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99ed8-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="99ed8-129">See also</span></span>



- [<span data-ttu-id="99ed8-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="99ed8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

