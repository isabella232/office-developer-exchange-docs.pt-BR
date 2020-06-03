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
description: O elemento MailboxData representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.
ms.openlocfilehash: bfcb8c01d40af81097c7d9868006fe9b7b5519d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467246"
---
# <a name="mailboxdata"></a><span data-ttu-id="cc034-103">MailboxData</span><span class="sxs-lookup"><span data-stu-id="cc034-103">MailboxData</span></span>

<span data-ttu-id="cc034-104">O elemento **MailboxData** representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cc034-104">The **MailboxData** element represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span> 
  
- [<span data-ttu-id="cc034-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="cc034-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="cc034-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="cc034-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="cc034-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="cc034-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxData>
   <Email>...</Email>
   <AttendeeType>...</AttendeeType>
   <ExcludeConflicts>...</ExcludeConflicts>
<MailboxData>
```

<span data-ttu-id="cc034-108">**MailboxData**</span><span class="sxs-lookup"><span data-stu-id="cc034-108">**MailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cc034-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cc034-109">Attributes and elements</span></span>

<span data-ttu-id="cc034-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cc034-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc034-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="cc034-111">Attributes</span></span>

<span data-ttu-id="cc034-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc034-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc034-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cc034-113">Child elements</span></span>

|<span data-ttu-id="cc034-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc034-114">**Element**</span></span>|<span data-ttu-id="cc034-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc034-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc034-116">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="cc034-116">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="cc034-117">Representa o usuário de caixa de correio de uma consulta GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="cc034-117">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> |
|[<span data-ttu-id="cc034-118">Articipantetype</span><span class="sxs-lookup"><span data-stu-id="cc034-118">AttendeeType</span></span>](attendeetype.md) <br/> |<span data-ttu-id="cc034-119">Representa o tipo de participante identificado no elemento [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="cc034-119">Represents the type of attendee identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="cc034-120">Isso é usado em solicitações de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="cc034-120">This is used in requests for meeting suggestions.</span></span>  <br/> |
|[<span data-ttu-id="cc034-121">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="cc034-121">ExcludeConflicts</span></span>](excludeconflicts.md) <br/> |<span data-ttu-id="cc034-122">Especifica se é para retornar horários sugeridos para os horários de calendário que entram em conflito entre os participantes.</span><span class="sxs-lookup"><span data-stu-id="cc034-122">Specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc034-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cc034-123">Parent elements</span></span>

|<span data-ttu-id="cc034-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc034-124">**Element**</span></span>|<span data-ttu-id="cc034-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc034-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc034-126">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="cc034-126">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="cc034-127">Contém uma lista de caixas de correio para consultar informações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc034-127">Contains a list of mailboxes to query for availability information.</span></span>  <br/> <span data-ttu-id="cc034-128">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="cc034-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc034-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="cc034-129">Remarks</span></span>

<span data-ttu-id="cc034-130">Um aplicativo cliente pode definir um para muitos elementos **MailboxData** .</span><span class="sxs-lookup"><span data-stu-id="cc034-130">A client application can define one to many **MailboxData** elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cc034-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cc034-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="cc034-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc034-132">Example</span></span>

```xml
<MailboxDataArray>
  <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="cc034-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cc034-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc034-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc034-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc034-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cc034-135">Schema Name</span></span>  <br/> |<span data-ttu-id="cc034-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cc034-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="cc034-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cc034-137">Validation File</span></span>  <br/> |<span data-ttu-id="cc034-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cc034-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc034-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cc034-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc034-140">False</span><span class="sxs-lookup"><span data-stu-id="cc034-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc034-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="cc034-141">See also</span></span>

- [<span data-ttu-id="cc034-142">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cc034-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="cc034-143">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="cc034-143">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="cc034-144">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="cc034-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

