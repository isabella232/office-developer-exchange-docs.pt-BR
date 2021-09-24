---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: O elemento FractionalPageItemView descreve onde o exibição paged é iniciado e o número máximo de itens retornados em uma solicitação FindItem.
ms.openlocfilehash: 0d948bad0ba24c4a105be32daa645d1864cb4f3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530237"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

O **elemento FractionalPageItemView** descreve onde o exibição paged é iniciado e o número máximo de itens retornados em uma [solicitação FindItem.](finditem.md) 
  
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
|**MaxEntriesReturned** <br/> |Identifica o número máximo de resultados a ser retornado na [resposta FindItem.](finditem.md) Esse atributo é opcional. Se esse atributo não for especificado, a chamada retornará todos os itens disponíveis.  <br/> |
|**Numerador** <br/> |Representa o numerador do deslocamento fracional desde o início do conjunto de resultados. Esse atributo é necessário. O numerador deve ser igual ou menor que o denominador. Esse atributo deve representar um valor integral igual ou maior que zero.  <br/> Para obter mais informações, consulte Comentários posteriormente neste tópico.  <br/> |
|**Denominador** <br/> |Representa o denominador do deslocamento fracional desde o início do número total de itens no conjunto de resultados. Esse atributo é necessário. Esse atributo deve representar um valor integral maior do que um.  <br/> Para obter mais informações, consulte Comentários posteriormente neste tópico.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar itens em uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

O deslocamento de exibição pagedo do início do conjunto de itens encontrados é descrito por uma fração. A fração, que é definida pelos **atributos Numerador** e **Denominador,** descreve onde a página de informações é iniciada. Por exemplo, se **Numerador** for igual a quatro e **Denominador** for igual a cinco, a página de informações retornadas começará em uma entrada localizada quatro quintos do caminho para o conjunto de resultados. 
  
Se a fração for avaliada como zero, isso indicará o início do conjunto de resultados. Se a fração for avaliada como um, isso indicará o final do conjunto de resultados.
  
> [!NOTE]
> A fração representa o ponto inicial da página, e não quantos resultados no conjunto de resultados serão retornados. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma [solicitação FindItem.](finditem.md) A solicitação retorna itens dos resultados da pesquisa que começam após o segundo terço de todos os itens no conjunto de resultados. 
  
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

Por exemplo, se o conjunto de resultados contiver nove itens, o modo de exibição pagedo retornará até 12 itens, começando no item encontrado dois terços do caminho para o conjunto de resultados. Nesse caso, a página começa no sétimo item. A página conterá o sétimo, oitavo e nono itens. Se o numerador estiver definido como zero, o exibição de página retornará todos os itens no conjunto de resultados, desde que o número seja menor que o **atributo MaxEntriesReturned.** 
  
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

