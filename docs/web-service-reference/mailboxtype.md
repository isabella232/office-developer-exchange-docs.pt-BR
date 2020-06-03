---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: O elemento MailboxType representa o tipo de caixa de correio que é representado pelo endereço de email.
ms.openlocfilehash: 8c322ab8a87730832f5d199698a369656b058a9a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459795"
---
# <a name="mailboxtype"></a><span data-ttu-id="d3fdd-103">MailboxType</span><span class="sxs-lookup"><span data-stu-id="d3fdd-103">MailboxType</span></span>

<span data-ttu-id="d3fdd-104">O elemento **MailboxType** representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-104">The **MailboxType** element represents the type of mailbox that is represented by the e-mail address.</span></span> 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

<span data-ttu-id="d3fdd-105">**MailboxTypeType**</span><span class="sxs-lookup"><span data-stu-id="d3fdd-105">**MailboxTypeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d3fdd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d3fdd-106">Attributes and elements</span></span>

<span data-ttu-id="d3fdd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3fdd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d3fdd-108">Attributes</span></span>

<span data-ttu-id="d3fdd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3fdd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3fdd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d3fdd-110">Child elements</span></span>

<span data-ttu-id="d3fdd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3fdd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d3fdd-112">Parent elements</span></span>

|<span data-ttu-id="d3fdd-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d3fdd-113">**Element**</span></span>|<span data-ttu-id="d3fdd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3fdd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3fdd-115">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="d3fdd-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d3fdd-116">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="d3fdd-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="d3fdd-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="d3fdd-118">Identifica uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3fdd-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d3fdd-119">Text value</span></span>

<span data-ttu-id="d3fdd-120">A tabela a seguir lista os valores possíveis para o elemento **MailboxType** .</span><span class="sxs-lookup"><span data-stu-id="d3fdd-120">The following table lists the possible values for the **MailboxType** element.</span></span> 
  
|<span data-ttu-id="d3fdd-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d3fdd-121">**Value**</span></span>|<span data-ttu-id="d3fdd-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3fdd-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3fdd-123">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="d3fdd-123">Mailbox</span></span>  <br/> |<span data-ttu-id="d3fdd-124">Representa um objeto do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-124">Represents a mail-enabled Active Directory object.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-125">PublicDL</span><span class="sxs-lookup"><span data-stu-id="d3fdd-125">PublicDL</span></span>  <br/> |<span data-ttu-id="d3fdd-126">Representa uma lista de distribuição pública.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-126">Represents a public distribution list.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-127">PrivateDL</span><span class="sxs-lookup"><span data-stu-id="d3fdd-127">PrivateDL</span></span>  <br/> |<span data-ttu-id="d3fdd-128">Representa uma lista de distribuição privada na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-128">Represents a private distribution list in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-129">Contato</span><span class="sxs-lookup"><span data-stu-id="d3fdd-129">Contact</span></span>  <br/> |<span data-ttu-id="d3fdd-130">Representa um contato na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-130">Represents a contact in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-131">PublicFolder</span><span class="sxs-lookup"><span data-stu-id="d3fdd-131">PublicFolder</span></span>  <br/> |<span data-ttu-id="d3fdd-132">Representa uma pasta pública.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-132">Represents a public folder.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-133">Desconhecido</span><span class="sxs-lookup"><span data-stu-id="d3fdd-133">Unknown</span></span>  <br/> |<span data-ttu-id="d3fdd-134">Representa um tipo desconhecido de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-134">Represents an unknown type of mailbox.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-135">OneOff</span><span class="sxs-lookup"><span data-stu-id="d3fdd-135">OneOff</span></span>  <br/> |<span data-ttu-id="d3fdd-136">Representa um membro one-off de uma lista de distribuição pessoal.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-136">Represents a one-off member of a personal distribution list.</span></span>  <br/> |
|<span data-ttu-id="d3fdd-137">GroupMailbox</span><span class="sxs-lookup"><span data-stu-id="d3fdd-137">GroupMailbox</span></span>  <br/> |<span data-ttu-id="d3fdd-138">Representa uma caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-138">Represents a group mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3fdd-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="d3fdd-139">Remarks</span></span>

<span data-ttu-id="d3fdd-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3fdd-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3fdd-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d3fdd-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3fdd-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3fdd-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3fdd-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d3fdd-143">Schema Name</span></span>  <br/> |<span data-ttu-id="d3fdd-144">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d3fdd-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3fdd-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d3fdd-145">Validation File</span></span>  <br/> |<span data-ttu-id="d3fdd-146">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d3fdd-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3fdd-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d3fdd-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3fdd-148">False</span><span class="sxs-lookup"><span data-stu-id="d3fdd-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3fdd-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="d3fdd-149">See also</span></span>

- [<span data-ttu-id="d3fdd-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d3fdd-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

