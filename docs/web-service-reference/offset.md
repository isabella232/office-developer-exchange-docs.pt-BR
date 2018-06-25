---
title: Deslocamento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: O elemento de deslocamento descreve o deslocamento, desde o BaseOffset. Em conjunto com o elemento BaseOffset, o elemento de deslocamento identifica se o tempo é standard ou o horário de verão.
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824642"
---
# <a name="offset"></a><span data-ttu-id="6f8d5-104">Deslocamento</span><span class="sxs-lookup"><span data-stu-id="6f8d5-104">Offset</span></span>

<span data-ttu-id="6f8d5-105">O elemento de **deslocamento** descreve o deslocamento, desde o [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="6f8d5-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="6f8d5-106">Em conjunto com o elemento **BaseOffset** , o elemento de **deslocamento** identifica se o tempo é standard ou o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="6f8d5-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="6f8d5-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f8d5-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6f8d5-108">Attributes and elements</span></span>

<span data-ttu-id="6f8d5-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f8d5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6f8d5-110">Attributes</span></span>

<span data-ttu-id="6f8d5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f8d5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6f8d5-112">Child elements</span></span>

<span data-ttu-id="6f8d5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f8d5-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6f8d5-114">Parent elements</span></span>

|<span data-ttu-id="6f8d5-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f8d5-115">**Element**</span></span>|<span data-ttu-id="6f8d5-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f8d5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f8d5-117">Horário de verão</span><span class="sxs-lookup"><span data-stu-id="6f8d5-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="6f8d5-118">Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="6f8d5-119">Standard</span><span class="sxs-lookup"><span data-stu-id="6f8d5-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="6f8d5-120">Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6f8d5-121">Text value</span><span class="sxs-lookup"><span data-stu-id="6f8d5-121">Text value</span></span>

<span data-ttu-id="6f8d5-122">O valor de texto representa o deslocamento do tempo Universal Coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="6f8d5-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6f8d5-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="6f8d5-123">Remarks</span></span>

<span data-ttu-id="6f8d5-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6f8d5-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f8d5-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6f8d5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f8d5-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f8d5-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f8d5-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6f8d5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6f8d5-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6f8d5-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f8d5-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6f8d5-129">Validation File</span></span>  <br/> |<span data-ttu-id="6f8d5-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f8d5-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f8d5-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6f8d5-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f8d5-132">False</span><span class="sxs-lookup"><span data-stu-id="6f8d5-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f8d5-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="6f8d5-133">See also</span></span>



- [<span data-ttu-id="6f8d5-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6f8d5-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

