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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752235"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="4fc13-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="4fc13-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="4fc13-104">O elemento **FederatedDeliveryMailbox** representa a caixa de correio ao qual uma mensagem entre local foi enviada.</span><span class="sxs-lookup"><span data-stu-id="4fc13-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="4fc13-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="4fc13-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fc13-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4fc13-106">Attributes and elements</span></span>

<span data-ttu-id="4fc13-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4fc13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fc13-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4fc13-108">Attributes</span></span>

<span data-ttu-id="4fc13-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4fc13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fc13-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4fc13-110">Child elements</span></span>

|<span data-ttu-id="4fc13-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fc13-111">**Element**</span></span>|<span data-ttu-id="4fc13-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fc13-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fc13-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4fc13-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="4fc13-114">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4fc13-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="4fc13-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="4fc13-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4fc13-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="4fc13-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="4fc13-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4fc13-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="4fc13-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="4fc13-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4fc13-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="4fc13-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="4fc13-120">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4fc13-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="4fc13-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="4fc13-121">The default is SMTP.</span></span> <span data-ttu-id="4fc13-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="4fc13-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4fc13-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="4fc13-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="4fc13-124">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4fc13-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="4fc13-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="4fc13-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4fc13-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="4fc13-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4fc13-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="4fc13-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="4fc13-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="4fc13-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fc13-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4fc13-129">Parent elements</span></span>

|<span data-ttu-id="4fc13-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fc13-130">**Element**</span></span>|<span data-ttu-id="4fc13-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fc13-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fc13-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="4fc13-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="4fc13-133">Contém os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="4fc13-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fc13-134">Text value</span><span class="sxs-lookup"><span data-stu-id="4fc13-134">Text value</span></span>

<span data-ttu-id="4fc13-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4fc13-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4fc13-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="4fc13-136">Remarks</span></span>

<span data-ttu-id="4fc13-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fc13-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fc13-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4fc13-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fc13-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="4fc13-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4fc13-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4fc13-140">Schema Name</span></span>  <br/> |<span data-ttu-id="4fc13-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4fc13-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4fc13-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4fc13-142">Validation File</span></span>  <br/> |<span data-ttu-id="4fc13-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4fc13-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4fc13-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4fc13-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fc13-145">False</span><span class="sxs-lookup"><span data-stu-id="4fc13-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fc13-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="4fc13-146">See also</span></span>



- [<span data-ttu-id="4fc13-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4fc13-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

