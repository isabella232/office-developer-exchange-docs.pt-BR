---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: O elemento EmailAddress Especifica o endereço SMTP completamente resolvido para a caixa de correio de site ou a pessoa associada.
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751984"
---
# <a name="emailaddress-emailaddresstype"></a><span data-ttu-id="bd047-103">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="bd047-103">EmailAddress (EmailAddressType)</span></span>

<span data-ttu-id="bd047-104">O elemento **EmailAddress** Especifica o endereço SMTP completamente resolvido para a caixa de correio de site ou a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="bd047-104">The **EmailAddress** element specifies the fully resolved SMTP address for the site mailbox or the associated persona.</span></span> 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 <span data-ttu-id="bd047-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="bd047-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd047-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bd047-106">Attributes and elements</span></span>

<span data-ttu-id="bd047-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bd047-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd047-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bd047-108">Attributes</span></span>

<span data-ttu-id="bd047-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bd047-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd047-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bd047-110">Child elements</span></span>

|<span data-ttu-id="bd047-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bd047-111">**Element**</span></span>|<span data-ttu-id="bd047-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bd047-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd047-113">Nome (string)</span><span class="sxs-lookup"><span data-stu-id="bd047-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="bd047-114">Especifica o nome de um usuário de email ou um nome de refinador de pesquisa ou chave.</span><span class="sxs-lookup"><span data-stu-id="bd047-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="bd047-115">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="bd047-115">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="bd047-116">Define o endereço SMTP principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="bd047-116">Defines the primary SMTP address of a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="bd047-117">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="bd047-117">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md) <br/> |<span data-ttu-id="bd047-118">Especifica o tipo de roteamento de um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="bd047-118">Specifies the routing type of an email address.</span></span>  <br/> |
|[<span data-ttu-id="bd047-119">MailboxType</span><span class="sxs-lookup"><span data-stu-id="bd047-119">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="bd047-120">Representa o tipo de caixa de correio que é representado por um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="bd047-120">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="bd047-121">ItemId</span><span class="sxs-lookup"><span data-stu-id="bd047-121">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="bd047-122">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd047-122">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd047-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bd047-123">Parent elements</span></span>

|<span data-ttu-id="bd047-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bd047-124">**Element**</span></span>|<span data-ttu-id="bd047-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bd047-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd047-126">Pessoa</span><span class="sxs-lookup"><span data-stu-id="bd047-126">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="bd047-127">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="bd047-127">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd047-128">Text value</span><span class="sxs-lookup"><span data-stu-id="bd047-128">Text value</span></span>

<span data-ttu-id="bd047-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bd047-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd047-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="bd047-130">Remarks</span></span>

<span data-ttu-id="bd047-131">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="bd047-131">This element is optional.</span></span>
  
<span data-ttu-id="bd047-132">O elemento **EmailAddress** é aplicável para clientes que visam o Exchange Online e versões do Microsoft Exchange Server, começando com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="bd047-132">The **EmailAddress** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="bd047-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bd047-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd047-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="bd047-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd047-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bd047-135">Schema Name</span></span>  <br/> |<span data-ttu-id="bd047-136">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="bd047-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="bd047-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bd047-137">Validation File</span></span>  <br/> |<span data-ttu-id="bd047-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd047-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd047-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="bd047-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bd047-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="bd047-140">See also</span></span>

- [<span data-ttu-id="bd047-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bd047-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

