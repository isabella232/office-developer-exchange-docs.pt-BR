---
title: MailboxData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxData
api_type:
- schema
ms.assetid: e9e3f50c-5a7b-49c7-a9ea-117959c08352
description: O elemento MailboxData representa um usuário da caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.
ms.openlocfilehash: df60294e7d83b1459e5cca7d75c2b6b4bb9d931d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824281"
---
# <a name="mailboxdata"></a><span data-ttu-id="4225d-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="4225d-103">MailboxData</span></span>

<span data-ttu-id="4225d-104">O elemento **MailboxData** representa um usuário da caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4225d-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="4225d-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4225d-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="4225d-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="4225d-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="4225d-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="4225d-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="4225d-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="4225d-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4225d-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4225d-109">Attributes and elements</span></span>

<span data-ttu-id="4225d-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4225d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4225d-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="4225d-111">Attributes</span></span>

<span data-ttu-id="4225d-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4225d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4225d-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4225d-113">Child elements</span></span>

|<span data-ttu-id="4225d-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4225d-114">**Element**</span></span>|<span data-ttu-id="4225d-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4225d-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4225d-116">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4225d-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="4225d-117">Representa o usuário de caixa de correio para uma consulta GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="4225d-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="4225d-118">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="4225d-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="4225d-119">Representa o tipo do attendee identificado no elemento de [Email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="4225d-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="4225d-120">Isso é usado nas solicitações para sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="4225d-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="4225d-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="4225d-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="4225d-122">Especifica se é necessário retornar sugerido horários de horas do calendário que estão em conflito entre os participantes.</span><span class="sxs-lookup"><span data-stu-id="4225d-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4225d-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4225d-123">Parent elements</span></span>

|<span data-ttu-id="4225d-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4225d-124">**Element**</span></span>|<span data-ttu-id="4225d-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4225d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4225d-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="4225d-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="4225d-127">Contém uma lista de caixas de correio para consultar informações sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="4225d-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="4225d-128">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="4225d-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4225d-129">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4225d-129">Remarks</span></span>

<span data-ttu-id="4225d-130">Um aplicativo cliente poderá defini-la para muitos elementos **MailboxData** .</span><span class="sxs-lookup"><span data-stu-id="4225d-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4225d-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4225d-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="4225d-132">Example</span><span class="sxs-lookup"><span data-stu-id="4225d-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <Email>
      <Name></Name>
      <Address>someone@ExServer.example.com</Address>
      <RoutingType>SMTP</RoutingType>
    </Email>
    <AttendeeType>Organizer</AttendeeType>
    <ExcludeConflicts>false</ExcludeConflicts>
  </MailboxData>
</MailboxDataArray>
```

## <a name="element-information"></a><span data-ttu-id="4225d-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4225d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4225d-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="4225d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4225d-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4225d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="4225d-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4225d-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="4225d-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4225d-137">Validation File</span></span>  <br/> |<span data-ttu-id="4225d-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4225d-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4225d-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4225d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="4225d-140">False</span><span class="sxs-lookup"><span data-stu-id="4225d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4225d-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="4225d-141">See also</span></span>

- [<span data-ttu-id="4225d-142">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4225d-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="4225d-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4225d-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="4225d-144">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="4225d-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

