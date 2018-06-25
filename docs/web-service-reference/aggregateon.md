---
title: AggregateOn
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
description: O elemento AggregateOn representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupada.
ms.openlocfilehash: fe14de23e6a4c90d826200cae927427acfccc3c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751073"
---
# <a name="aggregateon"></a>AggregateOn

O elemento **AggregateOn** representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupada. 
  
- [FindItem](finditem.md)  
- [GroupBy](groupby.md)
- [AggregateOn](aggregateon.md)
  
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

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Aggregate** <br/> | Indica o valor máximo ou mínimo da propriedade identificado pelo elemento [FieldURI](fielduri.md) que é usado para os grupos de itens de classificação.<br/><br/>Veja a seguir os valores possíveis:  <br/><br/>-Mínimo  <br/>-Maximum  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades estendidas de MAPI para obter, definir ou criar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GroupBy](groupby.md) <br/> |Especifica agrupamentos arbitrários para consultas FindItem.  <br/> Este é a expressão XPath para esse elemento:`/FindItem/GroupBy` <br/> |
   
## <a name="remarks"></a>Comentários

A [operação FindItem](finditem-operation.md) pode retornar resultados agrupados. Em resultados agrupados, todos os itens que têm o mesmo valor de uma propriedade de agrupamento determinado são coletados juntos e apresentados como filhos desse grupo. Por exemplo, se você agrupar por remetente, todos os emails são organizados em grupos separados com base em estarem ou do remetente A, B do remetente e assim por diante. Esses grupos são filhos do grupo do remetente. 
  
Cada um dos grupos dentro do grupo de remetente contém uma coleção de itens, como os e-mails reais fornecidos por cada remetente. Você pode usar o elemento [SortOrder](sortorder.md) para classificar os itens dentro de um grupo. Para classificar os grupos com base nos valores de propriedade de um item, no entanto, você deve usar agregação de lista segura. 
  
Com a agregação de lista segura, a ordem dos grupos baseia-se em uma propriedade específica dos itens dentro do grupo. Quando você usa agregação de lista segura para classificar itens dentro de um grupo, você deve identificar uma propriedade representativa pela qual classificar os grupos. Você pode usar o elemento **AggregateOn** para especificar a propriedade representativa. 
  
Quando uma propriedade representativa é identificada, o atributo de **agregação** é usado para indicar se os grupos são classificados de acordo com o máximo ou o valor mínimo da propriedade identificado. Se o atributo **agregado** é definido como máximo, os grupos são classificados começando com o maior valor da propriedade **AggregateOn** . Se o atributo **agregado** é definido como mínimo, os grupos são classificados começando com o menor valor da propriedade **AggregateOn** . 
  
Por exemplo, se você deseja que emite uma consulta agrupada FindItem, agrupando por remetente, mas você deseja que os grupos de ordem para que o grupo com a mensagem de email mais recente seja na parte superior, você pode agrupar por remetente e aggregate na data/hora recebida com uma **agregação** atributo de no máximo. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação FindItem agrupadas e a resposta. O exemplo mostra uma solicitação para retornar itens agrupados pela propriedade **ConversationTopic** . Dois grupos, A e B, são retornados em ordem decrescente com base no valor máximo da propriedade [DateTimeReceived](datetimereceived.md) . 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> Os identificadores de item e chaves de alteração tem sido reduzidas para preservar a legibilidade. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação FindItem](finditem-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

