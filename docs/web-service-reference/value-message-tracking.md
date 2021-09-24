---
title: Value (Message Tracking)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: O elemento Value representa o valor da propriedade de um relatório de controle de mensagens.
ms.openlocfilehash: c8aa4f3cc41e76b633ee1b244371de2f5410c944
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513959"
---
# <a name="value-message-tracking"></a>Value (Message Tracking)

O **elemento Value** representa o valor da propriedade de um relatório de controle de mensagens. 
  
```xml
<Value/>
```

**String**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Representa um nome e um par de valores de cadeias de caracteres usadas para criar propriedades para relatórios de controle de mensagens.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto é opcional.
  
## <a name="remarks"></a>Comentários

Esse elemento pode ocorrer no máximo uma vez no [elemento TrackingPropertyType.](trackingpropertytype.md) 
  
O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

