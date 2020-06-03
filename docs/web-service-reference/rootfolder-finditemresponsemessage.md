---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: O elemento RootFolder contém os resultados de uma pesquisa de uma única pasta raiz durante uma operação FindItem.
ms.openlocfilehash: 3bbab325dff26139739c50ef519b215aea620a0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457127"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="35ad6-103">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="35ad6-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="35ad6-104">O elemento **RootFolder** contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="35ad6-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="35ad6-105">**FindItemParentType**</span><span class="sxs-lookup"><span data-stu-id="35ad6-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35ad6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="35ad6-106">Attributes and elements</span></span>

<span data-ttu-id="35ad6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="35ad6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35ad6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="35ad6-108">Attributes</span></span>

|<span data-ttu-id="35ad6-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="35ad6-109">**Attribute**</span></span>|<span data-ttu-id="35ad6-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="35ad6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="35ad6-111">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="35ad6-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="35ad6-112">Representa o próximo índice que deve ser usado para a próxima solicitação ao usar um modo de exibição de paginação indexado.</span><span class="sxs-lookup"><span data-stu-id="35ad6-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="35ad6-113">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="35ad6-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="35ad6-114">Representa o novo valor do numerador a ser usado para a próxima solicitação ao usar as exibições da página de fração.</span><span class="sxs-lookup"><span data-stu-id="35ad6-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="35ad6-115">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="35ad6-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="35ad6-116">Representa o próximo denominador a ser usado para a próxima solicitação ao fazer paginação fracionária.</span><span class="sxs-lookup"><span data-stu-id="35ad6-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="35ad6-117">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="35ad6-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="35ad6-118">Indica se os resultados atuais contêm o último item da consulta, de modo que a paginação adicional não será necessária.</span><span class="sxs-lookup"><span data-stu-id="35ad6-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="35ad6-119">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="35ad6-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="35ad6-120">Representa o número total de itens que passam a restrição.</span><span class="sxs-lookup"><span data-stu-id="35ad6-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="35ad6-121">Em uma [operação FindItem](finditem-operation.md)agrupada, o atributo **TotalItemsInView** retorna o número total de itens no modo de exibição mais o número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="35ad6-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="35ad6-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="35ad6-122">Child elements</span></span>

|<span data-ttu-id="35ad6-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="35ad6-123">**Element**</span></span>|<span data-ttu-id="35ad6-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="35ad6-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ad6-125">Itens</span><span class="sxs-lookup"><span data-stu-id="35ad6-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="35ad6-126">Contém uma matriz de itens encontrados que têm os critérios de pesquisa identificados na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="35ad6-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="35ad6-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="35ad6-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="35ad6-128">Contém uma coleção de grupos encontrados que têm os critérios de pesquisa e agregação identificados na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="35ad6-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35ad6-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="35ad6-129">Parent elements</span></span>

|<span data-ttu-id="35ad6-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="35ad6-130">**Element**</span></span>|<span data-ttu-id="35ad6-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="35ad6-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35ad6-132">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="35ad6-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="35ad6-133">Contém o status e o resultado de uma solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="35ad6-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="35ad6-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="35ad6-134">Remarks</span></span>

<span data-ttu-id="35ad6-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="35ad6-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35ad6-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="35ad6-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35ad6-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="35ad6-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="35ad6-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="35ad6-138">Schema name</span></span>  <br/> |<span data-ttu-id="35ad6-139">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="35ad6-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="35ad6-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="35ad6-140">Validation file</span></span>  <br/> |<span data-ttu-id="35ad6-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="35ad6-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="35ad6-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="35ad6-142">Can be empty</span></span>  <br/> |<span data-ttu-id="35ad6-143">False</span><span class="sxs-lookup"><span data-stu-id="35ad6-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35ad6-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="35ad6-144">See also</span></span>



[<span data-ttu-id="35ad6-145">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="35ad6-145">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="35ad6-146">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="35ad6-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="35ad6-147">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="35ad6-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="35ad6-148">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="35ad6-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="35ad6-149">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="35ad6-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="35ad6-150">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="35ad6-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="35ad6-151">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="35ad6-151">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

