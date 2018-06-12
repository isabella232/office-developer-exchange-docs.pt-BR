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
description: O elemento FractionalPageItemView descreve onde o modo de exibição paginado é iniciado e o número máximo de itens retornados em uma solicitação de FindItem.
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752360"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="09769-103">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="09769-103">FractionalPageItemView</span></span>

<span data-ttu-id="09769-104">O elemento **FractionalPageItemView** descreve onde o modo de exibição paginado é iniciado e o número máximo de itens retornados em uma solicitação de [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="09769-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="09769-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="09769-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="09769-106">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="09769-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="09769-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="09769-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09769-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="09769-108">Attributes and elements</span></span>

<span data-ttu-id="09769-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="09769-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09769-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="09769-110">Attributes</span></span>

|<span data-ttu-id="09769-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="09769-111">**Attribute**</span></span>|<span data-ttu-id="09769-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="09769-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="09769-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="09769-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="09769-114">Identifica o número máximo de resultados a serem retornados na resposta [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="09769-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="09769-115">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="09769-115">This attribute is optional.</span></span> <span data-ttu-id="09769-116">Se esse atributo não for especificado, a chamada retornará todos os itens disponíveis.</span><span class="sxs-lookup"><span data-stu-id="09769-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="09769-117">**Numerador**</span><span class="sxs-lookup"><span data-stu-id="09769-117">**Numerator**</span></span> <br/> |<span data-ttu-id="09769-118">Representa o numerador do deslocamento fracional desde o início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="09769-119">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="09769-119">This attribute is required.</span></span> <span data-ttu-id="09769-120">O numerador deve ser igual ou menor que o denominador.</span><span class="sxs-lookup"><span data-stu-id="09769-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="09769-121">Este atributo deve representar um valor integral que é igual ou maior do que zero.</span><span class="sxs-lookup"><span data-stu-id="09769-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="09769-122">Para obter mais informações, consulte a seção comentários, mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="09769-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="09769-123">**Denominador**</span><span class="sxs-lookup"><span data-stu-id="09769-123">**Denominator**</span></span> <br/> |<span data-ttu-id="09769-124">Representa o denominador do deslocamento fracional desde o início do número total de itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="09769-125">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="09769-125">This attribute is required.</span></span> <span data-ttu-id="09769-126">Este atributo deve representar um valor inteiro maior que um.</span><span class="sxs-lookup"><span data-stu-id="09769-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="09769-127">Para obter mais informações, consulte a seção comentários, mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="09769-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="09769-128">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="09769-128">Child elements</span></span>

<span data-ttu-id="09769-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="09769-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09769-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="09769-130">Parent elements</span></span>

|<span data-ttu-id="09769-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="09769-131">**Element**</span></span>|<span data-ttu-id="09769-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="09769-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09769-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="09769-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="09769-134">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="09769-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="09769-135">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="09769-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="09769-136">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="09769-136">Remarks</span></span>

<span data-ttu-id="09769-137">O deslocamento do modo de exibição paginados desde o início do conjunto de itens encontrados descrito por uma fração.</span><span class="sxs-lookup"><span data-stu-id="09769-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="09769-138">A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciado.</span><span class="sxs-lookup"><span data-stu-id="09769-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="09769-139">Por exemplo, se **numerador** é igual a quatro e **denominador** igual a cinco, a página de informações retornadas começa em uma entrada localizado quatro-quintas da maneira no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="09769-140">Se fração for avaliada como zero, o que indica o início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="09769-141">Se fração for avaliada como um, que indica o fim do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="09769-142">A fração representa o ponto inicial da página, não quantos resultados no conjunto de resultados serão retornados.</span><span class="sxs-lookup"><span data-stu-id="09769-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="09769-143">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="09769-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="09769-144">Example</span><span class="sxs-lookup"><span data-stu-id="09769-144">Example</span></span>

<span data-ttu-id="09769-145">O exemplo a seguir mostra uma solicitação [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="09769-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="09769-146">A solicitação retorna os itens dos resultados da pesquisa que começam após o segundo terceiro de todos os itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
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

<span data-ttu-id="09769-147">Por exemplo, se o conjunto de resultados contiver nove itens, o modo de exibição paginado retornará até 12 itens, começando a dois terços encontrado item da maneira no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="09769-148">Nesse caso, a página começa com o sétimo item.</span><span class="sxs-lookup"><span data-stu-id="09769-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="09769-149">A página conterá o sétimo oitavo e o nono itens.</span><span class="sxs-lookup"><span data-stu-id="09769-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="09769-150">Se o numerador estiver definido como zero, o modo de exibição de página retornará todos os itens no conjunto desde que o número seja menor que o atributo **MaxEntriesReturned** de resultados.</span><span class="sxs-lookup"><span data-stu-id="09769-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="09769-151">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="09769-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09769-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="09769-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09769-153">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="09769-153">Schema Name</span></span>  <br/> |<span data-ttu-id="09769-154">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="09769-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="09769-155">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="09769-155">Validation File</span></span>  <br/> |<span data-ttu-id="09769-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="09769-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09769-157">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="09769-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="09769-158">False</span><span class="sxs-lookup"><span data-stu-id="09769-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09769-159">Ver também</span><span class="sxs-lookup"><span data-stu-id="09769-159">See also</span></span>



[<span data-ttu-id="09769-160">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="09769-160">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="09769-161">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="09769-161">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

