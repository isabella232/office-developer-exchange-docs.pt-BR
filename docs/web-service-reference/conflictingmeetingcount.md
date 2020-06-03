---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: O elemento ConflictingMeetingCount representa o número de reuniões que entram em conflito com o item do calendário.
ms.openlocfilehash: d53245e1b5d1f0182b28b15bf55ba9742bbb2a07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463857"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="0e782-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="0e782-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="0e782-104">O elemento **ConflictingMeetingCount** representa o número de reuniões que entram em conflito com o item do calendário.</span><span class="sxs-lookup"><span data-stu-id="0e782-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="0e782-105">**int**</span><span class="sxs-lookup"><span data-stu-id="0e782-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e782-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0e782-106">Attributes and elements</span></span>

<span data-ttu-id="0e782-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0e782-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e782-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0e782-108">Attributes</span></span>

<span data-ttu-id="0e782-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e782-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e782-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0e782-110">Child elements</span></span>

<span data-ttu-id="0e782-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e782-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e782-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0e782-112">Parent elements</span></span>

|<span data-ttu-id="0e782-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e782-113">**Element**</span></span>|<span data-ttu-id="0e782-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e782-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e782-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0e782-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0e782-116">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e782-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0e782-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0e782-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0e782-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e782-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e782-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0e782-119">Text value</span></span>

<span data-ttu-id="0e782-120">O valor de texto representa um inteiro.</span><span class="sxs-lookup"><span data-stu-id="0e782-120">The text value represents an integer.</span></span> <span data-ttu-id="0e782-121">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e782-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e782-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e782-122">Remarks</span></span>

<span data-ttu-id="0e782-123">Um item de calendário é considerado conflitante se ocorrer, pelo menos em parte, ao mesmo tempo que outro item de calendário na mesma pasta do calendário.</span><span class="sxs-lookup"><span data-stu-id="0e782-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="0e782-124">Se um item de calendário estiver em uma pasta que não seja de calendário, ele será comparado com os itens de calendário na pasta de calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="0e782-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="0e782-125">As solicitações de reunião são comparadas com os itens de calendário na pasta padrão calendário.</span><span class="sxs-lookup"><span data-stu-id="0e782-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="0e782-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0e782-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e782-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0e782-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e782-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e782-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e782-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0e782-129">Schema name</span></span>  <br/> |<span data-ttu-id="0e782-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0e782-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e782-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0e782-131">Validation file</span></span>  <br/> |<span data-ttu-id="0e782-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0e782-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e782-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0e782-133">Can be empty</span></span>  <br/> |<span data-ttu-id="0e782-134">False</span><span class="sxs-lookup"><span data-stu-id="0e782-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e782-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e782-135">See also</span></span>



- [<span data-ttu-id="0e782-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0e782-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

