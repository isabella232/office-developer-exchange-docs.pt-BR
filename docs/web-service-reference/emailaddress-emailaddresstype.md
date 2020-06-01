---
title: EmailAddress (EmailAddresstype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: O elemento EmailAddress especifica o endereço SMTP totalmente resolvido para a caixa de correio do site ou a pessoa associada.
ms.openlocfilehash: 8b04b75e91cc16be7f88c9a0ac08c5e36855056e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463458"
---
# <a name="emailaddress-emailaddresstype"></a><span data-ttu-id="47dbe-103">EmailAddress (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="47dbe-103">EmailAddress (EmailAddressType)</span></span>

<span data-ttu-id="47dbe-104">O elemento **EmailAddress** especifica o endereço SMTP totalmente resolvido para a caixa de correio do site ou a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="47dbe-104">The **EmailAddress** element specifies the fully resolved SMTP address for the site mailbox or the associated persona.</span></span> 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 <span data-ttu-id="47dbe-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="47dbe-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47dbe-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="47dbe-106">Attributes and elements</span></span>

<span data-ttu-id="47dbe-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47dbe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47dbe-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="47dbe-108">Attributes</span></span>

<span data-ttu-id="47dbe-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47dbe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47dbe-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47dbe-110">Child elements</span></span>

|<span data-ttu-id="47dbe-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47dbe-111">**Element**</span></span>|<span data-ttu-id="47dbe-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47dbe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47dbe-113">Nome (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="47dbe-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="47dbe-114">Especifica um nome ou chave de refinador de pesquisa ou o nome de um usuário de email.</span><span class="sxs-lookup"><span data-stu-id="47dbe-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="47dbe-115">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="47dbe-115">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="47dbe-116">Define o endereço SMTP principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="47dbe-116">Defines the primary SMTP address of a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="47dbe-117">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="47dbe-117">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md) <br/> |<span data-ttu-id="47dbe-118">Especifica o tipo de roteamento de um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="47dbe-118">Specifies the routing type of an email address.</span></span>  <br/> |
|[<span data-ttu-id="47dbe-119">MailboxType</span><span class="sxs-lookup"><span data-stu-id="47dbe-119">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="47dbe-120">Representa o tipo de caixa de correio que é representado pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="47dbe-120">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="47dbe-121">ItemId</span><span class="sxs-lookup"><span data-stu-id="47dbe-121">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="47dbe-122">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="47dbe-122">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47dbe-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47dbe-123">Parent elements</span></span>

|<span data-ttu-id="47dbe-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47dbe-124">**Element**</span></span>|<span data-ttu-id="47dbe-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47dbe-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47dbe-126">Pessoal</span><span class="sxs-lookup"><span data-stu-id="47dbe-126">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="47dbe-127">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="47dbe-127">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47dbe-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="47dbe-128">Text value</span></span>

<span data-ttu-id="47dbe-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47dbe-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="47dbe-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="47dbe-130">Remarks</span></span>

<span data-ttu-id="47dbe-131">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="47dbe-131">This element is optional.</span></span>
  
<span data-ttu-id="47dbe-132">O elemento **EmailAddress** é aplicável para clientes que direcionam o Exchange Online e versões do Microsoft Exchange Server a partir do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="47dbe-132">The **EmailAddress** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="47dbe-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="47dbe-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47dbe-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="47dbe-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47dbe-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47dbe-135">Schema Name</span></span>  <br/> |<span data-ttu-id="47dbe-136">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="47dbe-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="47dbe-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47dbe-137">Validation File</span></span>  <br/> |<span data-ttu-id="47dbe-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="47dbe-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="47dbe-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="47dbe-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="47dbe-140">Também consulte</span><span class="sxs-lookup"><span data-stu-id="47dbe-140">See also</span></span>

- [<span data-ttu-id="47dbe-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="47dbe-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

