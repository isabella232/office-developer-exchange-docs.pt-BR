---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: O elemento StandardGroupBy representa o padrão de agrupamento e agregar mecanismos para uma operação de FindItem agrupada.
ms.openlocfilehash: 8e2ec72a79ebafc2e5757d6dcebb27c0c53ec0b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825542"
---
# <a name="standardgroupby"></a>StandardGroupBy

O elemento **StandardGroupBy** representa o padrão de agrupamento e agregar mecanismos para uma operação de FindItem agrupada. 
  
[FindItem](finditem.md)
  
[DistinguishedGroupBy](distinguishedgroupby.md)
  
[StandardGroupBy](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 **StandardGroupByType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fornece agrupamentos padrão para consultas FindItem.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O único valor que pode ser usado para esse elemento é **ConversationTopic**. Grupos de **ConversationTopic** por mensagem: ConversationTopic e agregados no item: DateTimeReceived (máximo). Para obter mais informações sobre agregação de lista segura, consulte [AggregateOn](aggregateon.md).
  
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindItem](finditem-operation.md)
  
[FindItem](finditem.md)


[Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

