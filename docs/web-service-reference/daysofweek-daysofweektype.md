---
title: DaysOfWeek (DaysOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: c56f997d-28f3-4590-97b0-cb71f016dbe4
description: O elemento DaysOfWeek descreve os dias da semana usados nos padrões de recorrência do item.
ms.openlocfilehash: 3036cbe3f93ff87b9a4d5dc7bf164e3e952b06fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463717"
---
# <a name="daysofweek-daysofweektype"></a><span data-ttu-id="ce508-103">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="ce508-103">DaysOfWeek (DaysOfWeekType)</span></span>

<span data-ttu-id="ce508-104">O elemento **DaysOfWeek** descreve os dias da semana usados nos padrões de recorrência do item.</span><span class="sxs-lookup"><span data-stu-id="ce508-104">The **DaysOfWeek** element describes days of the week that are used in item recurrence patterns.</span></span> 
  
```XML
<DaysOfWeek/>
```

<span data-ttu-id="ce508-105">**DaysOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="ce508-105">**DaysOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ce508-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ce508-106">Attributes and elements</span></span>

<span data-ttu-id="ce508-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ce508-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce508-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ce508-108">Attributes</span></span>

<span data-ttu-id="ce508-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce508-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce508-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ce508-110">Child elements</span></span>

<span data-ttu-id="ce508-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ce508-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce508-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ce508-112">Parent elements</span></span>

|<span data-ttu-id="ce508-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ce508-113">**Element**</span></span>|<span data-ttu-id="ce508-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce508-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce508-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ce508-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="ce508-116">Descreve um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="ce508-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce508-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ce508-117">Text value</span></span>

<span data-ttu-id="ce508-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce508-118">A text value is required.</span></span> <span data-ttu-id="ce508-119">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="ce508-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="ce508-120">Domingo</span><span class="sxs-lookup"><span data-stu-id="ce508-120">Sunday</span></span>    
- <span data-ttu-id="ce508-121">Segunda-feira</span><span class="sxs-lookup"><span data-stu-id="ce508-121">Monday</span></span>    
- <span data-ttu-id="ce508-122">Terça-feira</span><span class="sxs-lookup"><span data-stu-id="ce508-122">Tuesday</span></span>    
- <span data-ttu-id="ce508-123">Quarta-feira</span><span class="sxs-lookup"><span data-stu-id="ce508-123">Wednesday</span></span>    
- <span data-ttu-id="ce508-124">Quinta-feira</span><span class="sxs-lookup"><span data-stu-id="ce508-124">Thursday</span></span>    
- <span data-ttu-id="ce508-125">Sexta-feira</span><span class="sxs-lookup"><span data-stu-id="ce508-125">Friday</span></span>    
- <span data-ttu-id="ce508-126">Sábado</span><span class="sxs-lookup"><span data-stu-id="ce508-126">Saturday</span></span>    
- <span data-ttu-id="ce508-127">Day (este valor não é válido para um padrão de recorrência semanal)</span><span class="sxs-lookup"><span data-stu-id="ce508-127">Day (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="ce508-128">WEEKDAY (este valor não é válido para um padrão de recorrência semanal)</span><span class="sxs-lookup"><span data-stu-id="ce508-128">Weekday (this value is not valid for a weekly recurrence pattern)</span></span>    
- <span data-ttu-id="ce508-129">WeekendDay (esse valor não é válido para um padrão de recorrência semanal)</span><span class="sxs-lookup"><span data-stu-id="ce508-129">WeekendDay (this value is not valid for a weekly recurrence pattern)</span></span>
    
<span data-ttu-id="ce508-130">Um padrão de recorrência semanal pode conter vários valores.</span><span class="sxs-lookup"><span data-stu-id="ce508-130">A weekly recurrence pattern can contain multiple values.</span></span> <span data-ttu-id="ce508-131">Os valores são separados por um caractere de espaço.</span><span class="sxs-lookup"><span data-stu-id="ce508-131">Values are separated by a space character.</span></span> <span data-ttu-id="ce508-132">Por exemplo, para uma recorrência semanal em terças e quinta-feira, o valor de texto será "terça-feira".</span><span class="sxs-lookup"><span data-stu-id="ce508-132">For example, for a weekly recurrence on Tuesdays and Thursdays, the text value will be "Tuesday Thursday".</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce508-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="ce508-133">Remarks</span></span>

<span data-ttu-id="ce508-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ce508-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce508-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ce508-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce508-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="ce508-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce508-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ce508-137">Schema Name</span></span>  <br/> |<span data-ttu-id="ce508-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ce508-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce508-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ce508-139">Validation File</span></span>  <br/> |<span data-ttu-id="ce508-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ce508-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce508-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ce508-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce508-142">False</span><span class="sxs-lookup"><span data-stu-id="ce508-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce508-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="ce508-143">See also</span></span>

- [<span data-ttu-id="ce508-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce508-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

