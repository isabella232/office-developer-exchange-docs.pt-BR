---
title: StartDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDateTime
api_type:
- schema
ms.assetid: 6fd41b7b-6c83-43b6-8b16-0bdb3d173d73
description: O elemento StartDateTime Especifica a data de início e a hora para uma regra ou uma pesquisa.
ms.openlocfilehash: 4bc32ed5626d692fc73dfa8bd7c46923aba72f9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825552"
---
# <a name="startdatetime"></a><span data-ttu-id="b7394-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="b7394-103">StartDateTime</span></span>

<span data-ttu-id="b7394-104">O elemento **StartDateTime** Especifica a data de início e a hora para uma regra ou uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b7394-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="b7394-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b7394-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b7394-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b7394-106">Attributes and elements</span></span>

<span data-ttu-id="b7394-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b7394-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7394-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b7394-108">Attributes</span></span>

<span data-ttu-id="b7394-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7394-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7394-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b7394-110">Child elements</span></span>

<span data-ttu-id="b7394-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7394-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7394-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b7394-112">Parent elements</span></span>

|<span data-ttu-id="b7394-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b7394-113">**Element**</span></span>|<span data-ttu-id="b7394-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b7394-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7394-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b7394-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b7394-116">Especifica os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="b7394-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="b7394-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b7394-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="b7394-118">Especifica o intervalo de datas dentro do qual as mensagens recebidas precisará foram recebidos em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="b7394-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7394-119">Text value</span><span class="sxs-lookup"><span data-stu-id="b7394-119">Text value</span></span>

 <span data-ttu-id="b7394-120">Se este elemento for usado, será necessário um valor de texto que representa um valor de data/hora.</span><span class="sxs-lookup"><span data-stu-id="b7394-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b7394-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="b7394-121">Remarks</span></span>

<span data-ttu-id="b7394-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7394-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7394-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b7394-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7394-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b7394-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7394-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b7394-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b7394-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b7394-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b7394-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b7394-127">Validation File</span></span>  <br/> |<span data-ttu-id="b7394-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b7394-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7394-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b7394-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7394-130">False</span><span class="sxs-lookup"><span data-stu-id="b7394-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7394-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="b7394-131">See also</span></span>

- [<span data-ttu-id="b7394-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b7394-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

