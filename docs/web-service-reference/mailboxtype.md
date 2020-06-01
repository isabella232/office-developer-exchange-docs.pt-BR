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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459795"
---
# <a name="mailboxtype"></a><span data-ttu-id="8a862-103">MailboxType</span><span class="sxs-lookup"><span data-stu-id="8a862-103">MailboxType</span></span>

<span data-ttu-id="8a862-104">O elemento **MailboxType** representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="8a862-104">The **MailboxType** element represents the type of mailbox that is represented by the e-mail address.</span></span> 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

<span data-ttu-id="8a862-105">**MailboxTypeType**</span><span class="sxs-lookup"><span data-stu-id="8a862-105">**MailboxTypeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8a862-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8a862-106">Attributes and elements</span></span>

<span data-ttu-id="8a862-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8a862-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a862-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8a862-108">Attributes</span></span>

<span data-ttu-id="8a862-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a862-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a862-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8a862-110">Child elements</span></span>

<span data-ttu-id="8a862-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8a862-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8a862-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8a862-112">Parent elements</span></span>

|<span data-ttu-id="8a862-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8a862-113">**Element**</span></span>|<span data-ttu-id="8a862-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a862-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a862-115">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="8a862-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8a862-116">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="8a862-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="8a862-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="8a862-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="8a862-118">Identifica uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="8a862-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8a862-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8a862-119">Text value</span></span>

<span data-ttu-id="8a862-120">A tabela a seguir lista os valores possíveis para o elemento **MailboxType** .</span><span class="sxs-lookup"><span data-stu-id="8a862-120">The following table lists the possible values for the **MailboxType** element.</span></span> 
  
|<span data-ttu-id="8a862-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="8a862-121">**Value**</span></span>|<span data-ttu-id="8a862-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a862-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a862-123">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="8a862-123">Mailbox</span></span>  <br/> |<span data-ttu-id="8a862-124">Representa um objeto do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="8a862-124">Represents a mail-enabled Active Directory object.</span></span>  <br/> |
|<span data-ttu-id="8a862-125">PublicDL</span><span class="sxs-lookup"><span data-stu-id="8a862-125">PublicDL</span></span>  <br/> |<span data-ttu-id="8a862-126">Representa uma lista de distribuição pública.</span><span class="sxs-lookup"><span data-stu-id="8a862-126">Represents a public distribution list.</span></span>  <br/> |
|<span data-ttu-id="8a862-127">PrivateDL</span><span class="sxs-lookup"><span data-stu-id="8a862-127">PrivateDL</span></span>  <br/> |<span data-ttu-id="8a862-128">Representa uma lista de distribuição privada na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a862-128">Represents a private distribution list in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="8a862-129">Contato</span><span class="sxs-lookup"><span data-stu-id="8a862-129">Contact</span></span>  <br/> |<span data-ttu-id="8a862-130">Representa um contato na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a862-130">Represents a contact in a user's mailbox.</span></span>  <br/> |
|<span data-ttu-id="8a862-131">PublicFolder</span><span class="sxs-lookup"><span data-stu-id="8a862-131">PublicFolder</span></span>  <br/> |<span data-ttu-id="8a862-132">Representa uma pasta pública.</span><span class="sxs-lookup"><span data-stu-id="8a862-132">Represents a public folder.</span></span>  <br/> |
|<span data-ttu-id="8a862-133">Desconhecido</span><span class="sxs-lookup"><span data-stu-id="8a862-133">Unknown</span></span>  <br/> |<span data-ttu-id="8a862-134">Representa um tipo desconhecido de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8a862-134">Represents an unknown type of mailbox.</span></span>  <br/> |
|<span data-ttu-id="8a862-135">OneOff</span><span class="sxs-lookup"><span data-stu-id="8a862-135">OneOff</span></span>  <br/> |<span data-ttu-id="8a862-136">Representa um membro one-off de uma lista de distribuição pessoal.</span><span class="sxs-lookup"><span data-stu-id="8a862-136">Represents a one-off member of a personal distribution list.</span></span>  <br/> |
|<span data-ttu-id="8a862-137">GroupMailbox</span><span class="sxs-lookup"><span data-stu-id="8a862-137">GroupMailbox</span></span>  <br/> |<span data-ttu-id="8a862-138">Representa uma caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="8a862-138">Represents a group mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a862-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="8a862-139">Remarks</span></span>

<span data-ttu-id="8a862-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a862-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a862-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8a862-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a862-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a862-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a862-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8a862-143">Schema Name</span></span>  <br/> |<span data-ttu-id="8a862-144">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8a862-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a862-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8a862-145">Validation File</span></span>  <br/> |<span data-ttu-id="8a862-146">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8a862-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a862-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8a862-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a862-148">False</span><span class="sxs-lookup"><span data-stu-id="8a862-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a862-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="8a862-149">See also</span></span>

- [<span data-ttu-id="8a862-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a862-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

