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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456910"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

O elemento **IndexedPageItemView** descreve como as informações de conversa paginadas ou de item são retornadas para uma [operação FindItem](finditem-operation.md) ou uma solicitação de [operação FindConversation](findconversation-operation.md) . 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de itens ou conversas a ser retornado na resposta. Esse atributo é opcional.  <br/> |
|**Offset** <br/> |Descreve o deslocamento do **BasePoint**. Se **BasePoint** for igual a início, o deslocamento será positivo. Se **BasePoint** for igual a end, o deslocamento será tratado como se fosse negativo. Isso identifica qual item ou conversa será o primeiro a ser entregue na resposta. Esse atributo é necessário.  <br/> |
|**BasePoint** <br/> |Descreve se a página de itens ou conversas começará no início ou no final do conjunto de itens ou conversas encontrados usando os critérios de pesquisa. Procurar a partir do fim sempre pesquisa retroativamente. Esse atributo é necessário.  <br/> |
   
#### <a name="basepoint-attribute"></a>Atributo BasePoint

|**Valor**|**Descrição**|
|:-----|:-----|
|Extremidade  <br/> |O modo de exibição paginado começa no início da conversa encontrada ou do conjunto de itens.  <br/> |
|Final  <br/> |O modo de exibição paginado começa no final da conversa encontrada ou do conjunto de itens.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Define uma solicitação para encontrar conversas em uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Comentários

Procurar a partir do final envolve mudar para a origem identificada pelo deslocamento. Além disso, o ponteiro é movido de volta pelo número de registros solicitados. Por exemplo, se houver 100 registros e o deslocamento for 25 a partir do final, a pesquisa iniciará de 75. Se 10 registros forem retornados, o ponteiro será movido para trás de 10 registros adicionais para 65 e retornará os registros 65 a 75. O próximo índice é 64. O próximo deslocamento do final de uma página é 100 menos 64, que é igual a 36. 36 é o valor do próximo deslocamento do fim para obter a próxima página indexada.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação de [operação FindItem](finditem-operation.md) . Cada item é retornado com sua ID e assunto. Um máximo de seis itens é retornado na resposta, conforme especificado pelo atributo **MaxEntriesReturned** . Os itens são listados em ordem crescente por prioridade. Os itens em um grupo são agregados por assunto. 
  
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

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)
  
[Operação FindConversation](findconversation-operation.md)


[Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

