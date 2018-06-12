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
description: O elemento de entrada representa um único endereço de email de um contato.
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752076"
---
# <a name="entry-emailaddress"></a><span data-ttu-id="4316b-103">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="4316b-103">Entry (EmailAddress)</span></span>

<span data-ttu-id="4316b-104">O elemento de **entrada** representa um único endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="4316b-104">The **Entry** element represents a single e-mail address for a contact.</span></span> 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

<span data-ttu-id="4316b-105">**EmailAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="4316b-105">**EmailAddressDictionaryEntryType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4316b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4316b-106">Attributes and elements</span></span>

<span data-ttu-id="4316b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4316b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4316b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4316b-108">Attributes</span></span>

|<span data-ttu-id="4316b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="4316b-109">**Attribute**</span></span>|<span data-ttu-id="4316b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4316b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4316b-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="4316b-111">**Key**</span></span> <br/> | <span data-ttu-id="4316b-112">Identifica o endereço de email.</span><span class="sxs-lookup"><span data-stu-id="4316b-112">Identifies the e-mail address.</span></span><br/><br/><span data-ttu-id="4316b-113">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="4316b-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="4316b-114">-EmailAddress1</span><span class="sxs-lookup"><span data-stu-id="4316b-114">-  EmailAddress1</span></span>  <br/><span data-ttu-id="4316b-115">-EmailAddress2</span><span class="sxs-lookup"><span data-stu-id="4316b-115">-  EmailAddress2</span></span>  <br/><span data-ttu-id="4316b-116">-EmailAddress3</span><span class="sxs-lookup"><span data-stu-id="4316b-116">-  EmailAddress3</span></span> <br/><br/>  <span data-ttu-id="4316b-117">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="4316b-117">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4316b-118">**Name**</span><span class="sxs-lookup"><span data-stu-id="4316b-118">**Name**</span></span> <br/> |<span data-ttu-id="4316b-119">Define o nome do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4316b-119">Defines the name of the mailbox user.</span></span> <span data-ttu-id="4316b-120">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="4316b-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="4316b-121">**RoutingType**</span><span class="sxs-lookup"><span data-stu-id="4316b-121">**RoutingType**</span></span> <br/> |<span data-ttu-id="4316b-122">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4316b-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="4316b-123">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="4316b-123">The default is SMTP.</span></span> <span data-ttu-id="4316b-124">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="4316b-124">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="4316b-125">**MailboxType**</span><span class="sxs-lookup"><span data-stu-id="4316b-125">**MailboxType**</span></span> <br/> |<span data-ttu-id="4316b-126">Define o tipo de caixa de correio de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4316b-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="4316b-127">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="4316b-127">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4316b-128">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4316b-128">Child elements</span></span>

<span data-ttu-id="4316b-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4316b-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4316b-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4316b-130">Parent elements</span></span>

|<span data-ttu-id="4316b-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4316b-131">**Element**</span></span>|<span data-ttu-id="4316b-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4316b-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4316b-133">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="4316b-133">EmailAddresses</span></span>](emailaddresses.md) <br/> |<span data-ttu-id="4316b-134">Representa uma coleção de endereços de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="4316b-134">Represents a collection of e-mail addresses for a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4316b-135">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4316b-135">Remarks</span></span>

<span data-ttu-id="4316b-136">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4316b-136">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4316b-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4316b-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4316b-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4316b-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4316b-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="4316b-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4316b-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4316b-140">Schema name</span></span>  <br/> |<span data-ttu-id="4316b-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4316b-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="4316b-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4316b-142">Validation file</span></span>  <br/> |<span data-ttu-id="4316b-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4316b-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4316b-144">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4316b-144">Can be empty</span></span>  <br/> |<span data-ttu-id="4316b-145">False</span><span class="sxs-lookup"><span data-stu-id="4316b-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4316b-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="4316b-146">See also</span></span>

- [<span data-ttu-id="4316b-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4316b-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

