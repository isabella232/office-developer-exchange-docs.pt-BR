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
# <a name="fractionalpageitemview"></a>FractionalPageItemView

O elemento **FractionalPageItemView** descreve onde o modo de exibição paginado começa e o número máximo de itens retornados em uma solicitação [FindItem](finditem.md) . 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifica o número máximo de resultados a serem retornados na resposta [FindItem](finditem.md) . Esse atributo é opcional. Se esse atributo não for especificado, a chamada retornará todos os itens disponíveis.  <br/> |
|**Numera** <br/> |Representa o numerador do deslocamento fracionado do início do conjunto de resultados. Esse atributo é necessário. O numerador deve ser igual ou menor que o denominador. Este atributo deve representar um valor inteiro igual ou maior que zero.  <br/> Para obter mais informações, consulte comentários mais adiante neste tópico.  <br/> |
|**Denominado** <br/> |Representa o denominador do deslocamento fracionado desde o início do número total de itens no conjunto de resultados. Esse atributo é necessário. Este atributo deve representar um valor integral maior que um.  <br/> Para obter mais informações, consulte comentários mais adiante neste tópico.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

O deslocamento de modo de exibição paginado desde o início do conjunto de itens encontrados é descrito por uma fração. A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciada. Por exemplo, se o **numerador** for igual a quatro e o **denominador** for igual a cinco, a página de informações retornadas será iniciada em uma entrada localizada em quatro cinco quinto da forma no conjunto de resultados. 
  
Se a fração for avaliada como zero, isso indica o início do conjunto de resultados. Se a fração for avaliada como um, isso indica o final do conjunto de resultados.
  
> [!NOTE]
> A fração representa o ponto de início da página, não quantos resultados serão retornados no conjunto de resultados. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação [FindItem](finditem.md) . A solicitação retorna itens dos resultados da pesquisa que começam após o segundo terço de todos os itens no conjunto de resultados. 
  
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

Por exemplo, se o conjunto de resultados contiver nove itens, o modo de exibição paginado retornará até 12 itens, começando no item encontrado dois terços da forma no conjunto de resultados. Nesse caso, a página começa no sétimo item. A página conterá os sétimo, oitavo e nono itens. Se o numerador for definido como zero, o modo de exibição de página retornará todos os itens no conjunto de resultados, desde que o número seja menor do que o atributo **MaxEntriesReturned** . 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)


[Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

