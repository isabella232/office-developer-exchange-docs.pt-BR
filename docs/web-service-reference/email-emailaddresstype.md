---
title: Email (EmailAddresstype)
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
description: O elemento email representa o usuário de caixa de correio de uma consulta GetUserAvailability.
ms.openlocfilehash: 2ed8de9c011a385ec6c4ebd2f8d1d47304343a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459227"
---
# <a name="email-emailaddresstype"></a><span data-ttu-id="20d49-103">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="20d49-103">Email (EmailAddressType)</span></span>

<span data-ttu-id="20d49-104">O elemento **email** representa o usuário de caixa de correio de uma consulta GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="20d49-104">The **Email** element represents the mailbox user for a GetUserAvailability query.</span></span> 
  
- [<span data-ttu-id="20d49-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="20d49-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)  
- [<span data-ttu-id="20d49-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="20d49-106">MailboxDataArray</span></span>](mailboxdataarray.md) 
- [<span data-ttu-id="20d49-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="20d49-107">MailboxData</span></span>](mailboxdata.md) 
- [<span data-ttu-id="20d49-108">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="20d49-108">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 <span data-ttu-id="20d49-109">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="20d49-109">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20d49-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="20d49-110">Attributes and elements</span></span>

<span data-ttu-id="20d49-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="20d49-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20d49-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="20d49-112">Attributes</span></span>

<span data-ttu-id="20d49-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20d49-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20d49-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="20d49-114">Child elements</span></span>

|<span data-ttu-id="20d49-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="20d49-115">**Element**</span></span>|<span data-ttu-id="20d49-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="20d49-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20d49-117">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="20d49-117">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="20d49-118">Representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="20d49-118">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="20d49-119">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="20d49-119">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="20d49-120">Representa o endereço de email do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="20d49-120">Represents the e-mail address of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="20d49-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="20d49-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="20d49-122">Representa o protocolo de roteamento para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="20d49-122">Represents the routing protocol for the message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20d49-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="20d49-123">Parent elements</span></span>

|<span data-ttu-id="20d49-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="20d49-124">**Element**</span></span>|<span data-ttu-id="20d49-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="20d49-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20d49-126">MailboxData</span><span class="sxs-lookup"><span data-stu-id="20d49-126">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="20d49-127">Representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="20d49-127">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="20d49-128">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="20d49-128">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="20d49-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="20d49-129">Remarks</span></span>

<span data-ttu-id="20d49-130">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="20d49-130">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20d49-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="20d49-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20d49-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="20d49-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20d49-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="20d49-133">Schema Name</span></span>  <br/> |<span data-ttu-id="20d49-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="20d49-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="20d49-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="20d49-135">Validation File</span></span>  <br/> |<span data-ttu-id="20d49-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="20d49-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20d49-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="20d49-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="20d49-138">False</span><span class="sxs-lookup"><span data-stu-id="20d49-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20d49-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="20d49-139">See also</span></span>

- [<span data-ttu-id="20d49-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="20d49-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="20d49-141">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="20d49-141">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="20d49-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="20d49-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

