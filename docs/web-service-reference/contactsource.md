---
title: ContactSource
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
description: O elemento ContactSource descreve se o contato está localizado no armazenamento do Exchange ou os serviços de domínio Active Directory (AD DS).
ms.openlocfilehash: a82b766fc81b9397fc707415ea82e2f2d63d952d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751451"
---
# <a name="contactsource"></a><span data-ttu-id="d90ec-103">ContactSource</span><span class="sxs-lookup"><span data-stu-id="d90ec-103">ContactSource</span></span>

<span data-ttu-id="d90ec-104">O elemento **ContactSource** descreve se o contato está localizado no armazenamento do Exchange ou os serviços de domínio Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="d90ec-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="d90ec-105">**ContactSourceType**</span><span class="sxs-lookup"><span data-stu-id="d90ec-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d90ec-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d90ec-106">Attributes and elements</span></span>

<span data-ttu-id="d90ec-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d90ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d90ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d90ec-108">Attributes</span></span>

<span data-ttu-id="d90ec-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d90ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d90ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d90ec-110">Child elements</span></span>

<span data-ttu-id="d90ec-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d90ec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d90ec-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d90ec-112">Parent elements</span></span>

|<span data-ttu-id="d90ec-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d90ec-113">**Element**</span></span>|<span data-ttu-id="d90ec-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d90ec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d90ec-115">Contato</span><span class="sxs-lookup"><span data-stu-id="d90ec-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d90ec-116">Representa um item de contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d90ec-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d90ec-117">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d90ec-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d90ec-118">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="d90ec-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d90ec-119">Text value</span><span class="sxs-lookup"><span data-stu-id="d90ec-119">Text value</span></span>

<span data-ttu-id="d90ec-120">Estes são os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d90ec-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="d90ec-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="d90ec-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="d90ec-122">Repositório</span><span class="sxs-lookup"><span data-stu-id="d90ec-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="d90ec-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="d90ec-123">Remarks</span></span>

<span data-ttu-id="d90ec-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d90ec-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d90ec-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d90ec-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d90ec-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d90ec-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d90ec-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d90ec-127">Schema name</span></span>  <br/> |<span data-ttu-id="d90ec-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d90ec-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d90ec-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d90ec-129">Validation file</span></span>  <br/> |<span data-ttu-id="d90ec-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d90ec-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d90ec-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d90ec-131">Can be empty</span></span>  <br/> |<span data-ttu-id="d90ec-132">False</span><span class="sxs-lookup"><span data-stu-id="d90ec-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d90ec-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="d90ec-133">See also</span></span>



- [<span data-ttu-id="d90ec-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d90ec-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

