---
title: Email (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: O elemento de Email representa o usuário de caixa de correio para uma consulta GetUserAvailability.
ms.openlocfilehash: 0e7848d7c4f5001ed86b06d11af1d7623b4bf1f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751979"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="d46e9-103">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d46e9-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="d46e9-104">O elemento de **Email** representa o usuário de caixa de correio para uma consulta GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="d46e9-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="d46e9-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d46e9-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="d46e9-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="d46e9-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="d46e9-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="d46e9-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="d46e9-108">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d46e9-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="d46e9-109">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="d46e9-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d46e9-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d46e9-110">Attributes and elements</span></span>

<span data-ttu-id="d46e9-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d46e9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d46e9-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="d46e9-112">Attributes</span></span>

<span data-ttu-id="d46e9-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d46e9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d46e9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d46e9-114">Child elements</span></span>

|<span data-ttu-id="d46e9-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d46e9-115">**Element**</span></span>|<span data-ttu-id="d46e9-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d46e9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d46e9-117">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d46e9-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="d46e9-118">Representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d46e9-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="d46e9-119">Endereço (string)</span><span class="sxs-lookup"><span data-stu-id="d46e9-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="d46e9-120">Representa o endereço de email do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d46e9-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="d46e9-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d46e9-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="d46e9-122">Representa o protocolo de roteamento para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d46e9-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d46e9-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d46e9-123">Parent elements</span></span>

|<span data-ttu-id="d46e9-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d46e9-124">**Element**</span></span>|<span data-ttu-id="d46e9-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d46e9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d46e9-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="d46e9-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="d46e9-127">Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d46e9-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="d46e9-128">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="d46e9-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d46e9-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="d46e9-129">Remarks</span></span>

<span data-ttu-id="d46e9-130">O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d46e9-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d46e9-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d46e9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d46e9-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="d46e9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d46e9-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d46e9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d46e9-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d46e9-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d46e9-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d46e9-135">Validation File</span></span>  <br/> |<span data-ttu-id="d46e9-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d46e9-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d46e9-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d46e9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d46e9-138">False</span><span class="sxs-lookup"><span data-stu-id="d46e9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d46e9-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="d46e9-139">See also</span></span>

- [<span data-ttu-id="d46e9-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d46e9-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="d46e9-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d46e9-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="d46e9-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="d46e9-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

