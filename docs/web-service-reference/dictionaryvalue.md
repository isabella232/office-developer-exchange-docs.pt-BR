---
title: DictionaryValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DictionaryValue
api_type:
- schema
ms.assetid: f4089381-826f-4f6a-8c6d-e51b910cbe6d
description: O elemento DictionaryValue especifica o valor de dicionário de uma propriedade de dicionário.
ms.openlocfilehash: c50563effc7435442dc3caf67b350533b9517eb0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546641"
---
# <a name="dictionaryvalue"></a>DictionaryValue

O **elemento DictionaryValue** especifica o valor de dicionário de uma propriedade de dicionário. 
  
```xml
<DictionaryValue>
   <Type/>
   <Value/>
</DictionaryValue>
```

 **UserConfigurationDictionaryObjectType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Type (UserConfiguration)](type-userconfiguration.md) <br/> |Especifica o tipo de objeto dictionary.  <br/> |
|[Value (UserConfiguration)](value-userconfiguration.md) <br/> |Especifica o valor do objeto dictionary como uma cadeia de caracteres.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Especifica o conteúdo de uma única propriedade de entrada de dicionário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

