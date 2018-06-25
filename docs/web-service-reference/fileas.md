---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: O elemento FileAs representa como uma lista de contatos ou de distribuição é arquivada na pasta Contatos.
ms.openlocfilehash: dab9142eebf7691862e7970a7d1e8f5874393b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752249"
---
# <a name="fileas"></a><span data-ttu-id="b3431-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="b3431-103">FileAs</span></span>

<span data-ttu-id="b3431-104">O elemento **FileAs** representa como uma lista de contatos ou de distribuição é arquivada na pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="b3431-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="b3431-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="b3431-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3431-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b3431-106">Attributes and elements</span></span>

<span data-ttu-id="b3431-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b3431-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3431-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b3431-108">Attributes</span></span>

<span data-ttu-id="b3431-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b3431-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3431-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b3431-110">Child elements</span></span>

<span data-ttu-id="b3431-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b3431-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b3431-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b3431-112">Parent elements</span></span>

|<span data-ttu-id="b3431-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b3431-113">**Element**</span></span>|<span data-ttu-id="b3431-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b3431-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3431-115">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b3431-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b3431-116">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="b3431-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="b3431-117">Contato</span><span class="sxs-lookup"><span data-stu-id="b3431-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b3431-118">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3431-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3431-119">Text value</span><span class="sxs-lookup"><span data-stu-id="b3431-119">Text value</span></span>

<span data-ttu-id="b3431-120">Se este elemento for usado, será necessário um valor de texto que representa uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b3431-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b3431-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="b3431-121">Remarks</span></span>

<span data-ttu-id="b3431-122">O elemento **FileAs** é usado para classificar os contatos e listas de distribuição por um nome que não seja um nome completo ou empresa.</span><span class="sxs-lookup"><span data-stu-id="b3431-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="b3431-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b3431-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3431-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b3431-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3431-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b3431-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3431-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b3431-126">Schema name</span></span>  <br/> |<span data-ttu-id="b3431-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b3431-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b3431-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b3431-128">Validation file</span></span>  <br/> |<span data-ttu-id="b3431-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b3431-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3431-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b3431-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b3431-131">False</span><span class="sxs-lookup"><span data-stu-id="b3431-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3431-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="b3431-132">See also</span></span>



- [<span data-ttu-id="b3431-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b3431-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

