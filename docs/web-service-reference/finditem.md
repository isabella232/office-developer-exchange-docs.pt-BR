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
description: O elemento de FindItem define uma solicitação para localizar itens em uma caixa de correio.
ms.openlocfilehash: 6664cd91007f1d39db7e8d446e0135f47d5ab932
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353921"
---
# <a name="finditem"></a><span data-ttu-id="6fcda-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="6fcda-103">FindItem</span></span>

<span data-ttu-id="6fcda-104">O elemento de **FindItem** define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6fcda-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
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


<span data-ttu-id="6fcda-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="6fcda-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6fcda-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6fcda-106">Attributes and elements</span></span>

<span data-ttu-id="6fcda-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6fcda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fcda-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6fcda-108">Attributes</span></span>

|<span data-ttu-id="6fcda-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="6fcda-109">**Attribute**</span></span>|<span data-ttu-id="6fcda-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fcda-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fcda-111">**Passagem**</span><span class="sxs-lookup"><span data-stu-id="6fcda-111">**Traversal**</span></span> <br/> |<span data-ttu-id="6fcda-112">Define se a pesquisa localizará itens em pastas ou dumpsters das pastas.</span><span class="sxs-lookup"><span data-stu-id="6fcda-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="6fcda-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6fcda-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="6fcda-114">Valores de atributos de passagem</span><span class="sxs-lookup"><span data-stu-id="6fcda-114">Traversal attribute values</span></span>

|<span data-ttu-id="6fcda-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6fcda-115">**Value**</span></span>|<span data-ttu-id="6fcda-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fcda-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fcda-117">Raso</span><span class="sxs-lookup"><span data-stu-id="6fcda-117">Shallow</span></span>  <br/> |<span data-ttu-id="6fcda-118">Retorna apenas as identidades dos itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="6fcda-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="6fcda-119">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="6fcda-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="6fcda-120">Retorna apenas as identidades dos itens que estão em uma pasta dumpster.</span><span class="sxs-lookup"><span data-stu-id="6fcda-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="6fcda-121">Observe que uma passagem excluída combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondem aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6fcda-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="6fcda-122">Associados</span><span class="sxs-lookup"><span data-stu-id="6fcda-122">Associated</span></span>  <br/> |<span data-ttu-id="6fcda-123">Retorna apenas as identidades dos itens associados na pasta.</span><span class="sxs-lookup"><span data-stu-id="6fcda-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6fcda-124">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6fcda-124">Child elements</span></span>

|<span data-ttu-id="6fcda-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6fcda-125">**Element**</span></span>|<span data-ttu-id="6fcda-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fcda-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fcda-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="6fcda-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="6fcda-128">Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6fcda-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="6fcda-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="6fcda-130">Descreve como paginados informações de item é retornada para uma solicitação de **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6fcda-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="6fcda-131">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="6fcda-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="6fcda-133">Descreve o modo de exibição paginado inicia onde e o número máximo de itens retornados em uma solicitação de **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6fcda-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="6fcda-134">O deslocamento do modo de exibição paginados desde o início do conjunto de itens encontrados descrito por uma fração.</span><span class="sxs-lookup"><span data-stu-id="6fcda-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="6fcda-135">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="6fcda-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="6fcda-137">Fornece tempo span limites para definir uma pesquisa de itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="6fcda-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="6fcda-138">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="6fcda-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="6fcda-140">Define uma pesquisa de itens de contato, com base em nomes para exibição em ordem alfabética.</span><span class="sxs-lookup"><span data-stu-id="6fcda-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="6fcda-141">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="6fcda-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="6fcda-143">Especifica agrupamentos arbitrários para consultas **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6fcda-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="6fcda-144">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="6fcda-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="6fcda-146">Fornece agrupamentos padrão para consultas **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6fcda-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="6fcda-147">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="6fcda-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="6fcda-149">Define a restrição ou a consulta que é usada para filtrar itens ou pastas no **FindItem**/ operações de pasta**FindFolder** e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6fcda-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="6fcda-150">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="6fcda-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="6fcda-152">Define como os itens são classificados em uma solicitação de FindItem.</span><span class="sxs-lookup"><span data-stu-id="6fcda-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="6fcda-153">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6fcda-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="6fcda-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="6fcda-155">Identifica as pastas para procurar as operações FindItem e FindFolder.</span><span class="sxs-lookup"><span data-stu-id="6fcda-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="6fcda-156">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="6fcda-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="6fcda-157">Contém uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).</span><span class="sxs-lookup"><span data-stu-id="6fcda-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6fcda-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6fcda-158">Parent elements</span></span>

<span data-ttu-id="6fcda-159">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6fcda-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6fcda-160">Comentários</span><span class="sxs-lookup"><span data-stu-id="6fcda-160">Remarks</span></span>

<span data-ttu-id="6fcda-161">Somente um do [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) elementos pode ser incluído em uma solicitação de **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6fcda-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="6fcda-162">Somente um dos elementos [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) pode ser incluído em uma solicitação de **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="6fcda-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="6fcda-163">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6fcda-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fcda-164">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6fcda-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fcda-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fcda-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6fcda-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6fcda-166">Schema Name</span></span>  <br/> |<span data-ttu-id="6fcda-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6fcda-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6fcda-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6fcda-168">Validation File</span></span>  <br/> |<span data-ttu-id="6fcda-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6fcda-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6fcda-170">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6fcda-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fcda-171">False</span><span class="sxs-lookup"><span data-stu-id="6fcda-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fcda-172">Ver também</span><span class="sxs-lookup"><span data-stu-id="6fcda-172">See also</span></span>

- [<span data-ttu-id="6fcda-173">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="6fcda-173">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="6fcda-174">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="6fcda-174">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

