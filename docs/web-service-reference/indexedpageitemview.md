---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: O elemento IndexedPageItemView descreve como as informações de conversa ou item de página são retornadas para uma operação FindItem ou uma solicitação de operação FindConversation.
ms.openlocfilehash: bf46bdbd457c4f4fa47e6b575d3b797b74f58995
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541123"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

O **elemento IndexedPageItemView** descreve como as informações de conversa ou item de página são retornadas para uma operação [FindItem](finditem-operation.md) ou uma solicitação de operação [FindConversation.](findconversation-operation.md) 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de itens ou conversas a ser retornada na resposta. Esse atributo é opcional.  <br/> |
|**Offset** <br/> |Descreve o deslocamento do **BasePoint**. Se **BasePoint** for igual a Beginning, o deslocamento será positivo. Se **BasePoint** for igual a End, o deslocamento será manipulado como se fosse negativo. Isso identifica qual item ou conversa será o primeiro a ser entregue na resposta. Esse atributo é necessário.  <br/> |
|**BasePoint** <br/> |Descreve se a página de itens ou conversas começará do início ou do final do conjunto de itens ou conversas que são encontradas usando os critérios de pesquisa. Procurar desde o final sempre pesquisa para trás. Esse atributo é necessário.  <br/> |
   
#### <a name="basepoint-attribute"></a>Atributo BasePoint

|**Valor**|**Descrição**|
|:-----|:-----|
|Início  <br/> |O exibição paged começa no início da conversa ou conjunto de itens encontrados.  <br/> |
|End  <br/> |O exibição paged começa no final da conversa ou conjunto de itens encontrados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar itens em uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Define uma solicitação para encontrar conversas em uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Comentários

Procurar desde o final envolve mover para a origem identificada pelo deslocamento. Além disso, o ponteiro é movido de volta pelo número de registros solicitados. Por exemplo, se houver 100 registros e o deslocamento for 25 a partir do final, a pesquisa começará a partir de 75. Se 10 registros são retornados, o ponteiro é movido para trás e 10 registros adicionais para 65 e retorna os registros de 65 a 75. O próximo índice é 64. O próximo deslocamento do final para uma página é 100 menos 64, o que equivale a 36. 36 é o valor do próximo deslocamento do final para obter a próxima página indexada.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma [solicitação de operação FindItem.](finditem-operation.md) Cada item é retornado com sua ID e assunto. No máximo seis itens são retornados na resposta, conforme especificado pelo **atributo MaxEntriesReturned.** Os itens são listados em ordem crescente agrupados por importância. Os itens em um grupo são agregados por assunto. 
  
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

