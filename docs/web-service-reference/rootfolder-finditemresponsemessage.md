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
description: O elemento RootFolder contém os resultados de uma pesquisa de uma pasta raiz única durante uma operação FindItem.
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825254"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="0857d-103">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="0857d-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="0857d-104">O elemento **RootFolder** contém os resultados de uma pesquisa de uma pasta raiz única durante uma [operação FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0857d-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="0857d-105">**FindItemParentType**</span><span class="sxs-lookup"><span data-stu-id="0857d-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0857d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0857d-106">Attributes and elements</span></span>

<span data-ttu-id="0857d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0857d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0857d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0857d-108">Attributes</span></span>

|<span data-ttu-id="0857d-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0857d-109">**Attribute**</span></span>|<span data-ttu-id="0857d-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0857d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0857d-111">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="0857d-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="0857d-112">Representa o próximo índice que deve ser usado para a próxima solicitação ao usar o modo de exibição indexada paginação.</span><span class="sxs-lookup"><span data-stu-id="0857d-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="0857d-113">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="0857d-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="0857d-114">Representa o novo valor numerador usada para a próxima solicitação quando usar exibições de página de fração.</span><span class="sxs-lookup"><span data-stu-id="0857d-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="0857d-115">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="0857d-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="0857d-116">Representa o denominador próximo a ser usado para a próxima solicitação ao fazer a paginação fracional.</span><span class="sxs-lookup"><span data-stu-id="0857d-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="0857d-117">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="0857d-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="0857d-118">Indica se os resultados atuais contêm o último item na consulta, de forma que não seja necessário paginação ainda mais.</span><span class="sxs-lookup"><span data-stu-id="0857d-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="0857d-119">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="0857d-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="0857d-120">Representa o número total de itens que passam a restrição.</span><span class="sxs-lookup"><span data-stu-id="0857d-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="0857d-121">Em uma [operação FindItem](finditem-operation.md)agrupada, o atributo **TotalItemsInView** retorna o número total de itens no modo de exibição mais o número total de grupos.</span><span class="sxs-lookup"><span data-stu-id="0857d-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0857d-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0857d-122">Child elements</span></span>

|<span data-ttu-id="0857d-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0857d-123">**Element**</span></span>|<span data-ttu-id="0857d-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0857d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0857d-125">Items</span><span class="sxs-lookup"><span data-stu-id="0857d-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="0857d-126">Contém uma matriz de itens encontrados com os critérios de pesquisa identificados na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0857d-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0857d-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="0857d-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="0857d-128">Contém uma coleção dos grupos encontrados que tenham os critérios de pesquisa e a agregação de lista segura identificados na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0857d-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0857d-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0857d-129">Parent elements</span></span>

|<span data-ttu-id="0857d-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0857d-130">**Element**</span></span>|<span data-ttu-id="0857d-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0857d-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0857d-132">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0857d-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="0857d-133">Contém o status e o resultado de uma solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0857d-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0857d-134">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0857d-134">Remarks</span></span>

<span data-ttu-id="0857d-135">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0857d-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0857d-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0857d-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0857d-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="0857d-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0857d-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0857d-138">Schema name</span></span>  <br/> |<span data-ttu-id="0857d-139">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0857d-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0857d-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0857d-140">Validation file</span></span>  <br/> |<span data-ttu-id="0857d-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0857d-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0857d-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0857d-142">Can be empty</span></span>  <br/> |<span data-ttu-id="0857d-143">False</span><span class="sxs-lookup"><span data-stu-id="0857d-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0857d-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="0857d-144">See also</span></span>



[<span data-ttu-id="0857d-145">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="0857d-145">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="0857d-146">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="0857d-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="0857d-147">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="0857d-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="0857d-148">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="0857d-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="0857d-149">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="0857d-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="0857d-150">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="0857d-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="0857d-151">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="0857d-151">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

