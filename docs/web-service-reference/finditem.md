---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: O elemento FindItem define uma solicitação para localizar itens em uma caixa de correio.
ms.openlocfilehash: 3aeda1cffc03292734a91bc3fff3289d51c9b445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460992"
---
# <a name="finditem"></a>FindItem

O elemento **FindItem** define uma solicitação para localizar itens em uma caixa de correio. 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


**FindItemType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Passagem** <br/> |Define se a pesquisa localiza itens nas pastas ou nos dumpster das pastas. Esse atributo é necessário.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores de atributos de passagem

|**Valor**|**Descrição**|
|:-----|:-----|
|Superficial  <br/> |Retorna somente as identidades dos itens na pasta.  <br/> |
|SoftDeleted  <br/> |Retorna somente as identidades dos itens que estão no dumpster de uma pasta. Observe que uma passagem com exclusão reversível combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondam aos critérios de pesquisa.  <br/> |
|Ao  <br/> |Retorna somente as identidades dos itens associados na pasta.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Shape](itemshape.md) <br/> |Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta de [operação do FindItem](finditem-operation.md) .  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Descreve como as informações de item paginado são retornadas para uma solicitação **FindItem** . Este elemento é opcional.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Descreve onde o modo de exibição paginado começa e o número máximo de itens retornados em uma solicitação **FindItem** . O deslocamento de modo de exibição paginado desde o início do conjunto de itens encontrados é descrito por uma fração. Este elemento é opcional.  <br/> |
|[Modo de exibição do Calendário](calendarview.md) <br/> |Fornece limites de intervalo de tempo para definir uma pesquisa para itens de calendário. Este elemento é opcional.  <br/> |
|[ContactsView](contactsview.md) <br/> |Define uma pesquisa para itens de contato com base em nomes de exibição em ordem alfabética. Este elemento é opcional.  <br/> |
|[GroupBy](groupby.md) <br/> |Especifica agrupamentos arbitrários para consultas do **FindItem** . Este elemento é opcional.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fornece agrupamentos padrão para consultas do **FindItem** . Este elemento é opcional.  <br/> |
|[Restriction](restriction.md) <br/> |Define a restrição ou a consulta usada para filtrar itens ou pastas no **FindItem** /  **FindFolder** e nas operações da pasta de pesquisa. Este elemento é opcional.  <br/> |
|[SortOrder](sortorder.md) <br/> |Define como os itens são classificados em uma solicitação FindItem. Este elemento é opcional.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica as pastas nas quais as operações do FindItem e do FindFolder serão pesquisadas.  <br/> |
|[QueryString (QueryStringtype)](querystring-querystringtype.md) <br/> |Contém uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

Somente um dos elementos [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) pode ser incluído em uma solicitação de **FindItem** . Somente um dos elementos [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) pode ser incluído em uma solicitação **FindItem** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindItem](finditem-operation.md)
- [Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

