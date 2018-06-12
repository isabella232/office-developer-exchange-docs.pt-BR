---
title: EmailAddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20049467-c01a-4c7d-8ada-ca1801cc95ed
description: O elemento EmailAddressEntity Especifica uma entidade de endereço de email único.
ms.openlocfilehash: c149ee69c1ed08c33d0341c8dfdac3bcda040afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752000"
---
# <a name="emailaddressentity"></a><span data-ttu-id="d8517-103">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="d8517-103">EmailAddressEntity</span></span>

<span data-ttu-id="d8517-104">O elemento **EmailAddressEntity** Especifica uma entidade de endereço de email único.</span><span class="sxs-lookup"><span data-stu-id="d8517-104">The **EmailAddressEntity** element specifies a single email address entity.</span></span> 
  
```XML
<EmailAddressEntity>
    <EmailAddress></EmailAddress>
</EmailAddressEntity>
```

 <span data-ttu-id="d8517-105">**EmailAddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="d8517-105">**EmailAddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8517-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d8517-106">Attributes and elements</span></span>

<span data-ttu-id="d8517-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8517-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8517-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8517-108">Attributes</span></span>

<span data-ttu-id="d8517-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8517-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8517-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8517-110">Child elements</span></span>

|<span data-ttu-id="d8517-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8517-111">**Element**</span></span>|<span data-ttu-id="d8517-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8517-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8517-113">EmailAddress (string)</span><span class="sxs-lookup"><span data-stu-id="d8517-113">EmailAddress (string)</span></span>](emailaddress-string.md) <br/> |<span data-ttu-id="d8517-114">Especifica um endereço de email único.</span><span class="sxs-lookup"><span data-stu-id="d8517-114">Specifies a single email address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8517-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8517-115">Parent elements</span></span>

|<span data-ttu-id="d8517-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8517-116">**Element**</span></span>|<span data-ttu-id="d8517-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8517-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8517-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="d8517-118">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="d8517-119">Especifica uma matriz de entidades de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d8517-119">Specifies an array of email address entities.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8517-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d8517-120">Remarks</span></span>

<span data-ttu-id="d8517-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8517-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8517-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8517-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8517-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d8517-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8517-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8517-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8517-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d8517-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d8517-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="d8517-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d8517-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d8517-127">Validation File</span></span>  <br/> |<span data-ttu-id="d8517-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8517-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8517-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d8517-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d8517-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="d8517-130">See also</span></span>



- [<span data-ttu-id="d8517-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d8517-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

