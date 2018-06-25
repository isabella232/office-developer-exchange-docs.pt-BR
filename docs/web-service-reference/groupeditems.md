---
title: GroupedItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupedItems
api_type:
- schema
ms.assetid: 53170df4-4272-4b37-b23f-cd8e2d4a7396
description: O elemento GroupedItems representa uma coleção de itens que são o resultado de uma chamada de operação FindItem agrupada.
ms.openlocfilehash: f8aed9b78fc54307f44b96a45e5c31a4cc76ab50
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823756"
---
# <a name="groupeditems"></a>GroupedItems

O elemento **GroupedItems** representa uma coleção de itens que são o resultado de uma [operação FindItem](finditem-operation.md) de agrupadas chamada. 
  
[FindItemResponse](finditemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[FindItemResponseMessage](finditemresponsemessage.md)
  
[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
  
[Grupos](groups.md)
  
[GroupedItems](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 **GroupedItemsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GroupIndex](groupindex.md) <br/> |Representa o valor da propriedade é usada para agrupar itens em uma agrupadas [FindItem operação](finditem-operation.md) chamada.  <br/> |
|[Items](items.md) <br/> |Contém uma matriz de itens agrupados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Grupos](groups.md) <br/> |Contém uma coleção dos grupos que são encontrados com os critérios de pesquisa e a agregação de lista segura é identificada na solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindItem](finditem-operation.md)


[Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

