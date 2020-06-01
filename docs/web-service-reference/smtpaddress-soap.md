---
title: SmtpAddress (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e833351c-4bd9-4937-8752-c743a7ce57ea
description: O elemento SmtpAddress representa o endereço SMTP alternativo da caixa de correio.
ms.openlocfilehash: 53238caef1287536de838f4167e8937c182b41b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459010"
---
# <a name="smtpaddress-soap"></a><span data-ttu-id="fd269-103">SmtpAddress (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd269-103">SmtpAddress (SOAP)</span></span>

<span data-ttu-id="fd269-104">O elemento **smtpAddress** representa o endereço SMTP alternativo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fd269-104">The **SmtpAddress** element represents the alternate mailbox SMTP address.</span></span> 
  
```XML
<SmtpAddress/>
```

<span data-ttu-id="fd269-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="fd269-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fd269-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fd269-106">Attributes and elements</span></span>

<span data-ttu-id="fd269-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fd269-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd269-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fd269-108">Attributes</span></span>

<span data-ttu-id="fd269-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd269-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd269-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fd269-110">Child elements</span></span>

<span data-ttu-id="fd269-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fd269-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd269-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fd269-112">Parent elements</span></span>

|<span data-ttu-id="fd269-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fd269-113">**Element**</span></span>|<span data-ttu-id="fd269-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd269-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd269-115">AlternateMailbox (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fd269-115">AlternateMailbox (SOAP)</span></span>](alternatemailbox-soap.md) <br/> |<span data-ttu-id="fd269-116">Representa uma caixa de correio alternativa.</span><span class="sxs-lookup"><span data-stu-id="fd269-116">Represents an alternate mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd269-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fd269-117">Text value</span></span>

<span data-ttu-id="fd269-118">O valor de texto do elemento **smtpAddress** é o endereço de email SMTP da caixa de correio alternativa.</span><span class="sxs-lookup"><span data-stu-id="fd269-118">The text value of the **SmtpAddress** element is the SMTP email address of the alternate mailbox.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fd269-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fd269-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd269-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd269-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fd269-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fd269-121">Schema Name</span></span>  <br/> |<span data-ttu-id="fd269-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="fd269-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fd269-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fd269-123">Validation File</span></span>  <br/> |<span data-ttu-id="fd269-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fd269-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd269-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fd269-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd269-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="fd269-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd269-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="fd269-127">See also</span></span>

- [<span data-ttu-id="fd269-128">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="fd269-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="fd269-129">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fd269-129">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

