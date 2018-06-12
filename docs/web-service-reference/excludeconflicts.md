---
title: ExcludeConflicts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExcludeConflicts
api_type:
- schema
ms.assetid: ec33ef23-8537-41eb-8d89-7eb906a1fad7
description: O elemento ExcludeConflicts Especifica se é necessário retornar sugerido horários de horas do calendário que estão em conflito entre os participantes.
ms.openlocfilehash: 66b69d57246942e551de2f683949870823e2e4e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752128"
---
# <a name="excludeconflicts"></a><span data-ttu-id="6ce04-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="6ce04-103">ExcludeConflicts</span></span>

<span data-ttu-id="6ce04-104">O elemento **ExcludeConflicts** Especifica se é necessário retornar sugerido horários de horas do calendário que estão em conflito entre os participantes.</span><span class="sxs-lookup"><span data-stu-id="6ce04-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="6ce04-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6ce04-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="6ce04-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="6ce04-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="6ce04-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="6ce04-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="6ce04-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="6ce04-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="6ce04-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6ce04-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ce04-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6ce04-110">Attributes and elements</span></span>

<span data-ttu-id="6ce04-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6ce04-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ce04-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6ce04-112">Attributes</span></span>

<span data-ttu-id="6ce04-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6ce04-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ce04-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6ce04-114">Child elements</span></span>

<span data-ttu-id="6ce04-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6ce04-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ce04-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6ce04-116">Parent elements</span></span>

|<span data-ttu-id="6ce04-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6ce04-117">**Element**</span></span>|<span data-ttu-id="6ce04-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ce04-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ce04-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="6ce04-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="6ce04-120">Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ce04-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="6ce04-121">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="6ce04-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ce04-122">Text value</span><span class="sxs-lookup"><span data-stu-id="6ce04-122">Text value</span></span>

<span data-ttu-id="6ce04-123">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="6ce04-123">A text value is required.</span></span> <span data-ttu-id="6ce04-124">Os valores possíveis são um booleano **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="6ce04-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ce04-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="6ce04-125">Remarks</span></span>

<span data-ttu-id="6ce04-126">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ce04-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6ce04-127">O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6ce04-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6ce04-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6ce04-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ce04-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ce04-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ce04-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6ce04-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6ce04-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6ce04-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ce04-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6ce04-132">Validation File</span></span>  <br/> |<span data-ttu-id="6ce04-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6ce04-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ce04-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6ce04-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ce04-135">False</span><span class="sxs-lookup"><span data-stu-id="6ce04-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ce04-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="6ce04-136">See also</span></span>



[<span data-ttu-id="6ce04-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6ce04-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6ce04-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6ce04-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="6ce04-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="6ce04-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

