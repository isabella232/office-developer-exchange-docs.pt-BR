---
title: Nome (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: O elemento Name representa o nome de exibição do usuário da caixa de correio.
ms.openlocfilehash: 6d30f06c3bfd77d2715798349ab084cdf81f21a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824505"
---
# <a name="name-emailaddress"></a><span data-ttu-id="c98c6-103">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c98c6-103">Name (EmailAddress)</span></span>

<span data-ttu-id="c98c6-104">O elemento **Name** representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c98c6-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="c98c6-105">**String**</span><span class="sxs-lookup"><span data-stu-id="c98c6-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c98c6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c98c6-106">Attributes and elements</span></span>

<span data-ttu-id="c98c6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c98c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c98c6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c98c6-108">Attributes</span></span>

<span data-ttu-id="c98c6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c98c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c98c6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c98c6-110">Child elements</span></span>

<span data-ttu-id="c98c6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c98c6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c98c6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c98c6-112">Parent elements</span></span>

|<span data-ttu-id="c98c6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c98c6-113">**Element**</span></span>|<span data-ttu-id="c98c6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c98c6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c98c6-115">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="c98c6-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="c98c6-116">Representa o usuário de caixa de correio para uma consulta GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="c98c6-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="c98c6-117">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="c98c6-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="c98c6-118">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="c98c6-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="c98c6-119">Representa o usuário de caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="c98c6-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="c98c6-120">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="c98c6-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c98c6-121">Text value</span><span class="sxs-lookup"><span data-stu-id="c98c6-121">Text value</span></span>

<span data-ttu-id="c98c6-122">Se este elemento for usado, será necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="c98c6-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c98c6-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="c98c6-123">Remarks</span></span>

<span data-ttu-id="c98c6-124">Esse elemento pode ocorrer no máximo uma vez no elemento de [Email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="c98c6-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="c98c6-125">Este elemento não é necessário.</span><span class="sxs-lookup"><span data-stu-id="c98c6-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c98c6-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c98c6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="c98c6-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c98c6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c98c6-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="c98c6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c98c6-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c98c6-129">Schema Name</span></span>  <br/> |<span data-ttu-id="c98c6-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c98c6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c98c6-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c98c6-131">Validation File</span></span>  <br/> |<span data-ttu-id="c98c6-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c98c6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c98c6-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c98c6-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="c98c6-134">False</span><span class="sxs-lookup"><span data-stu-id="c98c6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c98c6-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="c98c6-135">See also</span></span>

- [<span data-ttu-id="c98c6-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c98c6-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="c98c6-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="c98c6-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="c98c6-138">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="c98c6-138">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

