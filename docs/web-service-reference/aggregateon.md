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
# <a name="aggregateon"></a>Agregar

O elemento **Aggregate** representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupados. 
  
- [FindItem](finditem.md)  
- [GroupBy](groupby.md)
- [Agregar](aggregateon.md)
  
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
 
**AggregateOnType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Aggregate** <br/> | Indica o valor máximo ou mínimo da propriedade identificada pelo elemento [FieldURI](fielduri.md) que é usada para ordenar os grupos de itens.<br/><br/>Veja a seguir os valores possíveis:  <br/><br/>-Mínimo  <br/>-Máximo  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades com frequência referenciadas por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades de MAPI estendidas a serem obtidas, definidas ou criadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GroupBy](groupby.md) <br/> |Especifica agrupamentos arbitrários para consultas do FindItem.  <br/> A seguir está a expressão XPath para este elemento:`/FindItem/GroupBy` <br/> |
   
## <a name="remarks"></a>Comentários

A [operação FindItem](finditem-operation.md) pode retornar resultados agrupados. Nos resultados agrupados, todos os itens que têm o mesmo valor para uma determinada propriedade de agrupamento são coletados e apresentados como filhos desse grupo. Por exemplo, se você agrupar por remetente, todos os emails serão organizados em grupos separados, com base no remetente A, no remetente B e assim por diante. Esses grupos são filhos do grupo de remetentes. 
  
Cada um dos grupos no grupo de remetentes contém uma coleção de itens, como os emails reais provenientes de cada remetente. Você pode usar o elemento [SortOrder](sortorder.md) para classificar os itens dentro de um grupo. Para classificar os grupos com base nos valores de propriedade de um item, no entanto, você deve usar agregação. 
  
Com a agregação, a ordem dos grupos baseia-se em uma propriedade específica dos itens dentro do grupo. Ao usar a agregação para classificar itens dentro de um grupo, você deve identificar uma propriedade representativa pela qual classificar os grupos. Você pode usar o elemento **aggregateize** para especificar a propriedade Representation. 
  
Quando uma propriedade representativa é identificada, o atributo **Aggregate** é usado para indicar se os grupos são classificados de acordo com o valor máximo ou mínimo da propriedade identificada. Se o atributo **Aggregate** for definido como máximo, os grupos serão classificados começando com o maior valor para a propriedade **aggregaten** . Se o atributo **Aggregate** for definido como mínimo, os grupos serão classificados começando com o menor valor para a propriedade **aggregaten** . 
  
Por exemplo, se você deseja emitir uma consulta agrupada do FindItem, agrupando por remetente, mas deseja ordenar os grupos para que o grupo com a mensagem de email mais recente fique na parte superior, você pode agrupar por remetente e agregação na data/hora recebida com um atributo de **agregação** de máximo. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação e uma resposta de FindItem agrupadas. O exemplo mostra uma solicitação para retornar itens agrupados pela propriedade **ConversationTopic** . Dois grupos, A e B, são retornados em ordem decrescente com base no valor máximo da propriedade [DateTimeReceived](datetimereceived.md) . 
  
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

Para classificar os itens em um grupo, use o elemento [SortOrder](sortorder.md) . 
  
> [!NOTE]
> Os identificadores de item e as chaves de alteração foram reduzidos para preservar a legibilidade. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindItem](finditem-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

