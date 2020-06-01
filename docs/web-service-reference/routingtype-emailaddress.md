---
title: RoutingType (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: O elemento RoutingType representa o protocolo de roteamento para o destinatário.
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459031"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="61ce9-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="61ce9-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="61ce9-104">O elemento **RoutingType** representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="61ce9-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="61ce9-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="61ce9-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61ce9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="61ce9-106">Attributes and elements</span></span>

<span data-ttu-id="61ce9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61ce9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61ce9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61ce9-108">Attributes</span></span>

<span data-ttu-id="61ce9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61ce9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61ce9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61ce9-110">Child elements</span></span>

<span data-ttu-id="61ce9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="61ce9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61ce9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61ce9-112">Parent elements</span></span>

|<span data-ttu-id="61ce9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61ce9-113">**Element**</span></span>|<span data-ttu-id="61ce9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61ce9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61ce9-115">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="61ce9-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="61ce9-116">Especifica o endereço de email do objeto MailboxData.</span><span class="sxs-lookup"><span data-stu-id="61ce9-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="61ce9-117">Este elemento é usado na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="61ce9-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="61ce9-118">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="61ce9-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="61ce9-119">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="61ce9-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="61ce9-120">Representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="61ce9-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="61ce9-121">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="61ce9-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61ce9-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="61ce9-122">Text value</span></span>

<span data-ttu-id="61ce9-123">Um valor de texto é opcional.</span><span class="sxs-lookup"><span data-stu-id="61ce9-123">A text value is optional.</span></span> <span data-ttu-id="61ce9-124">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="61ce9-124">The following are the possible values:</span></span>

* <span data-ttu-id="61ce9-125">SMTP</span><span class="sxs-lookup"><span data-stu-id="61ce9-125">SMTP</span></span>
* <span data-ttu-id="61ce9-126">EX</span><span class="sxs-lookup"><span data-stu-id="61ce9-126">EX</span></span>

<span data-ttu-id="61ce9-127">Se nenhum valor for fornecido, o valor padrão de SMTP será usado.</span><span class="sxs-lookup"><span data-stu-id="61ce9-127">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61ce9-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="61ce9-128">Remarks</span></span>

<span data-ttu-id="61ce9-129">Esse elemento pode ocorrer no máximo uma vez no elemento [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="61ce9-129">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="61ce9-130">Esse elemento não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61ce9-130">This element is not required.</span></span> <span data-ttu-id="61ce9-131">Esse elemento existe para a inclusão de futuros protocolos.</span><span class="sxs-lookup"><span data-stu-id="61ce9-131">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="61ce9-132">Outro elemento **RoutingType** é usado para acessar itens na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="61ce9-132">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="61ce9-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61ce9-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61ce9-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="61ce9-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61ce9-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="61ce9-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61ce9-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61ce9-136">Schema Name</span></span>  <br/> |<span data-ttu-id="61ce9-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="61ce9-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="61ce9-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61ce9-138">Validation File</span></span>  <br/> |<span data-ttu-id="61ce9-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61ce9-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61ce9-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="61ce9-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="61ce9-141">False</span><span class="sxs-lookup"><span data-stu-id="61ce9-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61ce9-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="61ce9-142">See also</span></span>

- [<span data-ttu-id="61ce9-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="61ce9-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="61ce9-144">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="61ce9-144">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="61ce9-145">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="61ce9-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

