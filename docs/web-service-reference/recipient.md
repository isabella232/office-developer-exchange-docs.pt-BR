---
title: Destinatário
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipient
api_type:
- schema
ms.assetid: 52adbb30-3bfd-48aa-9ea8-9f7d3b4bee44
description: O elemento Recipient representa o destinatário para o qual o evento ocorreu.
ms.openlocfilehash: eb7e85acf3c2b898b3f0bff4b63168d344e1daa8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465853"
---
# <a name="recipient"></a><span data-ttu-id="67377-103">Destinatário</span><span class="sxs-lookup"><span data-stu-id="67377-103">Recipient</span></span>

<span data-ttu-id="67377-104">O elemento **Recipient** representa o destinatário para o qual o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="67377-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="67377-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="67377-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67377-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="67377-106">Attributes and elements</span></span>

<span data-ttu-id="67377-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="67377-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67377-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="67377-108">Attributes</span></span>

<span data-ttu-id="67377-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67377-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67377-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="67377-110">Child elements</span></span>

|<span data-ttu-id="67377-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="67377-111">**Element**</span></span>|<span data-ttu-id="67377-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="67377-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67377-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="67377-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="67377-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="67377-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="67377-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="67377-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="67377-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="67377-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="67377-117">Define o endereço SMTP (Simple Mail Transfer Protocol) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="67377-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="67377-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="67377-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="67377-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="67377-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="67377-120">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="67377-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="67377-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="67377-121">The default value is SMTP.</span></span> <span data-ttu-id="67377-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="67377-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="67377-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="67377-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="67377-124">Representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="67377-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="67377-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="67377-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="67377-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="67377-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="67377-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="67377-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="67377-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="67377-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67377-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="67377-129">Parent elements</span></span>

|<span data-ttu-id="67377-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="67377-130">**Element**</span></span>|<span data-ttu-id="67377-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="67377-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67377-132">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="67377-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="67377-133">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="67377-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="67377-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="67377-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="67377-135">Especifica critérios para os tipos de mensagens a serem encontradas.</span><span class="sxs-lookup"><span data-stu-id="67377-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67377-136">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="67377-136">Text value</span></span>

<span data-ttu-id="67377-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="67377-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="67377-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="67377-138">Remarks</span></span>

<span data-ttu-id="67377-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="67377-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67377-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="67377-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67377-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="67377-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67377-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="67377-142">Schema Name</span></span>  <br/> |<span data-ttu-id="67377-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="67377-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="67377-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="67377-144">Validation File</span></span>  <br/> |<span data-ttu-id="67377-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="67377-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67377-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="67377-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="67377-147">False</span><span class="sxs-lookup"><span data-stu-id="67377-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67377-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="67377-148">See also</span></span>



- [<span data-ttu-id="67377-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="67377-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

