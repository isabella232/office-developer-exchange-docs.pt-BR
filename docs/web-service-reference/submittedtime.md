---
title: Remetitime
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
description: O elemento remetitime representa a hora em que a mensagem entrou no servidor.
ms.openlocfilehash: bf9495aa700d2887d199eccb38289e0ebd2e8636
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465405"
---
# <a name="submittedtime"></a><span data-ttu-id="863e0-103">Remetitime</span><span class="sxs-lookup"><span data-stu-id="863e0-103">SubmittedTime</span></span>

<span data-ttu-id="863e0-104">O elemento **Remetitime** representa a hora em que a mensagem entrou no servidor.</span><span class="sxs-lookup"><span data-stu-id="863e0-104">The **SubmittedTime** element represents the time that the message entered the server.</span></span> 
  
```XML
<SubmittedTime/>
```

 <span data-ttu-id="863e0-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="863e0-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="863e0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="863e0-106">Attributes and elements</span></span>

<span data-ttu-id="863e0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="863e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="863e0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="863e0-108">Attributes</span></span>

<span data-ttu-id="863e0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="863e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="863e0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="863e0-110">Child elements</span></span>

<span data-ttu-id="863e0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="863e0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="863e0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="863e0-112">Parent elements</span></span>

|<span data-ttu-id="863e0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="863e0-113">**Element**</span></span>|<span data-ttu-id="863e0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="863e0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="863e0-115">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="863e0-115">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="863e0-116">Contém um único resultado de mensagem para um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="863e0-116">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="863e0-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="863e0-117">Text value</span></span>

 <span data-ttu-id="863e0-118">Um valor de texto que representa uma data/hora será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="863e0-118">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="863e0-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="863e0-119">Remarks</span></span>

<span data-ttu-id="863e0-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="863e0-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="863e0-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="863e0-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="863e0-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="863e0-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="863e0-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="863e0-123">Schema Name</span></span>  <br/> |<span data-ttu-id="863e0-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="863e0-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="863e0-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="863e0-125">Validation File</span></span>  <br/> |<span data-ttu-id="863e0-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="863e0-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="863e0-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="863e0-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="863e0-128">False</span><span class="sxs-lookup"><span data-stu-id="863e0-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="863e0-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="863e0-129">See also</span></span>



- [<span data-ttu-id="863e0-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="863e0-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

