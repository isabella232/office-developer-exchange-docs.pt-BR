---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: O elemento DateTimePrecision Especifica a precisão para valores de data/hora retornado.
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751686"
---
# <a name="datetimeprecision"></a><span data-ttu-id="aede3-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="aede3-103">DateTimePrecision</span></span>

<span data-ttu-id="aede3-104">O elemento **DateTimePrecision** Especifica a precisão para valores de data/hora retornado.</span><span class="sxs-lookup"><span data-stu-id="aede3-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="aede3-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="aede3-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="aede3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aede3-106">Attributes and elements</span></span>

<span data-ttu-id="aede3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aede3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aede3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aede3-108">Attributes</span></span>

<span data-ttu-id="aede3-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="aede3-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aede3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aede3-110">Child elements</span></span>

<span data-ttu-id="aede3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aede3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aede3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aede3-112">Parent elements</span></span>

<span data-ttu-id="aede3-113">O elemento **DateTimePrecision** está localizado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="aede3-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="aede3-114">Text value</span><span class="sxs-lookup"><span data-stu-id="aede3-114">Text value</span></span>

<span data-ttu-id="aede3-115">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="aede3-115">A text value is required.</span></span> <span data-ttu-id="aede3-116">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="aede3-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="aede3-117">Segundos</span><span class="sxs-lookup"><span data-stu-id="aede3-117">Seconds</span></span>
    
- <span data-ttu-id="aede3-118">Milissegundos</span><span class="sxs-lookup"><span data-stu-id="aede3-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="aede3-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="aede3-119">Remarks</span></span>

<span data-ttu-id="aede3-120">Data/hora de quando um cabeçalho SOAP com o elemento **DateTimePrecision** definido como "Segundos" é usado, os valores são retornados para os mais próximo segundos (00: 00:00).</span><span class="sxs-lookup"><span data-stu-id="aede3-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="aede3-121">Data/hora de quando "Milissegundos" são usados, os valores são retornados para o milissegundo mais próximo (00:00:00.0000).</span><span class="sxs-lookup"><span data-stu-id="aede3-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="aede3-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aede3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="aede3-123">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="aede3-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aede3-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aede3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aede3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="aede3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aede3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aede3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="aede3-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aede3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="aede3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aede3-128">Validation File</span></span>  <br/> |<span data-ttu-id="aede3-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aede3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aede3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aede3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="aede3-131">False</span><span class="sxs-lookup"><span data-stu-id="aede3-131">False</span></span>  <br/> |
   

