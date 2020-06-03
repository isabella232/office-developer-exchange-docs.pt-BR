---
title: Endereço (cadeia de caracteres)
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
description: O elemento address representa o endereço de email do usuário da caixa de correio.
ms.openlocfilehash: 839107050f22df5c00cb4dea9c531563df52933d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463640"
---
# <a name="address-string"></a><span data-ttu-id="afcdb-103">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="afcdb-103">Address (string)</span></span>

<span data-ttu-id="afcdb-104">O elemento **Address** representa o endereço de email do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afcdb-104">The **Address** element represents the e-mail address of the mailbox user.</span></span> 
  
```xml
<Address>...</Address>
```

 <span data-ttu-id="afcdb-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="afcdb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afcdb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="afcdb-106">Attributes and elements</span></span>

<span data-ttu-id="afcdb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="afcdb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afcdb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="afcdb-108">Attributes</span></span>

<span data-ttu-id="afcdb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afcdb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afcdb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="afcdb-110">Child elements</span></span>

<span data-ttu-id="afcdb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afcdb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afcdb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="afcdb-112">Parent elements</span></span>

|<span data-ttu-id="afcdb-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afcdb-113">**Element**</span></span>|<span data-ttu-id="afcdb-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afcdb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afcdb-115">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="afcdb-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="afcdb-116">Especifica o endereço de email do objeto MailboxData.</span><span class="sxs-lookup"><span data-stu-id="afcdb-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="afcdb-117">Este elemento é usado na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="afcdb-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span><br/><br/> <span data-ttu-id="afcdb-118">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="afcdb-118">The following is the XPath to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="afcdb-119">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="afcdb-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="afcdb-120">Representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="afcdb-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span><br/><br/>  <span data-ttu-id="afcdb-121">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="afcdb-121">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afcdb-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="afcdb-122">Text value</span></span>

<span data-ttu-id="afcdb-123">Um valor de texto será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="afcdb-123">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="afcdb-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="afcdb-124">Remarks</span></span>

<span data-ttu-id="afcdb-125">Esse elemento pode ocorrer no máximo uma vez no elemento [email (EmailAddressType)](email-emailaddresstype.md) e no elemento [Mailbox (disponibilidade)](mailbox-availability.md) .</span><span class="sxs-lookup"><span data-stu-id="afcdb-125">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element and the [Mailbox (Availability)](mailbox-availability.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="afcdb-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="afcdb-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="afcdb-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="afcdb-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afcdb-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="afcdb-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afcdb-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="afcdb-129">Schema Name</span></span>  <br/> |<span data-ttu-id="afcdb-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="afcdb-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="afcdb-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="afcdb-131">Validation File</span></span>  <br/> |<span data-ttu-id="afcdb-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="afcdb-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afcdb-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="afcdb-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="afcdb-134">False</span><span class="sxs-lookup"><span data-stu-id="afcdb-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afcdb-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="afcdb-135">See also</span></span>

- [<span data-ttu-id="afcdb-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="afcdb-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="afcdb-137">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="afcdb-137">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="afcdb-138">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="afcdb-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="afcdb-139">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="afcdb-139">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="afcdb-140">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="afcdb-140">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
- [<span data-ttu-id="afcdb-141">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="afcdb-141">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
- [<span data-ttu-id="afcdb-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="afcdb-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

