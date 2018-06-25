---
title: EndWallClock
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: O elemento EndWallClock Especifica a hora de término de uma reunião no fuso horário do local em que a reunião ocorre.
ms.openlocfilehash: 10e4a2bde50354b2f2752751c01a6a70aa084d05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752066"
---
# <a name="endwallclock"></a><span data-ttu-id="d2e76-103">EndWallClock</span><span class="sxs-lookup"><span data-stu-id="d2e76-103">EndWallClock</span></span>

<span data-ttu-id="d2e76-104">O elemento **EndWallClock** Especifica a hora de término de uma reunião no fuso horário do local em que a reunião ocorre.</span><span class="sxs-lookup"><span data-stu-id="d2e76-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="d2e76-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d2e76-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2e76-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d2e76-106">Attributes and elements</span></span>

<span data-ttu-id="d2e76-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2e76-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2e76-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2e76-108">Attributes</span></span>

<span data-ttu-id="d2e76-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2e76-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2e76-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2e76-110">Child elements</span></span>

<span data-ttu-id="d2e76-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2e76-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2e76-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2e76-112">Parent elements</span></span>

|<span data-ttu-id="d2e76-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2e76-113">**Element**</span></span>|<span data-ttu-id="d2e76-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2e76-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2e76-115">Pessoa</span><span class="sxs-lookup"><span data-stu-id="d2e76-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d2e76-116">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d2e76-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2e76-117">Text value</span><span class="sxs-lookup"><span data-stu-id="d2e76-117">Text value</span></span>

<span data-ttu-id="d2e76-118">O valor de texto do elemento **EndWallClock** é um valor string que especifica o identificador do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="d2e76-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d2e76-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="d2e76-119">Remarks</span></span>

<span data-ttu-id="d2e76-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2e76-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2e76-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2e76-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2e76-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d2e76-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2e76-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2e76-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2e76-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d2e76-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d2e76-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="d2e76-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="d2e76-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d2e76-126">Validation File</span></span>  <br/> |<span data-ttu-id="d2e76-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2e76-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2e76-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d2e76-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2e76-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="d2e76-129">See also</span></span>



- [<span data-ttu-id="d2e76-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d2e76-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

