---
title: DiagnosticsLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DiagnosticsLevel
api_type:
- schema
ms.assetid: 66794226-f5e0-44f0-8a0e-1f194bb0ba0f
description: O elemento DiagnosticsLevel representa informações de desempenho e de tempo que serão usadas para derivar o relatório.
ms.openlocfilehash: 9205625bb6cf38e370e29d96770eb293ed9277f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751798"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="593de-103">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="593de-103">DiagnosticsLevel</span></span>

<span data-ttu-id="593de-104">O elemento **DiagnosticsLevel** representa informações de desempenho e de tempo que serão usadas para derivar o relatório.</span><span class="sxs-lookup"><span data-stu-id="593de-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="593de-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="593de-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="593de-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="593de-106">Attributes and elements</span></span>

<span data-ttu-id="593de-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="593de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="593de-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="593de-108">Attributes</span></span>

<span data-ttu-id="593de-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="593de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="593de-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="593de-110">Child elements</span></span>

<span data-ttu-id="593de-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="593de-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="593de-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="593de-112">Parent elements</span></span>

|<span data-ttu-id="593de-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="593de-113">**Element**</span></span>|<span data-ttu-id="593de-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="593de-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="593de-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="593de-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="593de-116">Contém os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="593de-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="593de-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="593de-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="593de-118">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="593de-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="593de-119">Text value</span><span class="sxs-lookup"><span data-stu-id="593de-119">Text value</span></span>

<span data-ttu-id="593de-120">Se este elemento for usado, será necessário um valor de texto que representa uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="593de-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="593de-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="593de-121">Remarks</span></span>

<span data-ttu-id="593de-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="593de-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="593de-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="593de-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="593de-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="593de-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="593de-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="593de-125">Schema Name</span></span>  <br/> |<span data-ttu-id="593de-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="593de-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="593de-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="593de-127">Validation File</span></span>  <br/> |<span data-ttu-id="593de-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="593de-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="593de-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="593de-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="593de-130">False</span><span class="sxs-lookup"><span data-stu-id="593de-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="593de-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="593de-131">See also</span></span>

- [<span data-ttu-id="593de-132">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="593de-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="593de-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="593de-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

