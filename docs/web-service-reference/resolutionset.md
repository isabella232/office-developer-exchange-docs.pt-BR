---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: O elemento ResolutionSet contém uma matriz de resoluções para um nome ambíguo.
ms.openlocfilehash: 483a096a7fcedbabe25758ebcaa31c83405a0ad4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467169"
---
# <a name="resolutionset"></a><span data-ttu-id="12bae-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="12bae-103">ResolutionSet</span></span>

<span data-ttu-id="12bae-104">O elemento **ResolutionSet** contém uma matriz de resoluções para um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="12bae-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="12bae-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="12bae-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="12bae-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="12bae-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="12bae-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="12bae-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="12bae-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="12bae-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="12bae-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="12bae-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12bae-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="12bae-110">Attributes and elements</span></span>

<span data-ttu-id="12bae-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="12bae-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12bae-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="12bae-112">Attributes</span></span>

|<span data-ttu-id="12bae-113">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="12bae-113">**Attribute**</span></span>|<span data-ttu-id="12bae-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12bae-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="12bae-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="12bae-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="12bae-116">Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexado.</span><span class="sxs-lookup"><span data-stu-id="12bae-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="12bae-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="12bae-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="12bae-118">Representa o novo valor do numerador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="12bae-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="12bae-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="12bae-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="12bae-120">Representa o próximo denominador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="12bae-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="12bae-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="12bae-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="12bae-122">Esse atributo será true se os resultados atuais contiverem o último item na consulta, para que a paginação adicional não seja necessária.</span><span class="sxs-lookup"><span data-stu-id="12bae-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="12bae-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="12bae-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="12bae-124">Representa o número total de itens no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="12bae-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="12bae-125">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="12bae-125">Child elements</span></span>

|<span data-ttu-id="12bae-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12bae-126">**Element**</span></span>|<span data-ttu-id="12bae-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12bae-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12bae-128">Resolução</span><span class="sxs-lookup"><span data-stu-id="12bae-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="12bae-129">Contém uma única entidade resolvida.</span><span class="sxs-lookup"><span data-stu-id="12bae-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12bae-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="12bae-130">Parent elements</span></span>

|<span data-ttu-id="12bae-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12bae-131">**Element**</span></span>|<span data-ttu-id="12bae-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12bae-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12bae-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="12bae-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="12bae-134">Contém o status e o resultado de uma solicitação ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="12bae-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="12bae-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="12bae-135">Remarks</span></span>

<span data-ttu-id="12bae-136">Um elemento **ResolutionSet** pode conter um máximo de 100 entidades resolvidas.</span><span class="sxs-lookup"><span data-stu-id="12bae-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="12bae-137">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="12bae-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12bae-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="12bae-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12bae-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="12bae-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="12bae-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="12bae-140">Schema Name</span></span>  <br/> |<span data-ttu-id="12bae-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="12bae-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="12bae-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="12bae-142">Validation File</span></span>  <br/> |<span data-ttu-id="12bae-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="12bae-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12bae-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="12bae-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="12bae-145">False</span><span class="sxs-lookup"><span data-stu-id="12bae-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12bae-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="12bae-146">See also</span></span>



[<span data-ttu-id="12bae-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="12bae-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="12bae-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="12bae-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="12bae-149">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="12bae-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="12bae-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="12bae-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

