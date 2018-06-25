---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: O elemento GroupBy Especifica um agrupamento arbitrário para consultas FindItem.
ms.openlocfilehash: d85c0fddec244c99dfbea1f85da331fc5319536d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823753"
---
# <a name="groupby"></a>GroupBy

O elemento **GroupBy** Especifica um agrupamento arbitrário para consultas FindItem. 
  
- [FindItem](finditem.md)
- [GroupBy](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

 **GroupByType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Order** <br/> | Determina a ordem dos grupos da matriz de item agrupado que é retornado em tempo de resposta. Este atributo é do tipo SortDirectionType.  <br/> |
   
#### <a name="order-attribute-values"></a>Valores de atributos de ordem

|**Valor**|**Descrição**|
|:-----|:-----|
|Crescente  <br/> |Os grupos são classificados em ordem crescente.  <br/> |
|Decrescente  <br/> |Os grupos são classificados em ordem decrescente.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades estendidas de MAPI para obter, definir ou criar.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Representa o campo que é usado para determinar a ordem dos grupos em uma resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/><br/> Este é a expressão XPath para esse elemento:`/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

A resposta FindItem conterá uma coleção dos grupos. Cada grupo conterá todos os itens que tiveram valores da propriedade **GroupBy** correspondentes. A propriedade que determina o agrupamento é identificada no elemento [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação FindItem](finditem-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

