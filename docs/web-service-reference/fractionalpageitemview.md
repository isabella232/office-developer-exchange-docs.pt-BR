---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: O elemento FractionalPageItemView descreve onde o modo de exibição paginado começa e o número máximo de itens retornados em uma solicitação FindItem.
ms.openlocfilehash: cbf45838558873dc5846823c2d1b26cf2c8af514
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461307"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="c51ab-103">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="c51ab-103">FractionalPageItemView</span></span>

<span data-ttu-id="c51ab-104">O elemento **FractionalPageItemView** descreve onde o modo de exibição paginado começa e o número máximo de itens retornados em uma solicitação [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="c51ab-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="c51ab-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="c51ab-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="c51ab-106">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="c51ab-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="c51ab-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="c51ab-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c51ab-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c51ab-108">Attributes and elements</span></span>

<span data-ttu-id="c51ab-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c51ab-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c51ab-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c51ab-110">Attributes</span></span>

|<span data-ttu-id="c51ab-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="c51ab-111">**Attribute**</span></span>|<span data-ttu-id="c51ab-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c51ab-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c51ab-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="c51ab-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="c51ab-114">Identifica o número máximo de resultados a serem retornados na resposta [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="c51ab-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="c51ab-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="c51ab-115">This attribute is optional.</span></span> <span data-ttu-id="c51ab-116">Se esse atributo não for especificado, a chamada retornará todos os itens disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c51ab-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="c51ab-117">**Numera**</span><span class="sxs-lookup"><span data-stu-id="c51ab-117">**Numerator**</span></span> <br/> |<span data-ttu-id="c51ab-118">Representa o numerador do deslocamento fracionado do início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="c51ab-119">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="c51ab-119">This attribute is required.</span></span> <span data-ttu-id="c51ab-120">O numerador deve ser igual ou menor que o denominador.</span><span class="sxs-lookup"><span data-stu-id="c51ab-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="c51ab-121">Este atributo deve representar um valor inteiro igual ou maior que zero.</span><span class="sxs-lookup"><span data-stu-id="c51ab-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="c51ab-122">Para obter mais informações, consulte comentários mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="c51ab-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="c51ab-123">**Denominado**</span><span class="sxs-lookup"><span data-stu-id="c51ab-123">**Denominator**</span></span> <br/> |<span data-ttu-id="c51ab-124">Representa o denominador do deslocamento fracionado desde o início do número total de itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="c51ab-125">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="c51ab-125">This attribute is required.</span></span> <span data-ttu-id="c51ab-126">Este atributo deve representar um valor integral maior que um.</span><span class="sxs-lookup"><span data-stu-id="c51ab-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="c51ab-127">Para obter mais informações, consulte comentários mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="c51ab-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c51ab-128">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c51ab-128">Child elements</span></span>

<span data-ttu-id="c51ab-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c51ab-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c51ab-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c51ab-130">Parent elements</span></span>

|<span data-ttu-id="c51ab-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c51ab-131">**Element**</span></span>|<span data-ttu-id="c51ab-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c51ab-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c51ab-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="c51ab-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="c51ab-134">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c51ab-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="c51ab-135">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="c51ab-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c51ab-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="c51ab-136">Remarks</span></span>

<span data-ttu-id="c51ab-137">O deslocamento de modo de exibição paginado desde o início do conjunto de itens encontrados é descrito por uma fração.</span><span class="sxs-lookup"><span data-stu-id="c51ab-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="c51ab-138">A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciada.</span><span class="sxs-lookup"><span data-stu-id="c51ab-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="c51ab-139">Por exemplo, se o **numerador** for igual a quatro e o **denominador** for igual a cinco, a página de informações retornadas será iniciada em uma entrada localizada em quatro cinco quinto da forma no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="c51ab-140">Se a fração for avaliada como zero, isso indica o início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="c51ab-141">Se a fração for avaliada como um, isso indica o final do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c51ab-142">A fração representa o ponto de início da página, não quantos resultados serão retornados no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="c51ab-143">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c51ab-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="c51ab-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c51ab-144">Example</span></span>

<span data-ttu-id="c51ab-145">O exemplo a seguir mostra uma solicitação [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="c51ab-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="c51ab-146">A solicitação retorna itens dos resultados da pesquisa que começam após o segundo terço de todos os itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
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
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
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

<span data-ttu-id="c51ab-147">Por exemplo, se o conjunto de resultados contiver nove itens, o modo de exibição paginado retornará até 12 itens, começando no item encontrado dois terços da forma no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="c51ab-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="c51ab-148">Nesse caso, a página começa no sétimo item.</span><span class="sxs-lookup"><span data-stu-id="c51ab-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="c51ab-149">A página conterá os sétimo, oitavo e nono itens.</span><span class="sxs-lookup"><span data-stu-id="c51ab-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="c51ab-150">Se o numerador for definido como zero, o modo de exibição de página retornará todos os itens no conjunto de resultados, desde que o número seja menor do que o atributo **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="c51ab-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="c51ab-151">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c51ab-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c51ab-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="c51ab-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c51ab-153">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c51ab-153">Schema Name</span></span>  <br/> |<span data-ttu-id="c51ab-154">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c51ab-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c51ab-155">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c51ab-155">Validation File</span></span>  <br/> |<span data-ttu-id="c51ab-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c51ab-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c51ab-157">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c51ab-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="c51ab-158">False</span><span class="sxs-lookup"><span data-stu-id="c51ab-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c51ab-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="c51ab-159">See also</span></span>



[<span data-ttu-id="c51ab-160">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="c51ab-160">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="c51ab-161">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="c51ab-161">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

