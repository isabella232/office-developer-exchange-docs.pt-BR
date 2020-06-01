---
title: Envios
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
description: O elemento sendas representa um endereço de email que um usuário está tentando enviar como.
ms.openlocfilehash: cd11bd60cbbe3434fcc1b0b9a1cfe0de9f0b1e21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462133"
---
# <a name="sendingas"></a><span data-ttu-id="032f1-103">Envios</span><span class="sxs-lookup"><span data-stu-id="032f1-103">SendingAs</span></span>

<span data-ttu-id="032f1-104">O elemento **sendas** representa um endereço de email que um usuário está tentando enviar como.</span><span class="sxs-lookup"><span data-stu-id="032f1-104">The **SendingAs** element represents an e-mail address that a user is trying to send as.</span></span> 
  
```XML
<SendingAs>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</SendingAs>
```

 <span data-ttu-id="032f1-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="032f1-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="032f1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="032f1-106">Attributes and elements</span></span>

<span data-ttu-id="032f1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="032f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="032f1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="032f1-108">Attributes</span></span>

<span data-ttu-id="032f1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="032f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="032f1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="032f1-110">Child elements</span></span>

|<span data-ttu-id="032f1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="032f1-111">**Element**</span></span>|<span data-ttu-id="032f1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="032f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="032f1-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="032f1-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="032f1-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="032f1-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="032f1-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="032f1-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="032f1-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="032f1-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="032f1-117">Define o endereço SMTP (Simple Mail Transfer Protocol) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="032f1-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="032f1-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="032f1-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="032f1-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="032f1-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="032f1-120">Define o tipo de endereço da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="032f1-120">Defines the address type for the mailbox.</span></span> <span data-ttu-id="032f1-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="032f1-121">The default is SMTP.</span></span> <span data-ttu-id="032f1-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="032f1-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="032f1-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="032f1-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="032f1-124">Representa o tipo de caixa de correio representada por um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="032f1-124">Represents the type of mailbox that is represented by an e-mail user.</span></span> <span data-ttu-id="032f1-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="032f1-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="032f1-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="032f1-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="032f1-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="032f1-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="032f1-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="032f1-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="032f1-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="032f1-129">Parent elements</span></span>

|<span data-ttu-id="032f1-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="032f1-130">**Element**</span></span>|<span data-ttu-id="032f1-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="032f1-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="032f1-132">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="032f1-132">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="032f1-133">Contém os destinatários e os tipos de dicas de email a serem recuperadas.</span><span class="sxs-lookup"><span data-stu-id="032f1-133">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="032f1-134">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="032f1-134">Text value</span></span>

<span data-ttu-id="032f1-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="032f1-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="032f1-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="032f1-136">Remarks</span></span>

<span data-ttu-id="032f1-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="032f1-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="032f1-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="032f1-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="032f1-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="032f1-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="032f1-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="032f1-140">Schema Name</span></span>  <br/> |<span data-ttu-id="032f1-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="032f1-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="032f1-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="032f1-142">Validation File</span></span>  <br/> |<span data-ttu-id="032f1-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="032f1-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="032f1-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="032f1-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="032f1-145">False</span><span class="sxs-lookup"><span data-stu-id="032f1-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="032f1-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="032f1-146">See also</span></span>



- [<span data-ttu-id="032f1-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="032f1-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

