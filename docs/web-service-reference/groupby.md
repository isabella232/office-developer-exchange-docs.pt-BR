---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: O elemento GroupBy especifica um grupo arbitrário para consultas FindItem.
ms.openlocfilehash: 15e2d818ceae81f08ad0c52d9bdc881f7c3e2579
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539799"
---
# <a name="groupby"></a>GroupBy

O **elemento GroupBy** especifica um grupo arbitrário para consultas FindItem. 
  
- [FindItem](finditem.md)
- [GroupBy](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

**GroupByType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Order** <br/> | Determina a ordem dos grupos na matriz de itens agrupados retornada na resposta. Esse atributo é do tipo SortDirectionType.  <br/> |
   
#### <a name="order-attribute-values"></a>Ordenar valores de atributo

|**Valor**|**Descrição**|
|:-----|:-----|
|Crescente  <br/> |Os grupos são ordenados em ordem crescente.  <br/> |
|Decrescente  <br/> |Os grupos são ordenados em ordem decrescente.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica propriedades referenciadas com frequência por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica propriedades MAPI estendidas para obter, definir ou criar.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Representa o campo usado para determinar a ordem dos grupos em uma resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar itens em uma caixa de correio.  <br/><br/> Veja a seguir a expressão XPath para este elemento:  `/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

A resposta FindItem conterá uma coleção de grupos. Cada grupo conterá todos os itens que tinham valores correspondentes para a **propriedade GroupBy.** A propriedade que determina o agrupamento é identificada no [elemento FieldURI,](fielduri.md) [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI.](extendedfielduri.md) 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindItem](finditem-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

