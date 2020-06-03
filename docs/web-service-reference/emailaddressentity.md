---
title: EmailAddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: O elemento EmailAddressEntity especifica uma única entidade de endereço de email.
ms.openlocfilehash: b76b08f93e60c8492906f3cc94e60f5725c8a9dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526218"
---
# <a name="emailaddressentity"></a><span data-ttu-id="38505-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="38505-103">EmailAddressEntity</span></span>

<span data-ttu-id="38505-104">O elemento **EmailAddressEntity** especifica uma única entidade de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="38505-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="38505-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="38505-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38505-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="38505-106">Attributes and elements</span></span>

<span data-ttu-id="38505-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="38505-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38505-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="38505-108">Attributes</span></span>

<span data-ttu-id="38505-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38505-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38505-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="38505-110">Child elements</span></span>

|<span data-ttu-id="38505-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38505-111">**Element**</span></span>|<span data-ttu-id="38505-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38505-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38505-113">EmailAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="38505-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="38505-114">Especifica um único endereço de email.</span><span class="sxs-lookup"><span data-stu-id="38505-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38505-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="38505-115">Parent elements</span></span>

|<span data-ttu-id="38505-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38505-116">**Element**</span></span>|<span data-ttu-id="38505-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38505-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38505-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="38505-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="38505-119">Especifica uma matriz de entidades de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="38505-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38505-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="38505-120">Remarks</span></span>

<span data-ttu-id="38505-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="38505-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="38505-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="38505-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38505-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="38505-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38505-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="38505-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38505-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="38505-125">Schema Name</span></span>  <br/> |<span data-ttu-id="38505-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="38505-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="38505-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="38505-127">Validation File</span></span>  <br/> |<span data-ttu-id="38505-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="38505-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="38505-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="38505-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="38505-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="38505-130">See also</span></span>



- [<span data-ttu-id="38505-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="38505-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

