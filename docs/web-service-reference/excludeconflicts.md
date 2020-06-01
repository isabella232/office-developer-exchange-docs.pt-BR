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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456973"
---
# <a name="excludeconflicts"></a><span data-ttu-id="37aaa-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="37aaa-103">ExcludeConflicts</span></span>

<span data-ttu-id="37aaa-104">O elemento **ExcludeConflicts** especifica se é para retornar horários sugeridos para os horários de calendário que entram em conflito entre os participantes.</span><span class="sxs-lookup"><span data-stu-id="37aaa-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="37aaa-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="37aaa-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="37aaa-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="37aaa-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="37aaa-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="37aaa-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="37aaa-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="37aaa-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="37aaa-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="37aaa-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37aaa-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="37aaa-110">Attributes and elements</span></span>

<span data-ttu-id="37aaa-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="37aaa-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37aaa-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="37aaa-112">Attributes</span></span>

<span data-ttu-id="37aaa-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37aaa-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37aaa-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="37aaa-114">Child elements</span></span>

<span data-ttu-id="37aaa-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="37aaa-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37aaa-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="37aaa-116">Parent elements</span></span>

|<span data-ttu-id="37aaa-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37aaa-117">**Element**</span></span>|<span data-ttu-id="37aaa-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37aaa-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37aaa-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="37aaa-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="37aaa-120">Representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="37aaa-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="37aaa-121">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="37aaa-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37aaa-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="37aaa-122">Text value</span></span>

<span data-ttu-id="37aaa-123">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37aaa-123">A text value is required.</span></span> <span data-ttu-id="37aaa-124">Os valores possíveis são Boolean **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="37aaa-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="37aaa-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="37aaa-125">Remarks</span></span>

<span data-ttu-id="37aaa-126">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37aaa-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="37aaa-127">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="37aaa-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="37aaa-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="37aaa-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37aaa-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="37aaa-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37aaa-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="37aaa-130">Schema Name</span></span>  <br/> |<span data-ttu-id="37aaa-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="37aaa-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="37aaa-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="37aaa-132">Validation File</span></span>  <br/> |<span data-ttu-id="37aaa-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="37aaa-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37aaa-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="37aaa-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="37aaa-135">False</span><span class="sxs-lookup"><span data-stu-id="37aaa-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37aaa-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="37aaa-136">See also</span></span>



[<span data-ttu-id="37aaa-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="37aaa-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="37aaa-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="37aaa-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="37aaa-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="37aaa-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

