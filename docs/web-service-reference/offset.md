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
description: O elemento offset descreve o deslocamento do BaseOffset. Junto com o elemento BaseOffset, o elemento offset identifica se o horário é padrão ou horário de verão.
ms.openlocfilehash: 74ad87026c2cb89f3b0c35218c91f81380029963
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459753"
---
# <a name="offset"></a><span data-ttu-id="e3e58-104">Deslocamento</span><span class="sxs-lookup"><span data-stu-id="e3e58-104">Offset</span></span>

<span data-ttu-id="e3e58-105">O elemento **offset** descreve o deslocamento do [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="e3e58-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="e3e58-106">Junto com o elemento **BaseOffset** , o elemento **offset** identifica se o horário é padrão ou horário de verão.</span><span class="sxs-lookup"><span data-stu-id="e3e58-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="e3e58-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="e3e58-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3e58-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e3e58-108">Attributes and elements</span></span>

<span data-ttu-id="e3e58-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e3e58-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3e58-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e3e58-110">Attributes</span></span>

<span data-ttu-id="e3e58-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3e58-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3e58-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e3e58-112">Child elements</span></span>

<span data-ttu-id="e3e58-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e3e58-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e3e58-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e3e58-114">Parent elements</span></span>

|<span data-ttu-id="e3e58-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3e58-115">**Element**</span></span>|<span data-ttu-id="e3e58-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3e58-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3e58-117">Norte</span><span class="sxs-lookup"><span data-stu-id="e3e58-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="e3e58-118">Representa a data e a hora em que o horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="e3e58-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="e3e58-119">Standard</span><span class="sxs-lookup"><span data-stu-id="e3e58-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="e3e58-120">Representa a data e a hora em que o horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="e3e58-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3e58-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e3e58-121">Text value</span></span>

<span data-ttu-id="e3e58-122">O valor de texto representa o deslocamento do tempo universal coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="e3e58-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3e58-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="e3e58-123">Remarks</span></span>

<span data-ttu-id="e3e58-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e3e58-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3e58-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e3e58-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3e58-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3e58-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3e58-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e3e58-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e3e58-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e3e58-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3e58-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e3e58-129">Validation File</span></span>  <br/> |<span data-ttu-id="e3e58-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e3e58-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3e58-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e3e58-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3e58-132">False</span><span class="sxs-lookup"><span data-stu-id="e3e58-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3e58-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="e3e58-133">See also</span></span>



- [<span data-ttu-id="e3e58-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e3e58-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

