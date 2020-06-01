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
description: O elemento RecipientFilter representa um endereço de destinatário a ser usado com o relatório de acompanhamento de mensagens especificado.
ms.openlocfilehash: 945adf9155434e0690debfccc7caf70ba0cb94ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465804"
---
# <a name="recipientfilter"></a><span data-ttu-id="96605-103">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="96605-103">RecipientFilter</span></span>

<span data-ttu-id="96605-104">O elemento **RecipientFilter** representa um endereço de destinatário a ser usado com o relatório de acompanhamento de mensagens especificado.</span><span class="sxs-lookup"><span data-stu-id="96605-104">The **RecipientFilter** element represents a recipient address to use with the specified message tracking report.</span></span> 
  
```XML
 <RecipientFilter>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientFilter>
```

 <span data-ttu-id="96605-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="96605-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96605-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="96605-106">Attributes and elements</span></span>

<span data-ttu-id="96605-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96605-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96605-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="96605-108">Attributes</span></span>

<span data-ttu-id="96605-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96605-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96605-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96605-110">Child elements</span></span>

|<span data-ttu-id="96605-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96605-111">**Element**</span></span>|<span data-ttu-id="96605-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96605-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96605-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="96605-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="96605-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="96605-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="96605-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="96605-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="96605-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="96605-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="96605-117">Define o endereço SMTP (Simple Mail Transfer Protocol) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="96605-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="96605-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="96605-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="96605-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="96605-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="96605-120">Representa o protocolo de roteamento para este destinatário.</span><span class="sxs-lookup"><span data-stu-id="96605-120">Represents the routing protocol for this recipient.</span></span> <span data-ttu-id="96605-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="96605-121">The default value is SMTP.</span></span> <span data-ttu-id="96605-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="96605-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="96605-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="96605-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="96605-124">Representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="96605-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="96605-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="96605-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="96605-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="96605-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="96605-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="96605-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="96605-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="96605-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96605-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96605-129">Parent elements</span></span>

|<span data-ttu-id="96605-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96605-130">**Element**</span></span>|<span data-ttu-id="96605-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96605-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96605-132">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="96605-132">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="96605-133">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) para recuperar o relatório de acompanhamento de mensagens completo da ID especificada.</span><span class="sxs-lookup"><span data-stu-id="96605-133">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96605-134">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="96605-134">Text value</span></span>

<span data-ttu-id="96605-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96605-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96605-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="96605-136">Remarks</span></span>

<span data-ttu-id="96605-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="96605-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96605-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="96605-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96605-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="96605-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96605-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96605-140">Schema Name</span></span>  <br/> |<span data-ttu-id="96605-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="96605-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96605-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96605-142">Validation File</span></span>  <br/> |<span data-ttu-id="96605-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96605-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96605-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96605-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="96605-145">False</span><span class="sxs-lookup"><span data-stu-id="96605-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96605-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="96605-146">See also</span></span>



[<span data-ttu-id="96605-147">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="96605-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="96605-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96605-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

