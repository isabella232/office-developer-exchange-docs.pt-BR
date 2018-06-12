---
title: DistinguishedGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: O elemento DistinguishedGroupBy fornece agrupamentos padrão para consultas FindItem.
ms.openlocfilehash: 0635366447675bf28dedf3af4f7d76094ee5e0a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751897"
---
# <a name="distinguishedgroupby"></a>DistinguishedGroupBy

O elemento **DistinguishedGroupBy** fornece agrupamentos padrão para consultas FindItem. 
  
- [FindItem](finditem.md) 
- [DistinguishedGroupBy](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 **DistinguishedGroupByType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardGroupBy](standardgroupby.md) <br/> |Representa o padrão de agrupamento e agregar mecanismos para uma operação de FindItem agrupada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.<br/><br/>Este é a expressão XPath para esse elemento:`/FindItem` <br/> |
   
## <a name="remarks"></a>Coment�rios

O elemento **DistinguishedGroupBy** pode ser adicionado a uma operação FindItem quando os resultados devem vir armazenados agrupados e quando um dos grupos padrão atende aos requisitos de agrupamento. Se nem o elemento **DistinguishedGroupBy** nem o elemento [GroupBy](groupby.md) for especificado, desagrupado FindItem resultados retornarão. 
  
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
- [Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

