---
title: Endereço (string)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: O elemento de endereço representa o endereço de email do usuário da caixa de correio.
ms.openlocfilehash: 07c634d6166d88a8912bc66081a13671e600c801
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751067"
---
# <a name="address-string"></a><span data-ttu-id="8ac54-103">Endereço (string)</span><span class="sxs-lookup"><span data-stu-id="8ac54-103">Address (string)</span></span>

<span data-ttu-id="8ac54-104">O elemento de **endereço** representa o endereço de email do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8ac54-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="8ac54-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="8ac54-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ac54-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8ac54-106">Attributes and elements</span></span>

<span data-ttu-id="8ac54-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8ac54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ac54-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8ac54-108">Attributes</span></span>

<span data-ttu-id="8ac54-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ac54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ac54-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8ac54-110">Child elements</span></span>

<span data-ttu-id="8ac54-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ac54-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ac54-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8ac54-112">Parent elements</span></span>

|<span data-ttu-id="8ac54-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8ac54-113">**Element**</span></span>|<span data-ttu-id="8ac54-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ac54-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ac54-115">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8ac54-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="8ac54-116">Especifica o endereço de email do objeto MailboxData.</span><span class="sxs-lookup"><span data-stu-id="8ac54-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="8ac54-117">Este elemento é usado na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8ac54-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="8ac54-118">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="8ac54-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="8ac54-119">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="8ac54-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="8ac54-120">Representa o usuário de caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="8ac54-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="8ac54-121">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="8ac54-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ac54-122">Text value</span><span class="sxs-lookup"><span data-stu-id="8ac54-122">Text value</span></span>

<span data-ttu-id="8ac54-123">Se este elemento for usado, será necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="8ac54-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ac54-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="8ac54-124">Remarks</span></span>

<span data-ttu-id="8ac54-125">Esse elemento pode ocorrer no máximo uma vez no elemento de [Email (EmailAddressType)](email-emailaddresstype.md) e o elemento de [caixa de correio (disponibilidade)](mailbox-availability.md) .</span><span class="sxs-lookup"><span data-stu-id="8ac54-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8ac54-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8ac54-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8ac54-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8ac54-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ac54-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="8ac54-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ac54-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8ac54-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8ac54-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8ac54-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ac54-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8ac54-131">Validation File</span></span>  <br/> |<span data-ttu-id="8ac54-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ac54-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ac54-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8ac54-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ac54-134">False</span><span class="sxs-lookup"><span data-stu-id="8ac54-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ac54-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="8ac54-135">See also</span></span>

- [<span data-ttu-id="8ac54-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8ac54-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="8ac54-137">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ac54-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="8ac54-138">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ac54-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="8ac54-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="8ac54-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="8ac54-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="8ac54-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="8ac54-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="8ac54-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="8ac54-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="8ac54-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

