---
title: Contato
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactSource
api_type:
- schema
ms.assetid: 500b0423-864e-4cde-a39b-6b5b06d1aa6a
description: O elemento ContactName descreve se o contato está localizado no repositório do Exchange ou nos serviços de domínio do Active Directory (AD DS).
ms.openlocfilehash: 5447dedf199c5ad6b944aa33e6dca03e83a3c340
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462707"
---
# <a name="contactsource"></a><span data-ttu-id="a6d50-103">Contato</span><span class="sxs-lookup"><span data-stu-id="a6d50-103">ContactSource</span></span>

<span data-ttu-id="a6d50-104">O elemento **ContactName** descreve se o contato está localizado no repositório do Exchange ou nos serviços de domínio do Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="a6d50-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="a6d50-105">**ContactSourceType**</span><span class="sxs-lookup"><span data-stu-id="a6d50-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6d50-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a6d50-106">Attributes and elements</span></span>

<span data-ttu-id="a6d50-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a6d50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6d50-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a6d50-108">Attributes</span></span>

<span data-ttu-id="a6d50-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6d50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6d50-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a6d50-110">Child elements</span></span>

<span data-ttu-id="a6d50-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a6d50-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6d50-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a6d50-112">Parent elements</span></span>

|<span data-ttu-id="a6d50-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a6d50-113">**Element**</span></span>|<span data-ttu-id="a6d50-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a6d50-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6d50-115">Contato</span><span class="sxs-lookup"><span data-stu-id="a6d50-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="a6d50-116">Representa um item de contato no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6d50-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a6d50-117">DistributionList</span><span class="sxs-lookup"><span data-stu-id="a6d50-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="a6d50-118">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="a6d50-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6d50-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a6d50-119">Text value</span></span>

<span data-ttu-id="a6d50-120">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a6d50-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="a6d50-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="a6d50-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="a6d50-122">Repositório</span><span class="sxs-lookup"><span data-stu-id="a6d50-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="a6d50-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a6d50-123">Remarks</span></span>

<span data-ttu-id="a6d50-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6d50-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6d50-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a6d50-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6d50-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a6d50-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6d50-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a6d50-127">Schema name</span></span>  <br/> |<span data-ttu-id="a6d50-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a6d50-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6d50-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a6d50-129">Validation file</span></span>  <br/> |<span data-ttu-id="a6d50-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a6d50-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6d50-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a6d50-131">Can be empty</span></span>  <br/> |<span data-ttu-id="a6d50-132">False</span><span class="sxs-lookup"><span data-stu-id="a6d50-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6d50-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="a6d50-133">See also</span></span>



- [<span data-ttu-id="a6d50-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a6d50-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

