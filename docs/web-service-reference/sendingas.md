---
title: SendingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendingAs
api_type:
- schema
ms.assetid: b43ce19f-9ab0-4946-acb2-c5aafead9d35
description: O elemento SendingAs representa um endereço de email que um usuário está tentando enviar como.
ms.openlocfilehash: a5468ddb8facf99038d319252f7e1c780a888ca1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825338"
---
# <a name="sendingas"></a><span data-ttu-id="60d87-103">SendingAs</span><span class="sxs-lookup"><span data-stu-id="60d87-103">SendingAs</span></span>

<span data-ttu-id="60d87-104">O elemento **SendingAs** representa um endereço de email que um usuário está tentando enviar como.</span><span class="sxs-lookup"><span data-stu-id="60d87-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="60d87-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="60d87-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60d87-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="60d87-106">Attributes and elements</span></span>

<span data-ttu-id="60d87-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="60d87-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60d87-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="60d87-108">Attributes</span></span>

<span data-ttu-id="60d87-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="60d87-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60d87-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="60d87-110">Child elements</span></span>

|<span data-ttu-id="60d87-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="60d87-111">**Element**</span></span>|<span data-ttu-id="60d87-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="60d87-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60d87-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="60d87-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="60d87-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="60d87-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="60d87-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="60d87-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="60d87-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="60d87-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="60d87-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="60d87-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="60d87-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="60d87-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="60d87-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="60d87-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="60d87-120">Define o tipo de endereço da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="60d87-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="60d87-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="60d87-121">The default is SMTP.</span></span> <span data-ttu-id="60d87-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="60d87-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="60d87-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="60d87-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="60d87-124">Representa o tipo de caixa de correio que é representado por um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="60d87-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="60d87-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="60d87-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="60d87-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="60d87-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="60d87-127">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="60d87-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="60d87-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="60d87-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60d87-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="60d87-129">Parent elements</span></span>

|<span data-ttu-id="60d87-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="60d87-130">**Element**</span></span>|<span data-ttu-id="60d87-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="60d87-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60d87-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="60d87-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="60d87-133">Contém os destinatários e os tipos de dicas de email para recuperar.</span><span class="sxs-lookup"><span data-stu-id="60d87-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60d87-134">Text value</span><span class="sxs-lookup"><span data-stu-id="60d87-134">Text value</span></span>

<span data-ttu-id="60d87-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="60d87-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60d87-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="60d87-136">Remarks</span></span>

<span data-ttu-id="60d87-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="60d87-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60d87-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="60d87-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60d87-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="60d87-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60d87-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="60d87-140">Schema Name</span></span>  <br/> |<span data-ttu-id="60d87-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="60d87-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60d87-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="60d87-142">Validation File</span></span>  <br/> |<span data-ttu-id="60d87-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="60d87-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60d87-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="60d87-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="60d87-145">False</span><span class="sxs-lookup"><span data-stu-id="60d87-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60d87-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="60d87-146">See also</span></span>



- [<span data-ttu-id="60d87-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="60d87-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

