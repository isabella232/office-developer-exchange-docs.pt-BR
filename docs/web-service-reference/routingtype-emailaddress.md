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
ms.openlocfilehash: a0a6cf312bcb1d4b4818a82bc8d8d3e3f33ad6f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825255"
---
# <a name="routingtype-emailaddress"></a><span data-ttu-id="a697a-103">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a697a-103">RoutingType (EmailAddress)</span></span>

<span data-ttu-id="a697a-104">O elemento **RoutingType** representa o protocolo de roteamento para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="a697a-104">The **RoutingType** element represents the routing protocol for the recipient.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="a697a-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="a697a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a697a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a697a-106">Attributes and elements</span></span>

<span data-ttu-id="a697a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a697a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a697a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a697a-108">Attributes</span></span>

<span data-ttu-id="a697a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a697a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a697a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a697a-110">Child elements</span></span>

<span data-ttu-id="a697a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a697a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a697a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a697a-112">Parent elements</span></span>

|<span data-ttu-id="a697a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a697a-113">**Element**</span></span>|<span data-ttu-id="a697a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a697a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a697a-115">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a697a-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="a697a-116">Especifica o endereço de email do objeto MailboxData.</span><span class="sxs-lookup"><span data-stu-id="a697a-116">Specifies the e-mail address of the MailboxData object.</span></span> <span data-ttu-id="a697a-117">Este elemento é usado na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a697a-117">This element is used in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/><br/> <span data-ttu-id="a697a-118">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="a697a-118">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="a697a-119">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="a697a-119">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="a697a-120">Representa o usuário de caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="a697a-120">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="a697a-121">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a697a-121">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a697a-122">Text value</span><span class="sxs-lookup"><span data-stu-id="a697a-122">Text value</span></span>

<span data-ttu-id="a697a-123">Um valor de texto é opcional.</span><span class="sxs-lookup"><span data-stu-id="a697a-123">A text value is optional.</span></span> <span data-ttu-id="a697a-124">O único valor válido é SMTP.</span><span class="sxs-lookup"><span data-stu-id="a697a-124">The only valid value is SMTP.</span></span> <span data-ttu-id="a697a-125">Se nenhum valor for fornecido, o valor padrão do SMTP é usado.</span><span class="sxs-lookup"><span data-stu-id="a697a-125">If no value is provided, the default value of SMTP is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a697a-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="a697a-126">Remarks</span></span>

<span data-ttu-id="a697a-127">Esse elemento pode ocorrer no máximo uma vez no elemento de [Email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="a697a-127">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="a697a-128">Este elemento não é necessário.</span><span class="sxs-lookup"><span data-stu-id="a697a-128">This element is not required.</span></span> <span data-ttu-id="a697a-129">Este elemento existe para a inclusão de protocolos futuros.</span><span class="sxs-lookup"><span data-stu-id="a697a-129">This element exists for the inclusion of future protocols.</span></span> <span data-ttu-id="a697a-130">Outro elemento **RoutingType** é usado para acessar os itens na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a697a-130">Another **RoutingType** element is used for accessing items in a user's mailbox.</span></span> 
  
<span data-ttu-id="a697a-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a697a-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a697a-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a697a-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a697a-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a697a-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a697a-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a697a-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a697a-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a697a-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a697a-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a697a-136">Validation File</span></span>  <br/> |<span data-ttu-id="a697a-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a697a-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a697a-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a697a-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a697a-139">False</span><span class="sxs-lookup"><span data-stu-id="a697a-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a697a-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="a697a-140">See also</span></span>

- [<span data-ttu-id="a697a-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a697a-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="a697a-142">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="a697a-142">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="a697a-143">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a697a-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

