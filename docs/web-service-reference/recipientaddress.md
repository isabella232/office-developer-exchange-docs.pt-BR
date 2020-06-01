---
title: RecipientAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientAddress
api_type:
- schema
ms.assetid: 9ae6351a-2c60-4715-a489-5681a13641f9
description: O elemento RecipientAddress representa a caixa de correio do destinatário.
ms.openlocfilehash: f4b6edd034dd91471e6496f6b0cca65bd3ffb69a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465846"
---
# <a name="recipientaddress"></a><span data-ttu-id="58ab8-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="58ab8-103">RecipientAddress</span></span>

<span data-ttu-id="58ab8-104">O elemento **RecipientAddress** representa a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="58ab8-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="58ab8-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="58ab8-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58ab8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58ab8-106">Attributes and elements</span></span>

<span data-ttu-id="58ab8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58ab8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58ab8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="58ab8-108">Attributes</span></span>

<span data-ttu-id="58ab8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58ab8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58ab8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58ab8-110">Child elements</span></span>

|<span data-ttu-id="58ab8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58ab8-111">**Element**</span></span>|<span data-ttu-id="58ab8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58ab8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58ab8-113">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="58ab8-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="58ab8-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="58ab8-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="58ab8-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="58ab8-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58ab8-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="58ab8-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="58ab8-117">Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="58ab8-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="58ab8-118">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="58ab8-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58ab8-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="58ab8-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="58ab8-120">Representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="58ab8-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="58ab8-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="58ab8-121">The default is SMTP.</span></span> <span data-ttu-id="58ab8-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="58ab8-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58ab8-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="58ab8-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="58ab8-124">Representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="58ab8-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="58ab8-125">ItemId</span><span class="sxs-lookup"><span data-stu-id="58ab8-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="58ab8-126">Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="58ab8-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="58ab8-127">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="58ab8-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58ab8-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58ab8-128">Parent elements</span></span>

|<span data-ttu-id="58ab8-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58ab8-129">**Element**</span></span>|<span data-ttu-id="58ab8-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58ab8-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58ab8-131">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="58ab8-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="58ab8-132">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="58ab8-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="58ab8-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="58ab8-133">Remarks</span></span>

<span data-ttu-id="58ab8-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58ab8-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58ab8-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58ab8-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58ab8-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="58ab8-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58ab8-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58ab8-137">Schema Name</span></span>  <br/> |<span data-ttu-id="58ab8-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="58ab8-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="58ab8-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58ab8-139">Validation File</span></span>  <br/> |<span data-ttu-id="58ab8-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58ab8-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58ab8-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="58ab8-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="58ab8-142">False</span><span class="sxs-lookup"><span data-stu-id="58ab8-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58ab8-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="58ab8-143">See also</span></span>



- [<span data-ttu-id="58ab8-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58ab8-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

