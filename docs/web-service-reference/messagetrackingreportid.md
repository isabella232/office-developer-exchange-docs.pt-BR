---
title: Messagetrackingreportid deve ser passado
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: O elemento messagetrackingreportid deve ser passado representa a mensagem por sua ID de mensagem, a organização onde a mensagem foi encontrada, o servidor no qual a mensagem foi enviada e uma ID interna que identifica exclusivamente a mensagem.
ms.openlocfilehash: 8e0d85b203b8a34acedb5f6b9fe46359d5e0b97c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824456"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="fb2d2-103">Messagetrackingreportid deve ser passado</span><span class="sxs-lookup"><span data-stu-id="fb2d2-103">MessageTrackingReportId</span></span>

<span data-ttu-id="fb2d2-104">O elemento **messagetrackingreportid deve ser passado** representa a mensagem por sua ID de mensagem, a organização onde a mensagem foi encontrada, o servidor no qual a mensagem foi enviada e uma ID interna que identifica exclusivamente a mensagem.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="fb2d2-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="fb2d2-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb2d2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fb2d2-106">Attributes and elements</span></span>

<span data-ttu-id="fb2d2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb2d2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fb2d2-108">Attributes</span></span>

<span data-ttu-id="fb2d2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb2d2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fb2d2-110">Child elements</span></span>

<span data-ttu-id="fb2d2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb2d2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fb2d2-112">Parent elements</span></span>

|<span data-ttu-id="fb2d2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fb2d2-113">**Element**</span></span>|<span data-ttu-id="fb2d2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fb2d2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb2d2-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="fb2d2-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="fb2d2-116">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="fb2d2-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="fb2d2-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="fb2d2-118">Contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="fb2d2-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb2d2-119">Text value</span><span class="sxs-lookup"><span data-stu-id="fb2d2-119">Text value</span></span>

<span data-ttu-id="fb2d2-120">Se este elemento for usado, será necessário um valor de texto que representa uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb2d2-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="fb2d2-121">Remarks</span></span>

<span data-ttu-id="fb2d2-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb2d2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb2d2-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fb2d2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb2d2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb2d2-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb2d2-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fb2d2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fb2d2-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fb2d2-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb2d2-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fb2d2-127">Validation File</span></span>  <br/> |<span data-ttu-id="fb2d2-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb2d2-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb2d2-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fb2d2-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb2d2-130">False</span><span class="sxs-lookup"><span data-stu-id="fb2d2-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb2d2-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="fb2d2-131">See also</span></span>



[<span data-ttu-id="fb2d2-132">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="fb2d2-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="fb2d2-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fb2d2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

