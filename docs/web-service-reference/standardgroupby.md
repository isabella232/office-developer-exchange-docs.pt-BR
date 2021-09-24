---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: O elemento StandardGroupBy representa os mecanismos padrão de agrupação e agregação para uma operação FindItem agrupada.
ms.openlocfilehash: b19157b9ff3a19379880b7f6b9c52835c170df21
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521274"
---
# <a name="standardgroupby"></a>StandardGroupBy

O **elemento StandardGroupBy** representa os mecanismos padrão de agrupação e agregação para uma operação FindItem agrupada. 
  
[FindItem](finditem.md)
  
[DistinguishedGroupBy](distinguishedgroupby.md)
  
[StandardGroupBy](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 **StandardGroupByType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |Fornece agrupações padrão para consultas FindItem.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O único valor que pode ser usado para esse elemento é **ConversationTopic**. **Grupos ConversationTopic** por mensagem:ConversationTopic e agregados no item:DateTimeReceived (máximo). Para obter mais informações sobre a agregação, consulte [AggregateOn](aggregateon.md).
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)
  
[FindItem](finditem.md)


[Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

