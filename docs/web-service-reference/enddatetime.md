---
title: EndDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateTime
api_type:
- schema
ms.assetid: 54d14e47-a8f7-400b-a859-c7ea7ce4c6a4
description: O elemento EndDateTime Especifica a data de término e a hora para uma regra ou uma pesquisa.
ms.openlocfilehash: ad596c6441e7bdb10b4e886a8d0f3ba183c43c3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752061"
---
# <a name="enddatetime"></a><span data-ttu-id="cf8d2-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="cf8d2-103">EndDateTime</span></span>

<span data-ttu-id="cf8d2-104">O elemento **EndDateTime** Especifica a data de término e a hora para uma regra ou uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="cf8d2-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="cf8d2-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf8d2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cf8d2-106">Attributes and elements</span></span>

<span data-ttu-id="cf8d2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf8d2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf8d2-108">Attributes</span></span>

<span data-ttu-id="cf8d2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf8d2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf8d2-110">Child elements</span></span>

<span data-ttu-id="cf8d2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf8d2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf8d2-112">Parent elements</span></span>

|<span data-ttu-id="cf8d2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf8d2-113">**Element**</span></span>|<span data-ttu-id="cf8d2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf8d2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf8d2-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="cf8d2-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="cf8d2-116">Contém os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="cf8d2-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="cf8d2-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="cf8d2-118">Especifica o intervalo de datas dentro do qual as mensagens recebidas precisará foram recebidos em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf8d2-119">Text value</span><span class="sxs-lookup"><span data-stu-id="cf8d2-119">Text value</span></span>

<span data-ttu-id="cf8d2-120">Se este elemento for usado, será necessário um valor de texto que representa um valor de data/hora.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf8d2-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf8d2-121">Remarks</span></span>

<span data-ttu-id="cf8d2-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf8d2-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf8d2-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cf8d2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf8d2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf8d2-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cf8d2-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf8d2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cf8d2-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cf8d2-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cf8d2-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf8d2-127">Validation File</span></span>  <br/> |<span data-ttu-id="cf8d2-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf8d2-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf8d2-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf8d2-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf8d2-130">False</span><span class="sxs-lookup"><span data-stu-id="cf8d2-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf8d2-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="cf8d2-131">See also</span></span>



- [<span data-ttu-id="cf8d2-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cf8d2-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

