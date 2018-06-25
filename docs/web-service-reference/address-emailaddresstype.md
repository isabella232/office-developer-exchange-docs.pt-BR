---
title: Endereço (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: 518641c8-7f6f-496c-86f9-341e7c1bb44c
description: O elemento de endereço representa um endereço de email totalmente resolvido.
ms.openlocfilehash: 2a2d409edcc3a04bf82c6da0080183becfc9b25b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751133"
---
# <a name="address-emailaddresstype"></a><span data-ttu-id="d70c4-103">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d70c4-103">Address (EmailAddressType)</span></span>

<span data-ttu-id="d70c4-104">O elemento de **endereço** representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="d70c4-104">The **Address** element represents a fully resolved e-mail address.</span></span> 
  
```XML
<Address>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Address >
```

 <span data-ttu-id="d70c4-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="d70c4-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d70c4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d70c4-106">Attributes and elements</span></span>

<span data-ttu-id="d70c4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d70c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d70c4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d70c4-108">Attributes</span></span>

<span data-ttu-id="d70c4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d70c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d70c4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d70c4-110">Child elements</span></span>

|<span data-ttu-id="d70c4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d70c4-111">**Element**</span></span>|<span data-ttu-id="d70c4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d70c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d70c4-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d70c4-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="d70c4-114">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d70c4-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="d70c4-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d70c4-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d70c4-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="d70c4-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="d70c4-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d70c4-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="d70c4-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d70c4-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d70c4-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d70c4-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="d70c4-120">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d70c4-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="d70c4-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="d70c4-121">The default is SMTP.</span></span> <span data-ttu-id="d70c4-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d70c4-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d70c4-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="d70c4-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="d70c4-124">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d70c4-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="d70c4-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d70c4-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d70c4-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="d70c4-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d70c4-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="d70c4-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="d70c4-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d70c4-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d70c4-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d70c4-129">Parent elements</span></span>

|<span data-ttu-id="d70c4-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d70c4-130">**Element**</span></span>|<span data-ttu-id="d70c4-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d70c4-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d70c4-132">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="d70c4-132">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="d70c4-133">Contém uma coleção de endereços de email que representam os destinatários originais de uma mensagem controlada.</span><span class="sxs-lookup"><span data-stu-id="d70c4-133">Contains a collection of e-mail addresses that represent the original recipients of a tracked message.</span></span>  <br/> |
|[<span data-ttu-id="d70c4-134">RoomLists</span><span class="sxs-lookup"><span data-stu-id="d70c4-134">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="d70c4-135">Contém uma lista de salas em uma organização de reunião.</span><span class="sxs-lookup"><span data-stu-id="d70c4-135">Contains a list of meeting rooms in an organization.</span></span>  <br/> |
|[<span data-ttu-id="d70c4-136">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="d70c4-136">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="d70c4-137">Contém uma lista de endereços de email que precisam foram enviadas em ordem para a condição ou exceção para aplicar a mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="d70c4-137">Contains a list of e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d70c4-138">Text value</span><span class="sxs-lookup"><span data-stu-id="d70c4-138">Text value</span></span>

<span data-ttu-id="d70c4-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d70c4-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d70c4-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="d70c4-140">Remarks</span></span>

<span data-ttu-id="d70c4-141">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d70c4-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d70c4-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d70c4-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d70c4-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="d70c4-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d70c4-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d70c4-144">Schema Name</span></span>  <br/> |<span data-ttu-id="d70c4-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d70c4-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="d70c4-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d70c4-146">Validation File</span></span>  <br/> |<span data-ttu-id="d70c4-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d70c4-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d70c4-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d70c4-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="d70c4-149">False</span><span class="sxs-lookup"><span data-stu-id="d70c4-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d70c4-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="d70c4-150">See also</span></span>

- [<span data-ttu-id="d70c4-151">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d70c4-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) 
- [<span data-ttu-id="d70c4-152">Operação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="d70c4-152">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="d70c4-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d70c4-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

