---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: O elemento FindItem define uma solicitação para localizar itens em uma caixa de correio.
ms.openlocfilehash: 3aeda1cffc03292734a91bc3fff3289d51c9b445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460992"
---
# <a name="finditem"></a><span data-ttu-id="e8515-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="e8515-103">FindItem</span></span>

<span data-ttu-id="e8515-104">O elemento **FindItem** define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e8515-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


<span data-ttu-id="e8515-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="e8515-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e8515-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e8515-106">Attributes and elements</span></span>

<span data-ttu-id="e8515-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e8515-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8515-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e8515-108">Attributes</span></span>

|<span data-ttu-id="e8515-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e8515-109">**Attribute**</span></span>|<span data-ttu-id="e8515-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8515-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8515-111">**Passagem**</span><span class="sxs-lookup"><span data-stu-id="e8515-111">**Traversal**</span></span> <br/> |<span data-ttu-id="e8515-112">Define se a pesquisa localiza itens nas pastas ou nos dumpster das pastas.</span><span class="sxs-lookup"><span data-stu-id="e8515-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="e8515-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e8515-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="e8515-114">Valores de atributos de passagem</span><span class="sxs-lookup"><span data-stu-id="e8515-114">Traversal attribute values</span></span>

|<span data-ttu-id="e8515-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e8515-115">**Value**</span></span>|<span data-ttu-id="e8515-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8515-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8515-117">Superficial</span><span class="sxs-lookup"><span data-stu-id="e8515-117">Shallow</span></span>  <br/> |<span data-ttu-id="e8515-118">Retorna somente as identidades dos itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="e8515-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="e8515-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="e8515-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="e8515-120">Retorna somente as identidades dos itens que estão no dumpster de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e8515-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="e8515-121">Observe que uma passagem com exclusão reversível combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondam aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e8515-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="e8515-122">Ao</span><span class="sxs-lookup"><span data-stu-id="e8515-122">Associated</span></span>  <br/> |<span data-ttu-id="e8515-123">Retorna somente as identidades dos itens associados na pasta.</span><span class="sxs-lookup"><span data-stu-id="e8515-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e8515-124">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e8515-124">Child elements</span></span>

|<span data-ttu-id="e8515-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e8515-125">**Element**</span></span>|<span data-ttu-id="e8515-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e8515-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8515-127">Shape</span><span class="sxs-lookup"><span data-stu-id="e8515-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="e8515-128">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta de [operação do FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e8515-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="e8515-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="e8515-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="e8515-130">Descreve como as informações de item paginado são retornadas para uma solicitação **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="e8515-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="e8515-131">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="e8515-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="e8515-133">Descreve onde o modo de exibição paginado começa e o número máximo de itens retornados em uma solicitação **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="e8515-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="e8515-134">O deslocamento de modo de exibição paginado desde o início do conjunto de itens encontrados é descrito por uma fração.</span><span class="sxs-lookup"><span data-stu-id="e8515-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="e8515-135">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-136">Modo de exibição do Calendário</span><span class="sxs-lookup"><span data-stu-id="e8515-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="e8515-137">Fornece limites de intervalo de tempo para definir uma pesquisa para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="e8515-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="e8515-138">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="e8515-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="e8515-140">Define uma pesquisa para itens de contato com base em nomes de exibição em ordem alfabética.</span><span class="sxs-lookup"><span data-stu-id="e8515-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="e8515-141">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="e8515-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="e8515-143">Especifica agrupamentos arbitrários para consultas do **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="e8515-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="e8515-144">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="e8515-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="e8515-146">Fornece agrupamentos padrão para consultas do **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="e8515-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="e8515-147">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="e8515-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="e8515-149">Define a restrição ou a consulta usada para filtrar itens ou pastas no **FindItem** /  **FindFolder** e nas operações da pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e8515-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="e8515-150">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="e8515-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="e8515-152">Define como os itens são classificados em uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="e8515-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="e8515-153">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e8515-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e8515-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="e8515-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="e8515-155">Identifica as pastas nas quais as operações do FindItem e do FindFolder serão pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="e8515-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="e8515-156">QueryString (QueryStringtype)</span><span class="sxs-lookup"><span data-stu-id="e8515-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="e8515-157">Contém uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS).</span><span class="sxs-lookup"><span data-stu-id="e8515-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8515-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e8515-158">Parent elements</span></span>

<span data-ttu-id="e8515-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8515-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8515-160">Comentários</span><span class="sxs-lookup"><span data-stu-id="e8515-160">Remarks</span></span>

<span data-ttu-id="e8515-161">Somente um dos elementos [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) pode ser incluído em uma solicitação de **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="e8515-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="e8515-162">Somente um dos elementos [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) pode ser incluído em uma solicitação **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="e8515-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="e8515-163">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8515-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8515-164">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e8515-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8515-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8515-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8515-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e8515-166">Schema Name</span></span>  <br/> |<span data-ttu-id="e8515-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e8515-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8515-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e8515-168">Validation File</span></span>  <br/> |<span data-ttu-id="e8515-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8515-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8515-170">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e8515-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8515-171">False</span><span class="sxs-lookup"><span data-stu-id="e8515-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8515-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="e8515-172">See also</span></span>

- [<span data-ttu-id="e8515-173">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="e8515-173">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="e8515-174">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="e8515-174">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

