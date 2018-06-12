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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823919"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

O elemento **IndexedPageItemView** descreve como paginada conversa ou item a informação é retornada para uma solicitação de [operação de FindItem](finditem-operation.md) ou [FindConversation](findconversation-operation.md) . 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de itens ou conversas para retornar na resposta. Este atributo é opcional.  <br/> |
|**Offset** <br/> |Descreve o deslocamento, desde o **ponto de base**. Se o **ponto de base** é igual ao início, o deslocamento for positivo. Se o **ponto de base** for igual ao fim, o deslocamento é tratado como se fosse negativo. Isso identifica qual item ou conversa será a primeira a ser entregues a resposta. Este atributo é necessário.  <br/> |
|**Ponto de base** <br/> |Descreve como se a página de itens ou conversas será iniciado a partir do início ou no final do conjunto de itens ou conversas que são encontradas usando os critérios de pesquisa. Procurando a partir do término do sempre pesquisa para trás. Este atributo é necessário.  <br/> |
   
#### <a name="basepoint-attribute"></a>Atributo de ponto de base

|**Valor**|**Descrição**|
|:-----|:-----|
|Início  <br/> |O modo de exibição paginado começa no início do conjunto de conversa ou item encontrado.  <br/> |
|End  <br/> |O modo de exibição paginado inicia no final do conjunto de conversa ou item encontrado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Define uma solicitação para localizar conversas em uma caixa de correio.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Buscando a partir do término do envolve mover para a origem identificada pelo deslocamento. Além disso, o ponteiro é movido de volta pelo número de registros solicitados. Por exemplo, se existem 100 registros e o deslocamento for 25 do fim, a pesquisa começa a partir 75. Se 10 registros forem retornados, o ponteiro é movido para trás uma 10 adicionais registra como 65 e retorna registros 65 por meio de 75. O próximo índice é 64. O deslocamento próximo do final de uma página é 100 menos 64 que é igual a 36. 36 é o valor para o próximo deslocamento do final para obter a próxima página indexada.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Example

O exemplo a seguir mostra uma solicitação de [operação FindItem](finditem-operation.md) . Cada item é retornado com sua ID e o assunto. Um máximo de seis itens são retornados na resposta, conforme especificado pelo atributo **MaxEntriesReturned** . Os itens são listados na ordem agrupado por importância crescente. Itens em um grupo são agregados por assunto. 
  
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

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindItem](finditem-operation.md)
  
[Operação FindConversation](findconversation-operation.md)


[Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

