---
title: MessageTrackingReportId
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
description: O elemento MessageTrackingReportId representa a mensagem por sua ID de mensagem, a organização onde a mensagem foi encontrada, o servidor no qual a mensagem foi enviada e uma ID interna que identifica exclusivamente a mensagem.
ms.openlocfilehash: d6e92593d55608e260634602c2aab694804d716d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460593"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="70135-103">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="70135-103">MessageTrackingReportId</span></span>

<span data-ttu-id="70135-104">O elemento **MessageTrackingReportId** representa a mensagem por sua ID de mensagem, a organização onde a mensagem foi encontrada, o servidor no qual a mensagem foi enviada e uma ID interna que identifica exclusivamente a mensagem.</span><span class="sxs-lookup"><span data-stu-id="70135-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="70135-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="70135-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70135-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="70135-106">Attributes and elements</span></span>

<span data-ttu-id="70135-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70135-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70135-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="70135-108">Attributes</span></span>

<span data-ttu-id="70135-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70135-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70135-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70135-110">Child elements</span></span>

<span data-ttu-id="70135-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70135-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70135-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70135-112">Parent elements</span></span>

|<span data-ttu-id="70135-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70135-113">**Element**</span></span>|<span data-ttu-id="70135-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70135-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70135-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="70135-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="70135-116">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) para recuperar o relatório de acompanhamento de mensagens completo da ID especificada.</span><span class="sxs-lookup"><span data-stu-id="70135-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="70135-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="70135-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="70135-118">Contém um único resultado de mensagem para um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="70135-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70135-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="70135-119">Text value</span></span>

<span data-ttu-id="70135-120">Um valor de texto que representa uma cadeia de caracteres será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="70135-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70135-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="70135-121">Remarks</span></span>

<span data-ttu-id="70135-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="70135-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70135-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="70135-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70135-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="70135-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70135-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="70135-125">Schema Name</span></span>  <br/> |<span data-ttu-id="70135-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="70135-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="70135-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="70135-127">Validation File</span></span>  <br/> |<span data-ttu-id="70135-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="70135-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70135-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="70135-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="70135-130">False</span><span class="sxs-lookup"><span data-stu-id="70135-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70135-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="70135-131">See also</span></span>



[<span data-ttu-id="70135-132">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="70135-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="70135-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="70135-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

