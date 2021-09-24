---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: O elemento FindItem define uma solicitação para encontrar itens em uma caixa de correio.
ms.openlocfilehash: 7005b4a837c61ffa00a49b687e729de7ed769bcf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541312"
---
# <a name="finditem"></a>FindItem

O **elemento FindItem** define uma solicitação para encontrar itens em uma caixa de correio. 
  
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
|**Traversal** <br/> |Define se a pesquisa localiza itens em pastas ou lixeiras das pastas. Esse atributo é necessário.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores do atributo traversal

|**Valor**|**Descrição**|
|:-----|:-----|
|Superficial  <br/> |Retorna apenas as identidades dos itens na pasta.  <br/> |
|SoftDeleted  <br/> |Retorna apenas as identidades dos itens que estão na lixeira de uma pasta. Observe que uma transição excluída de forma suave combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que corresponderem aos critérios de pesquisa.  <br/> |
|Associado  <br/> |Retorna apenas as identidades dos itens associados na pasta.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta de [operação FindItem.](finditem-operation.md)  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Descreve como as informações de item paged são retornadas para uma **solicitação FindItem.** Esse elemento é opcional.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Descreve onde o exibição pagedo é iniciado e o número máximo de itens retornados em uma **solicitação FindItem.** O deslocamento de exibição pagedo desde o início do conjunto de itens encontrados é descrito por uma fração. Esse elemento é opcional.  <br/> |
|[Modo de exibição do Calendário](calendarview.md) <br/> |Fornece limites de intervalo de tempo para definir uma pesquisa de itens de calendário. Esse elemento é opcional.  <br/> |
|[ContactsView](contactsview.md) <br/> |Define uma pesquisa de itens de contato com base em nomes de exibição alfabéticos. Esse elemento é opcional.  <br/> |
|[GroupBy](groupby.md) <br/> |Especifica agrupações arbitrárias para consultas **FindItem.** Esse elemento é opcional.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fornece agrupações padrão para consultas **FindItem.** Esse elemento é opcional.  <br/> |
|[Restriction](restriction.md) <br/> |Define a restrição ou consulta usada para filtrar itens ou pastas em **FindItem** /  **FindFolder** e operações de pasta de pesquisa. Esse elemento é opcional.  <br/> |
|[SortOrder](sortorder.md) <br/> |Define como os itens são classificação em uma solicitação FindItem. Esse elemento é opcional.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica pastas para pesquisar as operações FindItem e FindFolder.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Contém uma cadeia de caracteres de consulta de caixa de correio com base na Sintaxe de Consulta Avançada (AQS).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Somente um dos elementos [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView,](fractionalpageitemview.md) [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) pode ser incluído em uma solicitação **FindItem.** Somente um dos elementos [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) pode ser incluído em uma **solicitação FindItem.** 
  
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

