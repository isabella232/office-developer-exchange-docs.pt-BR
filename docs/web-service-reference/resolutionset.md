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
description: O elemento ResolutionSet contém uma matriz de resoluções referentes a um nome ambíguo.
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825160"
---
# <a name="resolutionset"></a><span data-ttu-id="a1a29-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="a1a29-103">ResolutionSet</span></span>

<span data-ttu-id="a1a29-104">O elemento **ResolutionSet** contém uma matriz de resoluções referentes a um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="a1a29-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="a1a29-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="a1a29-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="a1a29-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a1a29-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="a1a29-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a1a29-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="a1a29-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="a1a29-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="a1a29-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="a1a29-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1a29-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a1a29-110">Attributes and elements</span></span>

<span data-ttu-id="a1a29-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a1a29-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1a29-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a1a29-112">Attributes</span></span>

|<span data-ttu-id="a1a29-113">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a1a29-113">**Attribute**</span></span>|<span data-ttu-id="a1a29-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a1a29-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a1a29-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="a1a29-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="a1a29-116">Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexados.</span><span class="sxs-lookup"><span data-stu-id="a1a29-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="a1a29-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="a1a29-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="a1a29-118">Representa o novo valor numerador a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="a1a29-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="a1a29-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="a1a29-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="a1a29-120">Representa o denominador próximo a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="a1a29-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="a1a29-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="a1a29-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="a1a29-122">Este atributo será true se os resultados atuais contêm o último item na consulta, para que a paginação adicional não é necessária.</span><span class="sxs-lookup"><span data-stu-id="a1a29-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="a1a29-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="a1a29-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="a1a29-124">Representa o número total de itens no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="a1a29-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a1a29-125">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a1a29-125">Child elements</span></span>

|<span data-ttu-id="a1a29-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a1a29-126">**Element**</span></span>|<span data-ttu-id="a1a29-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a1a29-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1a29-128">Resolução</span><span class="sxs-lookup"><span data-stu-id="a1a29-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="a1a29-129">Contém uma única entidade resolvida.</span><span class="sxs-lookup"><span data-stu-id="a1a29-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1a29-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a1a29-130">Parent elements</span></span>

|<span data-ttu-id="a1a29-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a1a29-131">**Element**</span></span>|<span data-ttu-id="a1a29-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a1a29-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1a29-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a1a29-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="a1a29-134">Contém o status e o resultado de uma solicitação de ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="a1a29-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a1a29-135">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a1a29-135">Remarks</span></span>

<span data-ttu-id="a1a29-136">Um elemento **ResolutionSet** pode conter no máximo 100 entidades resolvidos.</span><span class="sxs-lookup"><span data-stu-id="a1a29-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="a1a29-137">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a1a29-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1a29-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a1a29-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1a29-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="a1a29-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1a29-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a1a29-140">Schema Name</span></span>  <br/> |<span data-ttu-id="a1a29-141">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a1a29-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1a29-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a1a29-142">Validation File</span></span>  <br/> |<span data-ttu-id="a1a29-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a1a29-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1a29-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a1a29-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1a29-145">False</span><span class="sxs-lookup"><span data-stu-id="a1a29-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1a29-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="a1a29-146">See also</span></span>



[<span data-ttu-id="a1a29-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a1a29-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="a1a29-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="a1a29-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="a1a29-149">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a1a29-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="a1a29-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a1a29-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

