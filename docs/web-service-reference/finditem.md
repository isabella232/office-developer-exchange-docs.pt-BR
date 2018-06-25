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
description: O elemento de FindItem define uma solicitação para localizar itens em uma caixa de correio.
ms.openlocfilehash: 9831b034be7deb0cf6e756bb585bdbe34b370afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752287"
---
# <a name="finditem"></a>FindItem

O elemento de **FindItem** define uma solicitação para localizar itens em uma caixa de correio. 
  
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

 **FindItemType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Passagem** <br/> |Define se a pesquisa localizará itens em pastas ou dumpsters das pastas. Este atributo é necessário.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores de atributos de passagem

|**Valor**|**Descrição**|
|:-----|:-----|
|Raso  <br/> |Retorna apenas as identidades dos itens na pasta.  <br/> |
|SoftDeleted  <br/> |Retorna apenas as identidades dos itens que estão em uma pasta dumpster. Observe que uma passagem excluída combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondem aos critérios de pesquisa.  <br/> |
|Associados  <br/> |Retorna apenas as identidades dos itens associados na pasta.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta de [operação FindItem](finditem-operation.md) .  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Descreve como paginados informações de item é retornada para uma solicitação de **FindItem** . Esse elemento é opcional.  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |Descreve o modo de exibição paginado inicia onde e o número máximo de itens retornados em uma solicitação de **FindItem** . O deslocamento do modo de exibição paginados desde o início do conjunto de itens encontrados descrito por uma fração. Esse elemento é opcional.  <br/> |
|[Exibição de calendário](calendarview.md) <br/> |Fornece tempo span limites para definir uma pesquisa de itens de calendário. Esse elemento é opcional.  <br/> |
|[ContactsView](contactsview.md) <br/> |Define uma pesquisa de itens de contato, com base em nomes para exibição em ordem alfabética. Esse elemento é opcional.  <br/> |
|[GroupBy](groupby.md) <br/> |Especifica agrupamentos arbitrários para consultas **FindItem** . Esse elemento é opcional.  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fornece agrupamentos padrão para consultas **FindItem** . Esse elemento é opcional.  <br/> |
|[Restriction](restriction.md) <br/> |Define a restrição ou a consulta que é usada para filtrar itens ou pastas no **FindItem**/ operações de pasta**FindFolder** e pesquisa. Esse elemento é opcional.  <br/> |
|[SortOrder](sortorder.md) <br/> |Define como os itens são classificados em uma solicitação de FindItem. Esse elemento é opcional.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica as pastas para procurar as operações FindItem e FindFolder.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Contém uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Somente um do [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md)ou [ContactsView](contactsview.md) elementos pode ser incluído em uma solicitação de **FindItem** . Somente um dos elementos [GroupBy](groupby.md) ou [DistinguishedGroupBy](distinguishedgroupby.md) pode ser incluído em uma solicitação de **FindItem** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
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

