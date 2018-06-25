---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: O elemento IndexedPageItemView descreve como paginada conversa ou item a informação é retornada para uma operação de FindItem ou a solicitação de operação FindConversation.
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823919"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="fed13-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="fed13-103">IndexedPageItemView</span></span>

<span data-ttu-id="fed13-104">O elemento **IndexedPageItemView** descreve como paginada conversa ou item a informação é retornada para uma solicitação de [operação de FindItem](finditem-operation.md) ou [FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fed13-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="fed13-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="fed13-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fed13-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fed13-106">Attributes and elements</span></span>

<span data-ttu-id="fed13-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fed13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fed13-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fed13-108">Attributes</span></span>

|<span data-ttu-id="fed13-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="fed13-109">**Attribute**</span></span>|<span data-ttu-id="fed13-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fed13-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fed13-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="fed13-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="fed13-112">Descreve o número máximo de itens ou conversas para retornar na resposta.</span><span class="sxs-lookup"><span data-stu-id="fed13-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="fed13-113">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="fed13-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="fed13-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="fed13-114">**Offset**</span></span> <br/> |<span data-ttu-id="fed13-115">Descreve o deslocamento, desde o **ponto de base**.</span><span class="sxs-lookup"><span data-stu-id="fed13-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="fed13-116">Se o **ponto de base** é igual ao início, o deslocamento for positivo.</span><span class="sxs-lookup"><span data-stu-id="fed13-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="fed13-117">Se o **ponto de base** for igual ao fim, o deslocamento é tratado como se fosse negativo.</span><span class="sxs-lookup"><span data-stu-id="fed13-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="fed13-118">Isso identifica qual item ou conversa será a primeira a ser entregues a resposta.</span><span class="sxs-lookup"><span data-stu-id="fed13-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="fed13-119">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="fed13-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fed13-120">**Ponto de base**</span><span class="sxs-lookup"><span data-stu-id="fed13-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="fed13-121">Descreve como se a página de itens ou conversas será iniciado a partir do início ou no final do conjunto de itens ou conversas que são encontradas usando os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fed13-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="fed13-122">Procurando a partir do término do sempre pesquisa para trás.</span><span class="sxs-lookup"><span data-stu-id="fed13-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="fed13-123">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="fed13-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="fed13-124">Atributo de ponto de base</span><span class="sxs-lookup"><span data-stu-id="fed13-124">BasePoint Attribute</span></span>

|<span data-ttu-id="fed13-125">**Valor**</span><span class="sxs-lookup"><span data-stu-id="fed13-125">**Value**</span></span>|<span data-ttu-id="fed13-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fed13-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fed13-127">Início</span><span class="sxs-lookup"><span data-stu-id="fed13-127">Beginning</span></span>  <br/> |<span data-ttu-id="fed13-128">O modo de exibição paginado começa no início do conjunto de conversa ou item encontrado.</span><span class="sxs-lookup"><span data-stu-id="fed13-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="fed13-129">End</span><span class="sxs-lookup"><span data-stu-id="fed13-129">End</span></span>  <br/> |<span data-ttu-id="fed13-130">O modo de exibição paginado inicia no final do conjunto de conversa ou item encontrado.</span><span class="sxs-lookup"><span data-stu-id="fed13-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fed13-131">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fed13-131">Child elements</span></span>

<span data-ttu-id="fed13-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fed13-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fed13-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fed13-133">Parent elements</span></span>

|<span data-ttu-id="fed13-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fed13-134">**Element**</span></span>|<span data-ttu-id="fed13-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fed13-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fed13-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="fed13-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="fed13-137">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fed13-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="fed13-138">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="fed13-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="fed13-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="fed13-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="fed13-140">Define uma solicitação para localizar conversas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fed13-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fed13-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="fed13-141">Remarks</span></span>

<span data-ttu-id="fed13-142">Buscando a partir do término do envolve mover para a origem identificada pelo deslocamento.</span><span class="sxs-lookup"><span data-stu-id="fed13-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="fed13-143">Além disso, o ponteiro é movido de volta pelo número de registros solicitados.</span><span class="sxs-lookup"><span data-stu-id="fed13-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="fed13-144">Por exemplo, se existem 100 registros e o deslocamento for 25 do fim, a pesquisa começa a partir 75.</span><span class="sxs-lookup"><span data-stu-id="fed13-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="fed13-145">Se 10 registros forem retornados, o ponteiro é movido para trás uma 10 adicionais registra como 65 e retorna registros 65 por meio de 75.</span><span class="sxs-lookup"><span data-stu-id="fed13-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="fed13-146">O próximo índice é 64.</span><span class="sxs-lookup"><span data-stu-id="fed13-146">The next index is 64.</span></span> <span data-ttu-id="fed13-147">O deslocamento próximo do final de uma página é 100 menos 64 que é igual a 36.</span><span class="sxs-lookup"><span data-stu-id="fed13-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="fed13-148">36 é o valor para o próximo deslocamento do final para obter a próxima página indexada.</span><span class="sxs-lookup"><span data-stu-id="fed13-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="fed13-149">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fed13-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="fed13-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fed13-150">Example</span></span>

<span data-ttu-id="fed13-151">O exemplo a seguir mostra uma solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fed13-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="fed13-152">Cada item é retornado com sua ID e o assunto.</span><span class="sxs-lookup"><span data-stu-id="fed13-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="fed13-153">Um máximo de seis itens são retornados na resposta, conforme especificado pelo atributo **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="fed13-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="fed13-154">Os itens são listados na ordem agrupado por importância crescente.</span><span class="sxs-lookup"><span data-stu-id="fed13-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="fed13-155">Itens em um grupo são agregados por assunto.</span><span class="sxs-lookup"><span data-stu-id="fed13-155">Items in a group are aggregated by subject.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <IndexedPageItemView MaxEntriesReturned="6" BasePoint="Beginning" Offset="0" />
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="fed13-156">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fed13-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fed13-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="fed13-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fed13-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fed13-158">Schema Name</span></span>  <br/> |<span data-ttu-id="fed13-159">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fed13-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fed13-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fed13-160">Validation File</span></span>  <br/> |<span data-ttu-id="fed13-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fed13-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fed13-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fed13-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="fed13-163">False</span><span class="sxs-lookup"><span data-stu-id="fed13-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fed13-164">Ver também</span><span class="sxs-lookup"><span data-stu-id="fed13-164">See also</span></span>



[<span data-ttu-id="fed13-165">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="fed13-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="fed13-166">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="fed13-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="fed13-167">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="fed13-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

