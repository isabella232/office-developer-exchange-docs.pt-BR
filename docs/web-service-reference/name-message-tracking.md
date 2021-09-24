---
title: Name (Message Tracking)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: O elemento Name representa o nome da propriedade de um relatório de controle de mensagens.
ms.openlocfilehash: b57c109cfbcb2744ae6854e0afce52e240d22b30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515450"
---
# <a name="name-message-tracking"></a>Name (Message Tracking)

O **elemento Name** representa o nome da propriedade de um relatório de controle de mensagens. 
  
```xml
<Name/>
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

Um valor de texto será necessário se esse elemento for usado.
  
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

