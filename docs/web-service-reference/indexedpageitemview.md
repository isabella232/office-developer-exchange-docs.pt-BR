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
description: O elemento IndexedPageItemView descreve como as informações de conversa paginadas ou de item são retornadas para uma operação FindItem ou uma solicitação de operação FindConversation.
ms.openlocfilehash: 0a66f17855fd425082e3651886d3eeec4f217ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456910"
---
# <a name="indexedpageitemview"></a><span data-ttu-id="53505-103">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="53505-103">IndexedPageItemView</span></span>

<span data-ttu-id="53505-104">O elemento **IndexedPageItemView** descreve como as informações de conversa paginadas ou de item são retornadas para uma [operação FindItem](finditem-operation.md) ou uma solicitação de [operação FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="53505-104">The **IndexedPageItemView** element describes how paged conversation or item information is returned for a [FindItem operation](finditem-operation.md) or [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 <span data-ttu-id="53505-105">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="53505-105">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53505-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="53505-106">Attributes and elements</span></span>

<span data-ttu-id="53505-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="53505-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53505-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="53505-108">Attributes</span></span>

|<span data-ttu-id="53505-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="53505-109">**Attribute**</span></span>|<span data-ttu-id="53505-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53505-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53505-111">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="53505-111">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="53505-112">Descreve o número máximo de itens ou conversas a ser retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="53505-112">Describes the maximum number of items or conversations to return in the response.</span></span> <span data-ttu-id="53505-113">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="53505-113">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="53505-114">**Offset**</span><span class="sxs-lookup"><span data-stu-id="53505-114">**Offset**</span></span> <br/> |<span data-ttu-id="53505-115">Descreve o deslocamento do **BasePoint**.</span><span class="sxs-lookup"><span data-stu-id="53505-115">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="53505-116">Se **BasePoint** for igual a início, o deslocamento será positivo.</span><span class="sxs-lookup"><span data-stu-id="53505-116">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="53505-117">Se **BasePoint** for igual a end, o deslocamento será tratado como se fosse negativo.</span><span class="sxs-lookup"><span data-stu-id="53505-117">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span> <span data-ttu-id="53505-118">Isso identifica qual item ou conversa será o primeiro a ser entregue na resposta.</span><span class="sxs-lookup"><span data-stu-id="53505-118">This identifies which item or conversation will be the first to be delivered in the response.</span></span> <span data-ttu-id="53505-119">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="53505-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="53505-120">**BasePoint**</span><span class="sxs-lookup"><span data-stu-id="53505-120">**BasePoint**</span></span> <br/> |<span data-ttu-id="53505-121">Descreve se a página de itens ou conversas começará no início ou no final do conjunto de itens ou conversas encontrados usando os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="53505-121">Describes whether the page of items or conversations will start from the beginning or the end of the set of items or conversations that are found by using the search criteria.</span></span> <span data-ttu-id="53505-122">Procurar a partir do fim sempre pesquisa retroativamente.</span><span class="sxs-lookup"><span data-stu-id="53505-122">Seeking from the end always searches backward.</span></span> <span data-ttu-id="53505-123">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="53505-123">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="53505-124">Atributo BasePoint</span><span class="sxs-lookup"><span data-stu-id="53505-124">BasePoint Attribute</span></span>

|<span data-ttu-id="53505-125">**Valor**</span><span class="sxs-lookup"><span data-stu-id="53505-125">**Value**</span></span>|<span data-ttu-id="53505-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53505-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53505-127">Extremidade</span><span class="sxs-lookup"><span data-stu-id="53505-127">Beginning</span></span>  <br/> |<span data-ttu-id="53505-128">O modo de exibição paginado começa no início da conversa encontrada ou do conjunto de itens.</span><span class="sxs-lookup"><span data-stu-id="53505-128">The paged view starts at the beginning of the found conversation or item set.</span></span>  <br/> |
|<span data-ttu-id="53505-129">Final</span><span class="sxs-lookup"><span data-stu-id="53505-129">End</span></span>  <br/> |<span data-ttu-id="53505-130">O modo de exibição paginado começa no final da conversa encontrada ou do conjunto de itens.</span><span class="sxs-lookup"><span data-stu-id="53505-130">The paged view starts at the end of the found conversation or item set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="53505-131">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="53505-131">Child elements</span></span>

<span data-ttu-id="53505-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53505-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53505-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="53505-133">Parent elements</span></span>

|<span data-ttu-id="53505-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="53505-134">**Element**</span></span>|<span data-ttu-id="53505-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53505-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53505-136">FindItem</span><span class="sxs-lookup"><span data-stu-id="53505-136">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="53505-137">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="53505-137">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="53505-138">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="53505-138">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="53505-139">FindConversation</span><span class="sxs-lookup"><span data-stu-id="53505-139">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="53505-140">Define uma solicitação para encontrar conversas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="53505-140">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="53505-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="53505-141">Remarks</span></span>

<span data-ttu-id="53505-142">Procurar a partir do final envolve mudar para a origem identificada pelo deslocamento.</span><span class="sxs-lookup"><span data-stu-id="53505-142">Seeking from the end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="53505-143">Além disso, o ponteiro é movido de volta pelo número de registros solicitados.</span><span class="sxs-lookup"><span data-stu-id="53505-143">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="53505-144">Por exemplo, se houver 100 registros e o deslocamento for 25 a partir do final, a pesquisa iniciará de 75.</span><span class="sxs-lookup"><span data-stu-id="53505-144">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="53505-145">Se 10 registros forem retornados, o ponteiro será movido para trás de 10 registros adicionais para 65 e retornará os registros 65 a 75.</span><span class="sxs-lookup"><span data-stu-id="53505-145">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="53505-146">O próximo índice é 64.</span><span class="sxs-lookup"><span data-stu-id="53505-146">The next index is 64.</span></span> <span data-ttu-id="53505-147">O próximo deslocamento do final de uma página é 100 menos 64, que é igual a 36.</span><span class="sxs-lookup"><span data-stu-id="53505-147">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="53505-148">36 é o valor do próximo deslocamento do fim para obter a próxima página indexada.</span><span class="sxs-lookup"><span data-stu-id="53505-148">36 is the value for the next offset from the end to get the next indexed page.</span></span>
  
<span data-ttu-id="53505-149">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="53505-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="53505-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53505-150">Example</span></span>

<span data-ttu-id="53505-151">O exemplo a seguir mostra uma solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="53505-151">The following example shows a [FindItem operation](finditem-operation.md) request.</span></span> <span data-ttu-id="53505-152">Cada item é retornado com sua ID e assunto.</span><span class="sxs-lookup"><span data-stu-id="53505-152">Each item is returned with its ID and subject.</span></span> <span data-ttu-id="53505-153">Um máximo de seis itens é retornado na resposta, conforme especificado pelo atributo **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="53505-153">A maximum of six items are returned in the response, as specified by the **MaxEntriesReturned** attribute.</span></span> <span data-ttu-id="53505-154">Os itens são listados em ordem crescente por prioridade.</span><span class="sxs-lookup"><span data-stu-id="53505-154">The items are listed in ascending order grouped by importance.</span></span> <span data-ttu-id="53505-155">Os itens em um grupo são agregados por assunto.</span><span class="sxs-lookup"><span data-stu-id="53505-155">Items in a group are aggregated by subject.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="53505-156">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="53505-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53505-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="53505-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="53505-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="53505-158">Schema Name</span></span>  <br/> |<span data-ttu-id="53505-159">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="53505-159">Messages schema</span></span>  <br/> |
|<span data-ttu-id="53505-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="53505-160">Validation File</span></span>  <br/> |<span data-ttu-id="53505-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="53505-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="53505-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="53505-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="53505-163">False</span><span class="sxs-lookup"><span data-stu-id="53505-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53505-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="53505-164">See also</span></span>



[<span data-ttu-id="53505-165">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="53505-165">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="53505-166">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="53505-166">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="53505-167">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="53505-167">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

