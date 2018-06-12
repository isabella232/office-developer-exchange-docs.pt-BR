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
ms.openlocfilehash: 8eb53e4846ad55916e2c5876606c00c0f2e371ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751135"
---
# <a name="alternatemailbox-soap"></a><span data-ttu-id="804d6-103">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-103">AlternateMailbox (SOAP)</span></span>

<span data-ttu-id="804d6-104">O elemento **AlternateMailbox** representa uma caixa de correio alternativa.</span><span class="sxs-lookup"><span data-stu-id="804d6-104">The **AlternateMailbox** element represents an alternate mailbox.</span></span> 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 <span data-ttu-id="804d6-105">**AlternateMailbox**</span><span class="sxs-lookup"><span data-stu-id="804d6-105">**AlternateMailbox**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="804d6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="804d6-106">Attributes and elements</span></span>

<span data-ttu-id="804d6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="804d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="804d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="804d6-108">Attributes</span></span>

<span data-ttu-id="804d6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="804d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="804d6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="804d6-110">Child elements</span></span>

|<span data-ttu-id="804d6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="804d6-111">**Element**</span></span>|<span data-ttu-id="804d6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="804d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="804d6-113">Tipo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-113">Type (SOAP)</span></span>](type-soap.md) <br/> |<span data-ttu-id="804d6-114">Representa o tipo de caixa de correio alternativo.</span><span class="sxs-lookup"><span data-stu-id="804d6-114">Represents the alternate mailbox type.</span></span>  <br/> |
|[<span data-ttu-id="804d6-115">DisplayName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-115">DisplayName (SOAP)</span></span>](displayname-soap.md) <br/> |<span data-ttu-id="804d6-116">Representa o nome de exibição da caixa de correio alternativo.</span><span class="sxs-lookup"><span data-stu-id="804d6-116">Represents the alternate mailbox display name.</span></span>  <br/> |
|[<span data-ttu-id="804d6-117">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-117">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="804d6-118">Representa o nome distinto herdado de caixa de correio alternativo.</span><span class="sxs-lookup"><span data-stu-id="804d6-118">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="804d6-119">Servidor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-119">Server (SOAP)</span></span>](server-soap.md) <br/> |<span data-ttu-id="804d6-120">Representa o servidor de caixa de correio alternativo.</span><span class="sxs-lookup"><span data-stu-id="804d6-120">Represents the alternate mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="804d6-121">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-121">SmtpAddress (SOAP)</span></span>](smtpaddress-soap.md) <br/> |<span data-ttu-id="804d6-122">Representa a endereço SMTP da caixa de correio alternativa.</span><span class="sxs-lookup"><span data-stu-id="804d6-122">Represents the alternate mailbox SMTP address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="804d6-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="804d6-123">Parent elements</span></span>

|<span data-ttu-id="804d6-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="804d6-124">**Element**</span></span>|<span data-ttu-id="804d6-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="804d6-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="804d6-126">AlternateMailboxes (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-126">AlternateMailboxes (SOAP)</span></span>](alternatemailboxes-soap.md) <br/> |<span data-ttu-id="804d6-127">Representa uma coleção de caixas de correio alternativas.</span><span class="sxs-lookup"><span data-stu-id="804d6-127">Represents a collection of alternate mailboxes.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="804d6-128">Text value</span><span class="sxs-lookup"><span data-stu-id="804d6-128">Text value</span></span>

<span data-ttu-id="804d6-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="804d6-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="804d6-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="804d6-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="804d6-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="804d6-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="804d6-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="804d6-132">Schema Name</span></span>  <br/> |<span data-ttu-id="804d6-133">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="804d6-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="804d6-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="804d6-134">Validation File</span></span>  <br/> |<span data-ttu-id="804d6-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="804d6-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="804d6-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="804d6-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="804d6-137">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="804d6-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="804d6-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="804d6-138">See also</span></span>

- [<span data-ttu-id="804d6-139">AlternateMailboxCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="804d6-139">AlternateMailboxCollectionSetting (SOAP)</span></span>](alternatemailboxcollectionsetting-soap.md)

