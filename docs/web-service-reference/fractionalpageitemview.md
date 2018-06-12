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
# <a name="fractionalpageitemview"></a>FractionalPageItemView

O elemento **FractionalPageItemView** descreve onde o modo de exibição paginado é iniciado e o número máximo de itens retornados em uma solicitação de [FindItem](finditem.md) . 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifica o número máximo de resultados a serem retornados na resposta [FindItem](finditem.md) . Este atributo é opcional. Se esse atributo não for especificado, a chamada retornará todos os itens disponíveis.  <br/> |
|**Numerador** <br/> |Representa o numerador do deslocamento fracional desde o início do conjunto de resultados. Este atributo é necessário. O numerador deve ser igual ou menor que o denominador. Este atributo deve representar um valor integral que é igual ou maior do que zero.  <br/> Para obter mais informações, consulte a seção comentários, mais adiante neste tópico.  <br/> |
|**Denominador** <br/> |Representa o denominador do deslocamento fracional desde o início do número total de itens no conjunto de resultados. Este atributo é necessário. Este atributo deve representar um valor inteiro maior que um.  <br/> Para obter mais informações, consulte a seção comentários, mais adiante neste tópico.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Coment�rios

O deslocamento do modo de exibição paginados desde o início do conjunto de itens encontrados descrito por uma fração. A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciado. Por exemplo, se **numerador** é igual a quatro e **denominador** igual a cinco, a página de informações retornadas começa em uma entrada localizado quatro-quintas da maneira no conjunto de resultados. 
  
Se fração for avaliada como zero, o que indica o início do conjunto de resultados. Se fração for avaliada como um, que indica o fim do conjunto de resultados.
  
> [!NOTE]
> A fração representa o ponto inicial da página, não quantos resultados no conjunto de resultados serão retornados. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Example

O exemplo a seguir mostra uma solicitação [FindItem](finditem.md) . A solicitação retorna os itens dos resultados da pesquisa que começam após o segundo terceiro de todos os itens no conjunto de resultados. 
  
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

Por exemplo, se o conjunto de resultados contiver nove itens, o modo de exibição paginado retornará até 12 itens, começando a dois terços encontrado item da maneira no conjunto de resultados. Nesse caso, a página começa com o sétimo item. A página conterá o sétimo oitavo e o nono itens. Se o numerador estiver definido como zero, o modo de exibição de página retornará todos os itens no conjunto desde que o número seja menor que o atributo **MaxEntriesReturned** de resultados. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindItem](finditem-operation.md)


[Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

