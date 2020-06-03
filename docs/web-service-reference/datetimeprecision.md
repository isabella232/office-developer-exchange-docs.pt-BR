---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: O elemento DateTimePrecision especifica a precisão dos valores de data/hora retornados.
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529221"
---
# <a name="datetimeprecision"></a><span data-ttu-id="30245-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="30245-103">DateTimePrecision</span></span>

<span data-ttu-id="30245-104">O elemento **DateTimePrecision** especifica a precisão dos valores de data/hora retornados.</span><span class="sxs-lookup"><span data-stu-id="30245-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="30245-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="30245-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="30245-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="30245-106">Attributes and elements</span></span>

<span data-ttu-id="30245-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30245-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30245-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30245-108">Attributes</span></span>

<span data-ttu-id="30245-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="30245-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30245-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30245-110">Child elements</span></span>

<span data-ttu-id="30245-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30245-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30245-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30245-112">Parent elements</span></span>

<span data-ttu-id="30245-113">O elemento **DateTimePrecision** está localizado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="30245-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="30245-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="30245-114">Text value</span></span>

<span data-ttu-id="30245-115">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30245-115">A text value is required.</span></span> <span data-ttu-id="30245-116">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="30245-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="30245-117">Segundos</span><span class="sxs-lookup"><span data-stu-id="30245-117">Seconds</span></span>
    
- <span data-ttu-id="30245-118">Milissegundos</span><span class="sxs-lookup"><span data-stu-id="30245-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="30245-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="30245-119">Remarks</span></span>

<span data-ttu-id="30245-120">Quando um cabeçalho SOAP com o elemento **DateTimePrecision** definido como "segundos" é usado, os valores de data/hora são retornados para os segundos mais próximos (00:00:00).</span><span class="sxs-lookup"><span data-stu-id="30245-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="30245-121">Quando "milissegundos" é usado, os valores de data/hora são retornados para o milissegundo mais próximo (00:00:00.0000).</span><span class="sxs-lookup"><span data-stu-id="30245-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="30245-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30245-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="30245-123">Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="30245-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30245-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="30245-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30245-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="30245-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30245-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30245-126">Schema Name</span></span>  <br/> |<span data-ttu-id="30245-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="30245-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="30245-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30245-128">Validation File</span></span>  <br/> |<span data-ttu-id="30245-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="30245-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30245-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="30245-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="30245-131">Falso</span><span class="sxs-lookup"><span data-stu-id="30245-131">False</span></span>  <br/> |
   

