---
title: Entrada (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: O elemento ENTRY representa um único endereço de email de um contato.
ms.openlocfilehash: 766d67cda10b02c07a7677e541fddfc38a4285cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459641"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="75eb7-103">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="75eb7-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="75eb7-104">O elemento **entry** representa um único endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="75eb7-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="75eb7-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="75eb7-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="75eb7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="75eb7-106">Attributes and elements</span></span>

<span data-ttu-id="75eb7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="75eb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75eb7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="75eb7-108">Attributes</span></span>

|<span data-ttu-id="75eb7-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="75eb7-109">**Attribute**</span></span>|<span data-ttu-id="75eb7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="75eb7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="75eb7-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="75eb7-111">**Key**</span></span> <br/> | <span data-ttu-id="75eb7-112">Identifica o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="75eb7-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="75eb7-113">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="75eb7-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="75eb7-114">- EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="75eb7-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="75eb7-115">- EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="75eb7-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="75eb7-116">- EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="75eb7-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="75eb7-117">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="75eb7-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="75eb7-118">**Nome**</span><span class="sxs-lookup"><span data-stu-id="75eb7-118">**Name**</span></span> <br/> |<span data-ttu-id="75eb7-119">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="75eb7-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="75eb7-120">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="75eb7-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="75eb7-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="75eb7-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="75eb7-122">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="75eb7-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="75eb7-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="75eb7-123">The default is SMTP.</span></span> <span data-ttu-id="75eb7-124">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="75eb7-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="75eb7-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="75eb7-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="75eb7-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="75eb7-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="75eb7-127">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="75eb7-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="75eb7-128">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="75eb7-128">Child elements</span></span>

<span data-ttu-id="75eb7-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="75eb7-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75eb7-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="75eb7-130">Parent elements</span></span>

|<span data-ttu-id="75eb7-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="75eb7-131">**Element**</span></span>|<span data-ttu-id="75eb7-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="75eb7-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75eb7-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="75eb7-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="75eb7-134">Representa uma coleção de endereços de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="75eb7-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="75eb7-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="75eb7-135">Remarks</span></span>

<span data-ttu-id="75eb7-136">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="75eb7-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="75eb7-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="75eb7-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75eb7-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="75eb7-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75eb7-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="75eb7-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75eb7-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="75eb7-140">Schema name</span></span>  <br/> |<span data-ttu-id="75eb7-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="75eb7-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="75eb7-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="75eb7-142">Validation file</span></span>  <br/> |<span data-ttu-id="75eb7-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="75eb7-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75eb7-144">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="75eb7-144">Can be empty</span></span>  <br/> |<span data-ttu-id="75eb7-145">False</span><span class="sxs-lookup"><span data-stu-id="75eb7-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75eb7-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="75eb7-146">See also</span></span>

- [<span data-ttu-id="75eb7-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="75eb7-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

