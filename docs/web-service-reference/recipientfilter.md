---
title: RecipientFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientFilter
api_type:
- schema
ms.assetid: 956c287a-a38a-49a7-a877-6d2088dfbc06
description: O elemento RecipientFilter representa um endereço de destinatário para usar com o relatório de controle de mensagens especificada.
ms.openlocfilehash: c31ed469132b110a690416b112d5e4e96e44c501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824972"
---
# <a name="recipientfilter"></a><span data-ttu-id="2e58b-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="2e58b-103">RecipientFilter</span></span>

<span data-ttu-id="2e58b-104">O elemento **RecipientFilter** representa um endereço de destinatário para usar com o relatório de controle de mensagens especificada.</span><span class="sxs-lookup"><span data-stu-id="2e58b-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="2e58b-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="2e58b-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e58b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2e58b-106">Attributes and elements</span></span>

<span data-ttu-id="2e58b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2e58b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e58b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2e58b-108">Attributes</span></span>

<span data-ttu-id="2e58b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e58b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e58b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2e58b-110">Child elements</span></span>

|<span data-ttu-id="2e58b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e58b-111">**Element**</span></span>|<span data-ttu-id="2e58b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e58b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e58b-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2e58b-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="2e58b-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2e58b-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="2e58b-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2e58b-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2e58b-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2e58b-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="2e58b-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2e58b-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="2e58b-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2e58b-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2e58b-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="2e58b-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="2e58b-120">Representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="2e58b-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="2e58b-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="2e58b-121">The default value is SMTP.</span></span> <span data-ttu-id="2e58b-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2e58b-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2e58b-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="2e58b-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="2e58b-124">Representa o tipo de caixa de correio que é representado por um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="2e58b-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="2e58b-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2e58b-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2e58b-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="2e58b-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2e58b-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e58b-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="2e58b-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2e58b-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e58b-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2e58b-129">Parent elements</span></span>

|<span data-ttu-id="2e58b-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e58b-130">**Element**</span></span>|<span data-ttu-id="2e58b-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e58b-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e58b-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2e58b-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="2e58b-133">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="2e58b-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2e58b-134">Text value</span><span class="sxs-lookup"><span data-stu-id="2e58b-134">Text value</span></span>

<span data-ttu-id="2e58b-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e58b-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2e58b-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e58b-136">Remarks</span></span>

<span data-ttu-id="2e58b-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e58b-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e58b-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2e58b-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e58b-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e58b-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2e58b-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2e58b-140">Schema Name</span></span>  <br/> |<span data-ttu-id="2e58b-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2e58b-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2e58b-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2e58b-142">Validation File</span></span>  <br/> |<span data-ttu-id="2e58b-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2e58b-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2e58b-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2e58b-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e58b-145">False</span><span class="sxs-lookup"><span data-stu-id="2e58b-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e58b-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="2e58b-146">See also</span></span>



[<span data-ttu-id="2e58b-147">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="2e58b-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="2e58b-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2e58b-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

