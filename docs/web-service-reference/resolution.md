---
title: Resolução
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Resolution
api_type:
- schema
ms.assetid: 573bed4b-d7b1-4baf-b16f-0795cdebf1a7
description: O elemento Resolution contém uma única entidade resolvida.
ms.openlocfilehash: 63c80f3c8d7dabf7e6dc1494df04c0be821b28bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468282"
---
# <a name="resolution"></a><span data-ttu-id="3909e-103">Resolução</span><span class="sxs-lookup"><span data-stu-id="3909e-103">Resolution</span></span>

<span data-ttu-id="3909e-104">O elemento **Resolution** contém uma única entidade resolvida.</span><span class="sxs-lookup"><span data-stu-id="3909e-104">The **Resolution** element contains a single resolved entity.</span></span> 
  
[<span data-ttu-id="3909e-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="3909e-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="3909e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3909e-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="3909e-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3909e-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="3909e-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="3909e-108">ResolutionSet</span></span>](resolutionset.md)
  
[<span data-ttu-id="3909e-109">Resolução</span><span class="sxs-lookup"><span data-stu-id="3909e-109">Resolution</span></span>](resolution.md)
  
```xml
<Resolution>
   <Mailbox/>
   <Contact/>
</Resolution>
```

 <span data-ttu-id="3909e-110">**ResolutionType**</span><span class="sxs-lookup"><span data-stu-id="3909e-110">**ResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3909e-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3909e-111">Attributes and elements</span></span>

<span data-ttu-id="3909e-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3909e-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3909e-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="3909e-113">Attributes</span></span>

<span data-ttu-id="3909e-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3909e-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3909e-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3909e-115">Child elements</span></span>

|<span data-ttu-id="3909e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3909e-116">**Element**</span></span>|<span data-ttu-id="3909e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3909e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3909e-118">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="3909e-118">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3909e-119">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="3909e-119">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
|[<span data-ttu-id="3909e-120">Contato</span><span class="sxs-lookup"><span data-stu-id="3909e-120">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3909e-121">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3909e-121">Represents an Exchange contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3909e-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3909e-122">Parent elements</span></span>

|<span data-ttu-id="3909e-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3909e-123">**Element**</span></span>|<span data-ttu-id="3909e-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3909e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3909e-125">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="3909e-125">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="3909e-126">Contém uma matriz de resoluções para um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="3909e-126">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3909e-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="3909e-127">Remarks</span></span>

<span data-ttu-id="3909e-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3909e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3909e-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3909e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3909e-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="3909e-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3909e-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3909e-131">Schema name</span></span>  <br/> |<span data-ttu-id="3909e-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3909e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3909e-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3909e-133">Validation file</span></span>  <br/> |<span data-ttu-id="3909e-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3909e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3909e-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3909e-135">Can be empty</span></span>  <br/> |<span data-ttu-id="3909e-136">False</span><span class="sxs-lookup"><span data-stu-id="3909e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3909e-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="3909e-137">See also</span></span>



[<span data-ttu-id="3909e-138">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="3909e-138">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="3909e-139">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="3909e-139">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="3909e-140">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="3909e-140">ResolveNames operation</span></span>](resolvenames-operation.md)

