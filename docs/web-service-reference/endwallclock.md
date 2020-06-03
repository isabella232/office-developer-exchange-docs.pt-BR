---
title: EndWallClock
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc04e44e-e6d1-4355-a2b1-feb6663dc647
description: O elemento EndWallClock especifica a hora de término de uma reunião no fuso horário do local em que a reunião ocorre.
ms.openlocfilehash: 48b762d0bfe367b966b6f1790230f6a2118c3fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462968"
---
# <a name="endwallclock"></a><span data-ttu-id="8e7b5-103">EndWallClock</span><span class="sxs-lookup"><span data-stu-id="8e7b5-103">EndWallClock</span></span>

<span data-ttu-id="8e7b5-104">O elemento **EndWallClock** especifica a hora de término de uma reunião no fuso horário do local em que a reunião ocorre.</span><span class="sxs-lookup"><span data-stu-id="8e7b5-104">The **EndWallClock** element specifies the end time of a meeting in the time zone of the location in which the meeting takes place.</span></span> 
  
```XML
<EndWallClock></EndWallClock>
```

 <span data-ttu-id="8e7b5-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8e7b5-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e7b5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8e7b5-106">Attributes and elements</span></span>

<span data-ttu-id="8e7b5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8e7b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e7b5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8e7b5-108">Attributes</span></span>

<span data-ttu-id="8e7b5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e7b5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e7b5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8e7b5-110">Child elements</span></span>

<span data-ttu-id="8e7b5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8e7b5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e7b5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8e7b5-112">Parent elements</span></span>

|<span data-ttu-id="8e7b5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8e7b5-113">**Element**</span></span>|<span data-ttu-id="8e7b5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8e7b5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e7b5-115">Pessoal</span><span class="sxs-lookup"><span data-stu-id="8e7b5-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="8e7b5-116">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="8e7b5-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e7b5-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8e7b5-117">Text value</span></span>

<span data-ttu-id="8e7b5-118">O valor de texto do elemento **EndWallClock** é um valor String que especifica o identificador de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8e7b5-118">The text value of the **EndWallClock** element is a string value that specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8e7b5-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="8e7b5-119">Remarks</span></span>

<span data-ttu-id="8e7b5-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8e7b5-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8e7b5-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e7b5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e7b5-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8e7b5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e7b5-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e7b5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e7b5-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8e7b5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8e7b5-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="8e7b5-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="8e7b5-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8e7b5-126">Validation File</span></span>  <br/> |<span data-ttu-id="8e7b5-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8e7b5-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e7b5-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8e7b5-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8e7b5-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="8e7b5-129">See also</span></span>



- [<span data-ttu-id="8e7b5-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8e7b5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

