---
title: Valor (rastreamento de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: O elemento de valor representa o valor da propriedade para um relatório de controle de mensagens.
ms.openlocfilehash: 152e4fe61a4cff8013ae02900bd84bf244ae84a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838020"
---
# <a name="value-message-tracking"></a>Valor (rastreamento de mensagens)

O elemento de **valor** representa o valor da propriedade para um relatório de controle de mensagens. 
  
```xml
<Value/>
```

**String**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de acompanhamento de mensagens.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é opcional.
  
## <a name="remarks"></a>Comentários

Esse elemento pode ocorrer no máximo uma vez no elemento [TrackingPropertyType](trackingpropertytype.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

