---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: O elemento AlternateMailbox representa uma caixa de correio alternativa.
ms.openlocfilehash: 9019f85a373cc186cc9dadddceee3dc9d11b3854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466154"
---
# <a name="alternatemailbox-soap"></a><span data-ttu-id="4aa54-103">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-103">AlternateMailbox (SOAP)</span></span>

<span data-ttu-id="4aa54-104">O elemento **AlternateMailbox** representa uma caixa de correio alternativa.</span><span class="sxs-lookup"><span data-stu-id="4aa54-104">The **AlternateMailbox** element represents an alternate mailbox.</span></span> 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 <span data-ttu-id="4aa54-105">**AlternateMailbox**</span><span class="sxs-lookup"><span data-stu-id="4aa54-105">**AlternateMailbox**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4aa54-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4aa54-106">Attributes and elements</span></span>

<span data-ttu-id="4aa54-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4aa54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4aa54-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4aa54-108">Attributes</span></span>

<span data-ttu-id="4aa54-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4aa54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4aa54-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4aa54-110">Child elements</span></span>

|<span data-ttu-id="4aa54-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4aa54-111">**Element**</span></span>|<span data-ttu-id="4aa54-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4aa54-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aa54-113">Tipo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-113">Type (SOAP)</span></span>](type-soap.md) <br/> |<span data-ttu-id="4aa54-114">Representa o tipo de caixa de correio alternativa.</span><span class="sxs-lookup"><span data-stu-id="4aa54-114">Represents the alternate mailbox type.</span></span>  <br/> |
|[<span data-ttu-id="4aa54-115">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-115">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="4aa54-116">Representa o nome de exibição alternativo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4aa54-116">Represents the alternate mailbox display name.</span></span>  <br/> |
|[<span data-ttu-id="4aa54-117">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-117">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="4aa54-118">Representa o nome diferenciado herdado da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4aa54-118">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="4aa54-119">Servidor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-119">Server (SOAP)</span></span>](server-soap.md) <br/> |<span data-ttu-id="4aa54-120">Representa o servidor de caixa de correio alternativo.</span><span class="sxs-lookup"><span data-stu-id="4aa54-120">Represents the alternate mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="4aa54-121">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-121">SmtpAddress (SOAP)</span></span>](smtpaddress-soap.md) <br/> |<span data-ttu-id="4aa54-122">Representa o endereço SMTP alternativo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4aa54-122">Represents the alternate mailbox SMTP address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4aa54-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4aa54-123">Parent elements</span></span>

|<span data-ttu-id="4aa54-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4aa54-124">**Element**</span></span>|<span data-ttu-id="4aa54-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4aa54-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aa54-126">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-126">AlternateMailboxes (SOAP)</span></span>](alternatemailboxes-soap.md) <br/> |<span data-ttu-id="4aa54-127">Representa uma coleção de caixas de correio alternadas.</span><span class="sxs-lookup"><span data-stu-id="4aa54-127">Represents a collection of alternate mailboxes.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4aa54-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4aa54-128">Text value</span></span>

<span data-ttu-id="4aa54-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4aa54-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4aa54-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4aa54-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4aa54-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="4aa54-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4aa54-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4aa54-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4aa54-133">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="4aa54-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4aa54-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4aa54-134">Validation File</span></span>  <br/> |<span data-ttu-id="4aa54-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4aa54-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4aa54-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4aa54-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4aa54-137">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4aa54-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4aa54-138">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4aa54-138">See also</span></span>

- [<span data-ttu-id="4aa54-139">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4aa54-139">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md)

