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
description: O elemento FederatedDeliveryMailbox representa a caixa de correio para a qual uma mensagem entre instalações foi enviada.
ms.openlocfilehash: d493ed81e82237b7257e8c469f4552d931b73aa6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461944"
---
# <a name="federateddeliverymailbox"></a><span data-ttu-id="089d5-103">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="089d5-103">FederatedDeliveryMailbox</span></span>

<span data-ttu-id="089d5-104">O elemento **FederatedDeliveryMailbox** representa a caixa de correio para a qual uma mensagem entre instalações foi enviada.</span><span class="sxs-lookup"><span data-stu-id="089d5-104">The **FederatedDeliveryMailbox** element represents the mailbox to which a cross-premise message was sent.</span></span> 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 <span data-ttu-id="089d5-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="089d5-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="089d5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="089d5-106">Attributes and elements</span></span>

<span data-ttu-id="089d5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="089d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="089d5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="089d5-108">Attributes</span></span>

<span data-ttu-id="089d5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="089d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="089d5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="089d5-110">Child elements</span></span>

|<span data-ttu-id="089d5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="089d5-111">**Element**</span></span>|<span data-ttu-id="089d5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="089d5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="089d5-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="089d5-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="089d5-114">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="089d5-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="089d5-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="089d5-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="089d5-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="089d5-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="089d5-117">Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="089d5-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="089d5-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="089d5-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="089d5-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="089d5-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="089d5-120">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="089d5-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="089d5-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="089d5-121">The default is SMTP.</span></span> <span data-ttu-id="089d5-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="089d5-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="089d5-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="089d5-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="089d5-124">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="089d5-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="089d5-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="089d5-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="089d5-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="089d5-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="089d5-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="089d5-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="089d5-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="089d5-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="089d5-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="089d5-129">Parent elements</span></span>

|<span data-ttu-id="089d5-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="089d5-130">**Element**</span></span>|<span data-ttu-id="089d5-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="089d5-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="089d5-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="089d5-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="089d5-133">Contém critérios para os tipos de mensagens a serem localizados.</span><span class="sxs-lookup"><span data-stu-id="089d5-133">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="089d5-134">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="089d5-134">Text value</span></span>

<span data-ttu-id="089d5-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="089d5-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="089d5-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="089d5-136">Remarks</span></span>

<span data-ttu-id="089d5-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="089d5-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="089d5-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="089d5-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="089d5-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="089d5-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="089d5-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="089d5-140">Schema Name</span></span>  <br/> |<span data-ttu-id="089d5-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="089d5-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="089d5-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="089d5-142">Validation File</span></span>  <br/> |<span data-ttu-id="089d5-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="089d5-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="089d5-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="089d5-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="089d5-145">False</span><span class="sxs-lookup"><span data-stu-id="089d5-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="089d5-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="089d5-146">See also</span></span>



- [<span data-ttu-id="089d5-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="089d5-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

