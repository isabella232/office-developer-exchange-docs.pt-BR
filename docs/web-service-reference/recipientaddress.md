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
ms.openlocfilehash: 10928ac206227cfc21bd83ab5bfa9a55aad354e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824974"
---
# <a name="recipientaddress"></a><span data-ttu-id="afb89-103">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="afb89-103">RecipientAddress</span></span>

<span data-ttu-id="afb89-104">O elemento **RecipientAddress** representa a caixa de correio do destinatário.</span><span class="sxs-lookup"><span data-stu-id="afb89-104">The **RecipientAddress** element represents the mailbox of the recipient.</span></span> 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 <span data-ttu-id="afb89-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="afb89-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afb89-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="afb89-106">Attributes and elements</span></span>

<span data-ttu-id="afb89-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="afb89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afb89-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="afb89-108">Attributes</span></span>

<span data-ttu-id="afb89-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afb89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afb89-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="afb89-110">Child elements</span></span>

|<span data-ttu-id="afb89-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afb89-111">**Element**</span></span>|<span data-ttu-id="afb89-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afb89-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afb89-113">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="afb89-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="afb89-114">Representa o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afb89-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="afb89-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="afb89-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="afb89-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="afb89-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="afb89-117">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afb89-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="afb89-118">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="afb89-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="afb89-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="afb89-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="afb89-120">Representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="afb89-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="afb89-121">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="afb89-121">The default is SMTP.</span></span> <span data-ttu-id="afb89-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="afb89-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="afb89-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="afb89-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="afb89-124">Representa o tipo de caixa de correio que é representado por um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="afb89-124">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="afb89-125">ItemId</span><span class="sxs-lookup"><span data-stu-id="afb89-125">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="afb89-126">Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="afb89-126">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="afb89-127">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="afb89-127">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="afb89-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="afb89-128">Parent elements</span></span>

|<span data-ttu-id="afb89-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afb89-129">**Element**</span></span>|<span data-ttu-id="afb89-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afb89-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afb89-131">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="afb89-131">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="afb89-132">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="afb89-132">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="afb89-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="afb89-133">Remarks</span></span>

<span data-ttu-id="afb89-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="afb89-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afb89-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="afb89-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afb89-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="afb89-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afb89-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="afb89-137">Schema Name</span></span>  <br/> |<span data-ttu-id="afb89-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="afb89-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="afb89-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="afb89-139">Validation File</span></span>  <br/> |<span data-ttu-id="afb89-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afb89-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afb89-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="afb89-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="afb89-142">False</span><span class="sxs-lookup"><span data-stu-id="afb89-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afb89-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="afb89-143">See also</span></span>



- [<span data-ttu-id="afb89-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="afb89-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

