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
description: O elemento ExcludeConflicts especifica se é para retornar horários sugeridos para os horários de calendário que entram em conflito entre os participantes.
ms.openlocfilehash: d20c594ae600abf110681ea678b2d95a23bf7809
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456973"
---
# <a name="excludeconflicts"></a><span data-ttu-id="6c02a-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="6c02a-103">ExcludeConflicts</span></span>

<span data-ttu-id="6c02a-104">O elemento **ExcludeConflicts** especifica se é para retornar horários sugeridos para os horários de calendário que entram em conflito entre os participantes.</span><span class="sxs-lookup"><span data-stu-id="6c02a-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="6c02a-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6c02a-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="6c02a-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="6c02a-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="6c02a-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="6c02a-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="6c02a-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="6c02a-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="6c02a-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6c02a-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c02a-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6c02a-110">Attributes and elements</span></span>

<span data-ttu-id="6c02a-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6c02a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c02a-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6c02a-112">Attributes</span></span>

<span data-ttu-id="6c02a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c02a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c02a-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6c02a-114">Child elements</span></span>

<span data-ttu-id="6c02a-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6c02a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c02a-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6c02a-116">Parent elements</span></span>

|<span data-ttu-id="6c02a-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6c02a-117">**Element**</span></span>|<span data-ttu-id="6c02a-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6c02a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c02a-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="6c02a-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="6c02a-120">Representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c02a-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="6c02a-121">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="6c02a-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c02a-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6c02a-122">Text value</span></span>

<span data-ttu-id="6c02a-123">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c02a-123">A text value is required.</span></span> <span data-ttu-id="6c02a-124">Os valores possíveis são Boolean **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="6c02a-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c02a-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="6c02a-125">Remarks</span></span>

<span data-ttu-id="6c02a-126">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c02a-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6c02a-127">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6c02a-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6c02a-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6c02a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c02a-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c02a-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c02a-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6c02a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6c02a-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6c02a-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c02a-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6c02a-132">Validation File</span></span>  <br/> |<span data-ttu-id="6c02a-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6c02a-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c02a-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6c02a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c02a-135">False</span><span class="sxs-lookup"><span data-stu-id="6c02a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c02a-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="6c02a-136">See also</span></span>



[<span data-ttu-id="6c02a-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6c02a-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6c02a-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6c02a-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="6c02a-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="6c02a-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

