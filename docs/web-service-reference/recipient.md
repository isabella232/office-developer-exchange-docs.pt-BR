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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465853"
---
# <a name="recipient"></a><span data-ttu-id="b36ec-103">Destinatário</span><span class="sxs-lookup"><span data-stu-id="b36ec-103">Recipient</span></span>

<span data-ttu-id="b36ec-104">O elemento **Recipient** representa o destinatário para o qual o evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="b36ec-104">The **Recipient** element represents the recipient for whom the event occurred.</span></span> 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 <span data-ttu-id="b36ec-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="b36ec-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b36ec-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b36ec-106">Attributes and elements</span></span>

<span data-ttu-id="b36ec-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b36ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b36ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b36ec-108">Attributes</span></span>

<span data-ttu-id="b36ec-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b36ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b36ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b36ec-110">Child elements</span></span>

|<span data-ttu-id="b36ec-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b36ec-111">**Element**</span></span>|<span data-ttu-id="b36ec-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b36ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b36ec-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="b36ec-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="b36ec-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b36ec-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="b36ec-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b36ec-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b36ec-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="b36ec-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="b36ec-117">Define o endereço SMTP (Simple Mail Transfer Protocol) principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b36ec-117">Defines the primary Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="b36ec-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b36ec-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b36ec-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="b36ec-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="b36ec-120">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b36ec-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="b36ec-121">O valor padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="b36ec-121">The default value is SMTP.</span></span> <span data-ttu-id="b36ec-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b36ec-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b36ec-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="b36ec-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="b36ec-124">Representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="b36ec-124">Represents the type of mailbox that is represented by the e-mail address.</span></span> <span data-ttu-id="b36ec-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b36ec-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b36ec-126">ItemId</span><span class="sxs-lookup"><span data-stu-id="b36ec-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b36ec-127">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b36ec-127">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="b36ec-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b36ec-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b36ec-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b36ec-129">Parent elements</span></span>

|<span data-ttu-id="b36ec-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b36ec-130">**Element**</span></span>|<span data-ttu-id="b36ec-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b36ec-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b36ec-132">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="b36ec-132">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="b36ec-133">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="b36ec-133">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="b36ec-134">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b36ec-134">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b36ec-135">Especifica critérios para os tipos de mensagens a serem encontradas.</span><span class="sxs-lookup"><span data-stu-id="b36ec-135">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b36ec-136">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b36ec-136">Text value</span></span>

<span data-ttu-id="b36ec-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b36ec-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b36ec-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="b36ec-138">Remarks</span></span>

<span data-ttu-id="b36ec-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b36ec-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b36ec-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b36ec-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b36ec-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="b36ec-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b36ec-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b36ec-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b36ec-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b36ec-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b36ec-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b36ec-144">Validation File</span></span>  <br/> |<span data-ttu-id="b36ec-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b36ec-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b36ec-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b36ec-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b36ec-147">False</span><span class="sxs-lookup"><span data-stu-id="b36ec-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b36ec-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="b36ec-148">See also</span></span>



- [<span data-ttu-id="b36ec-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b36ec-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

