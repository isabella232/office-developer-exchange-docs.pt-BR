---
title: Domínio
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 7e45a061-856f-4b44-b053-a7c4d5ad569e
description: O elemento de domínio identifica um único domínio SMTP.
ms.openlocfilehash: 78eb1edfd347a513b84b9c15d143d76425041e85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751916"
---
# <a name="domain"></a><span data-ttu-id="71bab-103">Domínio</span><span class="sxs-lookup"><span data-stu-id="71bab-103">Domain</span></span>

<span data-ttu-id="71bab-104">O elemento de **domínio** identifica um único domínio SMTP.</span><span class="sxs-lookup"><span data-stu-id="71bab-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="71bab-105">**StmpDomain**</span><span class="sxs-lookup"><span data-stu-id="71bab-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71bab-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="71bab-106">Attributes and elements</span></span>

<span data-ttu-id="71bab-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="71bab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71bab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="71bab-108">Attributes</span></span>

|<span data-ttu-id="71bab-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="71bab-109">**Attribute**</span></span>|<span data-ttu-id="71bab-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71bab-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71bab-111">Nome</span><span class="sxs-lookup"><span data-stu-id="71bab-111">Name</span></span>  <br/> |<span data-ttu-id="71bab-112">Identifica o nome de um domínio.</span><span class="sxs-lookup"><span data-stu-id="71bab-112">Identifies the name of a domain.</span></span> <span data-ttu-id="71bab-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="71bab-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="71bab-114">IncludeSubdomains</span><span class="sxs-lookup"><span data-stu-id="71bab-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="71bab-115">Indica se os subdomínios do domínio identificado pelo atributo **Name** serão considerados internos.</span><span class="sxs-lookup"><span data-stu-id="71bab-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="71bab-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="71bab-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71bab-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="71bab-117">Child elements</span></span>

<span data-ttu-id="71bab-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="71bab-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71bab-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="71bab-119">Parent elements</span></span>

|<span data-ttu-id="71bab-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71bab-120">**Element**</span></span>|<span data-ttu-id="71bab-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71bab-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71bab-122">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="71bab-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="71bab-123">Identifica a lista de domínios de SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="71bab-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71bab-124">Text value</span><span class="sxs-lookup"><span data-stu-id="71bab-124">Text value</span></span>

<span data-ttu-id="71bab-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="71bab-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71bab-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="71bab-126">Remarks</span></span>

<span data-ttu-id="71bab-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="71bab-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71bab-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="71bab-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71bab-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="71bab-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71bab-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="71bab-130">Schema Name</span></span>  <br/> |<span data-ttu-id="71bab-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="71bab-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="71bab-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="71bab-132">Validation File</span></span>  <br/> |<span data-ttu-id="71bab-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71bab-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71bab-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="71bab-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="71bab-135">False</span><span class="sxs-lookup"><span data-stu-id="71bab-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71bab-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="71bab-136">See also</span></span>

- [<span data-ttu-id="71bab-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="71bab-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

