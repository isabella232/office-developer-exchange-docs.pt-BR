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
description: O elemento FileAs representa como um contato ou uma lista de distribuição é arquivado na pasta contatos.
ms.openlocfilehash: be756d86d7608fcb758dd54f2ada9f03a04343e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461195"
---
# <a name="fileas"></a><span data-ttu-id="be551-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="be551-103">FileAs</span></span>

<span data-ttu-id="be551-104">O elemento **FileAs** representa como um contato ou uma lista de distribuição é arquivado na pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="be551-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="be551-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="be551-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be551-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="be551-106">Attributes and elements</span></span>

<span data-ttu-id="be551-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="be551-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be551-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="be551-108">Attributes</span></span>

<span data-ttu-id="be551-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be551-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be551-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="be551-110">Child elements</span></span>

<span data-ttu-id="be551-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be551-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be551-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="be551-112">Parent elements</span></span>

|<span data-ttu-id="be551-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="be551-113">**Element**</span></span>|<span data-ttu-id="be551-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be551-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be551-115">DistributionList</span><span class="sxs-lookup"><span data-stu-id="be551-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="be551-116">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="be551-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="be551-117">Contato</span><span class="sxs-lookup"><span data-stu-id="be551-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="be551-118">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be551-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be551-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="be551-119">Text value</span></span>

<span data-ttu-id="be551-120">Um valor de texto que representa uma cadeia de caracteres será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="be551-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be551-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="be551-121">Remarks</span></span>

<span data-ttu-id="be551-122">O elemento **FileAs** é usado para classificar contatos e listas de distribuição por um nome diferente de um nome completo ou nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="be551-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="be551-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="be551-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be551-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="be551-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be551-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="be551-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be551-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="be551-126">Schema name</span></span>  <br/> |<span data-ttu-id="be551-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="be551-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="be551-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="be551-128">Validation file</span></span>  <br/> |<span data-ttu-id="be551-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="be551-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be551-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="be551-130">Can be empty</span></span>  <br/> |<span data-ttu-id="be551-131">False</span><span class="sxs-lookup"><span data-stu-id="be551-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be551-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="be551-132">See also</span></span>



- [<span data-ttu-id="be551-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be551-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

