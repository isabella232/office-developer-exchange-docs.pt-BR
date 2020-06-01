---
title: Agregar
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AggregateOn
api_type:
- schema
ms.assetid: 9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb
description: O elemento Aggregate representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupados.
ms.openlocfilehash: 04359c187ef11538d64f8f0d3ea2fe84bc3d048b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463563"
---
# <a name="aggregateon"></a><span data-ttu-id="993e6-103">Agregar</span><span class="sxs-lookup"><span data-stu-id="993e6-103">AggregateOn</span></span>

<span data-ttu-id="993e6-104">O elemento **Aggregate** representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupados.</span><span class="sxs-lookup"><span data-stu-id="993e6-104">The **AggregateOn** element represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span> 
  
- [<span data-ttu-id="993e6-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="993e6-105">FindItem</span></span>](finditem.md)  
- [<span data-ttu-id="993e6-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="993e6-106">GroupBy</span></span>](groupby.md)
- [<span data-ttu-id="993e6-107">Agregar</span><span class="sxs-lookup"><span data-stu-id="993e6-107">AggregateOn</span></span>](aggregateon.md)
  
```xml
<AggregateOn>
   <FieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <IndexedFieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <ExtendedFieldURI/>
</AggregateOn>
```
 
<span data-ttu-id="993e6-108">**AggregateOnType**</span><span class="sxs-lookup"><span data-stu-id="993e6-108">**AggregateOnType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="993e6-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="993e6-109">Attributes and elements</span></span>

<span data-ttu-id="993e6-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="993e6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="993e6-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="993e6-111">Attributes</span></span>

|<span data-ttu-id="993e6-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="993e6-112">**Attribute**</span></span>|<span data-ttu-id="993e6-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="993e6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="993e6-114">**Aggregate**</span><span class="sxs-lookup"><span data-stu-id="993e6-114">**Aggregate**</span></span> <br/> | <span data-ttu-id="993e6-115">Indica o valor máximo ou mínimo da propriedade identificada pelo elemento [FieldURI](fielduri.md) que é usada para ordenar os grupos de itens.</span><span class="sxs-lookup"><span data-stu-id="993e6-115">Indicates the maximum or minimum value of the property identified by the [FieldURI](fielduri.md) element that is used for ordering the groups of items.</span></span><br/><br/><span data-ttu-id="993e6-116">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="993e6-116">The following are the possible values:</span></span>  <br/><br/><span data-ttu-id="993e6-117">-Mínimo</span><span class="sxs-lookup"><span data-stu-id="993e6-117">- Minimum</span></span>  <br/><span data-ttu-id="993e6-118">-Máximo</span><span class="sxs-lookup"><span data-stu-id="993e6-118">- Maximum</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="993e6-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="993e6-119">Child elements</span></span>

|<span data-ttu-id="993e6-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="993e6-120">**Element**</span></span>|<span data-ttu-id="993e6-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="993e6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="993e6-122">FieldURI</span><span class="sxs-lookup"><span data-stu-id="993e6-122">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="993e6-123">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="993e6-123">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="993e6-124">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="993e6-124">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="993e6-125">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="993e6-125">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="993e6-126">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="993e6-126">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="993e6-127">Identifica as propriedades de MAPI estendidas a serem obtidas, definidas ou criadas.</span><span class="sxs-lookup"><span data-stu-id="993e6-127">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="993e6-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="993e6-128">Parent elements</span></span>

|<span data-ttu-id="993e6-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="993e6-129">**Element**</span></span>|<span data-ttu-id="993e6-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="993e6-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="993e6-131">GroupBy</span><span class="sxs-lookup"><span data-stu-id="993e6-131">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="993e6-132">Especifica agrupamentos arbitrários para consultas do FindItem.</span><span class="sxs-lookup"><span data-stu-id="993e6-132">Specifies arbitrary groupings for FindItem queries.</span></span>  <br/> <span data-ttu-id="993e6-133">A seguir está a expressão XPath para este elemento:`/FindItem/GroupBy`</span><span class="sxs-lookup"><span data-stu-id="993e6-133">The following is the XPath expression to this element:  `/FindItem/GroupBy`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="993e6-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="993e6-134">Remarks</span></span>

<span data-ttu-id="993e6-135">A [operação FindItem](finditem-operation.md) pode retornar resultados agrupados.</span><span class="sxs-lookup"><span data-stu-id="993e6-135">The [FindItem operation](finditem-operation.md) can return grouped results.</span></span> <span data-ttu-id="993e6-136">Nos resultados agrupados, todos os itens que têm o mesmo valor para uma determinada propriedade de agrupamento são coletados e apresentados como filhos desse grupo.</span><span class="sxs-lookup"><span data-stu-id="993e6-136">Within grouped results, all items that have the same value for a given grouping property are gathered together and presented as children of that group.</span></span> <span data-ttu-id="993e6-137">Por exemplo, se você agrupar por remetente, todos os emails serão organizados em grupos separados, com base no remetente A, no remetente B e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="993e6-137">For example, if you group by sender, all e-mails are organized into separate groups based on whether they are from sender A, sender B, and so on.</span></span> <span data-ttu-id="993e6-138">Esses grupos são filhos do grupo de remetentes.</span><span class="sxs-lookup"><span data-stu-id="993e6-138">These groups are children of the sender group.</span></span> 
  
<span data-ttu-id="993e6-139">Cada um dos grupos no grupo de remetentes contém uma coleção de itens, como os emails reais provenientes de cada remetente.</span><span class="sxs-lookup"><span data-stu-id="993e6-139">Each of the groups within the sender group contains a collection of items, such as the actual e-mails that came from each sender.</span></span> <span data-ttu-id="993e6-140">Você pode usar o elemento [SortOrder](sortorder.md) para classificar os itens dentro de um grupo.</span><span class="sxs-lookup"><span data-stu-id="993e6-140">You can use the [SortOrder](sortorder.md) element to sort the items within a group.</span></span> <span data-ttu-id="993e6-141">Para classificar os grupos com base nos valores de propriedade de um item, no entanto, você deve usar agregação.</span><span class="sxs-lookup"><span data-stu-id="993e6-141">To sort the groups based on an item's property values, however, you must use aggregation.</span></span> 
  
<span data-ttu-id="993e6-142">Com a agregação, a ordem dos grupos baseia-se em uma propriedade específica dos itens dentro do grupo.</span><span class="sxs-lookup"><span data-stu-id="993e6-142">With aggregation, the order of groups is based on a specific property of the items within the group.</span></span> <span data-ttu-id="993e6-143">Ao usar a agregação para classificar itens dentro de um grupo, você deve identificar uma propriedade representativa pela qual classificar os grupos.</span><span class="sxs-lookup"><span data-stu-id="993e6-143">When you use aggregation to sort items within a group, you must identify a representative property by which to sort the groups.</span></span> <span data-ttu-id="993e6-144">Você pode usar o elemento **aggregateize** para especificar a propriedade Representation.</span><span class="sxs-lookup"><span data-stu-id="993e6-144">You can use the **AggregateOn** element to specify the representative property.</span></span> 
  
<span data-ttu-id="993e6-145">Quando uma propriedade representativa é identificada, o atributo **Aggregate** é usado para indicar se os grupos são classificados de acordo com o valor máximo ou mínimo da propriedade identificada.</span><span class="sxs-lookup"><span data-stu-id="993e6-145">When a representative property is identified, the **Aggregate** attribute is used to indicate whether the groups are sorted according to the maximum or the minimum value of the identified property.</span></span> <span data-ttu-id="993e6-146">Se o atributo **Aggregate** for definido como máximo, os grupos serão classificados começando com o maior valor para a propriedade **aggregaten** .</span><span class="sxs-lookup"><span data-stu-id="993e6-146">If the **Aggregate** attribute is set to Maximum, the groups are sorted beginning with the largest value for the **AggregateOn** property.</span></span> <span data-ttu-id="993e6-147">Se o atributo **Aggregate** for definido como mínimo, os grupos serão classificados começando com o menor valor para a propriedade **aggregaten** .</span><span class="sxs-lookup"><span data-stu-id="993e6-147">If the **Aggregate** attribute is set to Minimum, the groups are sorted beginning with the smallest value for the **AggregateOn** property.</span></span> 
  
<span data-ttu-id="993e6-148">Por exemplo, se você deseja emitir uma consulta agrupada do FindItem, agrupando por remetente, mas deseja ordenar os grupos para que o grupo com a mensagem de email mais recente fique na parte superior, você pode agrupar por remetente e agregação na data/hora recebida com um atributo de **agregação** de máximo.</span><span class="sxs-lookup"><span data-stu-id="993e6-148">For example, if you want to issue a FindItem grouped query, grouping by sender, but you want to order the groups so that the group with the most recent e-mail message is on top, you can group by sender and aggregate on date/time received with an **Aggregate** attribute of Maximum.</span></span> 
  
<span data-ttu-id="993e6-149">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="993e6-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="993e6-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="993e6-150">Example</span></span>

<span data-ttu-id="993e6-151">O exemplo a seguir mostra uma solicitação e uma resposta de FindItem agrupadas.</span><span class="sxs-lookup"><span data-stu-id="993e6-151">The following example shows a grouped FindItem request and response.</span></span> <span data-ttu-id="993e6-152">O exemplo mostra uma solicitação para retornar itens agrupados pela propriedade **ConversationTopic** .</span><span class="sxs-lookup"><span data-stu-id="993e6-152">The example shows a request to return items grouped by the **ConversationTopic** property.</span></span> <span data-ttu-id="993e6-153">Dois grupos, A e B, são retornados em ordem decrescente com base no valor máximo da propriedade [DateTimeReceived](datetimereceived.md) .</span><span class="sxs-lookup"><span data-stu-id="993e6-153">Two groups, A and B, are returned in descending order based on the maximum value of the [DateTimeReceived](datetimereceived.md) property.</span></span> 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="message:ConversationTopic"/>
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AdditionalProperties>    
      </ItemShape>
      <IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="20" Offset="0"/>
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="message:ConversationTopic"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
<!-- EXAMPLE RESPONSE -->
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>B</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAH=" ChangeKey="CQAAABY" />
                    <t:DateTimeReceived>2006-09-14T23:59:18Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnAHR=" ChangeKey="CQAAAw" />
                    <t:DateTimeReceived>2006-09-15T00:00:24Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnA==" ChangeKey="CQAAJXT" />
                    <t:DateTimeReceived>2006-09-15T00:22:45Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>A</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAAA==" ChangeKey="CQCJNe" />
                    <t:DateTimeReceived>2006-09-14T23:56:12Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQWgAA==" ChangeKey="CQAACJV6" />
                    <t:DateTimeReceived>2006-09-14T23:57:33Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAAA==" ChangeKey="CQA6CJXw" />
                    <t:DateTimeReceived>2006-09-15T00:23:31Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="993e6-154">Para classificar os itens em um grupo, use o elemento [SortOrder](sortorder.md) .</span><span class="sxs-lookup"><span data-stu-id="993e6-154">To sort the items in a group, use the [SortOrder](sortorder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="993e6-155">Os identificadores de item e as chaves de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="993e6-155">The item identifiers and change keys have been shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="993e6-156">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="993e6-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="993e6-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="993e6-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="993e6-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="993e6-158">Schema Name</span></span>  <br/> |<span data-ttu-id="993e6-159">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="993e6-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="993e6-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="993e6-160">Validation File</span></span>  <br/> |<span data-ttu-id="993e6-161">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="993e6-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="993e6-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="993e6-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="993e6-163">False</span><span class="sxs-lookup"><span data-stu-id="993e6-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="993e6-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="993e6-164">See also</span></span>

- [<span data-ttu-id="993e6-165">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="993e6-165">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="993e6-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="993e6-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="993e6-167">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="993e6-167">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

