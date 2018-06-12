---
title: FederatedDeliveryMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FederatedDeliveryMailbox
api_type:
- schema
ms.assetid: cd56bcc0-d24a-4e8b-87bd-999bf69234b7
description: O elemento FederatedDeliveryMailbox representa a caixa de correio ao qual uma mensagem entre local foi enviada.
ms.openlocfilehash: 4a9250455f8de3ede25f2b5ba9433690137ca1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752235"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="d0b4f-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="d0b4f-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="d0b4f-104">O elemento **FederatedDeliveryMailbox** representa a caixa de correio ao qual uma mensagem entre local foi enviada.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="d0b4f-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0b4f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d0b4f-106">Attributes and elements</span></span>

<span data-ttu-id="d0b4f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0b4f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d0b4f-108">Attributes</span></span>

<span data-ttu-id="d0b4f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0b4f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d0b4f-110">Child elements</span></span>

|<span data-ttu-id="d0b4f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-111">**Element**</span></span>|<span data-ttu-id="d0b4f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0b4f-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="d0b4f-114">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="d0b4f-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="d0b4f-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="d0b4f-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="d0b4f-120">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="d0b4f-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-121">The default is SMTP.</span></span> <span data-ttu-id="d0b4f-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="d0b4f-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="d0b4f-124">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="d0b4f-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="d0b4f-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d0b4f-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="d0b4f-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0b4f-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d0b4f-129">Parent elements</span></span>

|<span data-ttu-id="d0b4f-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-130">**Element**</span></span>|<span data-ttu-id="d0b4f-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0b4f-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="d0b4f-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="d0b4f-133">Contém os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0b4f-134">Text value</span><span class="sxs-lookup"><span data-stu-id="d0b4f-134">Text value</span></span>

<span data-ttu-id="d0b4f-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0b4f-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="d0b4f-136">Remarks</span></span>

<span data-ttu-id="d0b4f-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0b4f-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0b4f-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d0b4f-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0b4f-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0b4f-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0b4f-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d0b4f-140">Schema Name</span></span>  <br/> |<span data-ttu-id="d0b4f-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d0b4f-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0b4f-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d0b4f-142">Validation File</span></span>  <br/> |<span data-ttu-id="d0b4f-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0b4f-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0b4f-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d0b4f-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0b4f-145">False</span><span class="sxs-lookup"><span data-stu-id="d0b4f-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0b4f-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="d0b4f-146">See also</span></span>



- [<span data-ttu-id="d0b4f-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0b4f-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

