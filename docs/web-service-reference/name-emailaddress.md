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
description: O elemento name representa o nome de exibição do usuário da caixa de correio.
ms.openlocfilehash: 2c6b29f1b069f9cc72ac84e7aebfff99437e630a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466952"
---
# <a name="name-emailaddress"></a><span data-ttu-id="a467d-103">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a467d-103">Name (EmailAddress)</span></span>

<span data-ttu-id="a467d-104">O elemento **Name** representa o nome de exibição do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a467d-104">The **Name** element represents the display name of the mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="a467d-105">**String**</span><span class="sxs-lookup"><span data-stu-id="a467d-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a467d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a467d-106">Attributes and elements</span></span>

<span data-ttu-id="a467d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a467d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a467d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a467d-108">Attributes</span></span>

<span data-ttu-id="a467d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a467d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a467d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a467d-110">Child elements</span></span>

<span data-ttu-id="a467d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a467d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a467d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a467d-112">Parent elements</span></span>

|<span data-ttu-id="a467d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a467d-113">**Element**</span></span>|<span data-ttu-id="a467d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a467d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a467d-115">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="a467d-115">Email (EmailAddressType)</span></span>](email-emailaddresstype.md) <br/> |<span data-ttu-id="a467d-116">Representa o usuário de caixa de correio de uma consulta GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="a467d-116">Represents the mailbox user for a GetUserAvailability query.</span></span>  <br/> <br/><span data-ttu-id="a467d-117">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a467d-117">The following is the XPath to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[<span data-ttu-id="a467d-118">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="a467d-118">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> | <span data-ttu-id="a467d-119">Representa o usuário de caixa de correio de uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="a467d-119">Represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/><br/>  <span data-ttu-id="a467d-120">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a467d-120">The following are the XPath expressions to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a467d-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a467d-121">Text value</span></span>

<span data-ttu-id="a467d-122">Um valor de texto será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="a467d-122">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a467d-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a467d-123">Remarks</span></span>

<span data-ttu-id="a467d-124">Esse elemento pode ocorrer no máximo uma vez no elemento [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="a467d-124">This element can occur at most one time in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="a467d-125">Esse elemento não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a467d-125">This element is not required.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a467d-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a467d-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a467d-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a467d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a467d-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="a467d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a467d-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a467d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="a467d-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a467d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a467d-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a467d-131">Validation File</span></span>  <br/> |<span data-ttu-id="a467d-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a467d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a467d-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a467d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="a467d-134">False</span><span class="sxs-lookup"><span data-stu-id="a467d-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a467d-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="a467d-135">See also</span></span>

- [<span data-ttu-id="a467d-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a467d-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="a467d-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="a467d-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="a467d-138">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a467d-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

