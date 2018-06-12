---
title: DictionaryKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: O elemento DictionaryKey Especifica a chave de dicionário para uma propriedade de dicionário.
ms.openlocfilehash: 7e706f16fe155278ea56f303ffbb5971c1779879
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751807"
---
# <a name="dictionarykey"></a>DictionaryKey

O elemento **DictionaryKey** Especifica a chave de dicionário para uma propriedade de dicionário. 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 **UserConfigurationDictionaryObjectType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Tipo (UserConfiguration)](type-userconfiguration.md) <br/> | Especifica um tipo de objeto do dicionário.<br/><br/>O tipo pode ser um dos valores de cadeia de caracteres a seguir:<br/><br/>-DateTime  <br/>-Boolean  <br/>-Byte  <br/>-String  <br/>-Integer32  <br/>-UnsignedInteger32  <br/>-Integer64  <br/>-UnsignedInteger64  <br/>-StringArray  <br/>-ByteArray  <br/> |
|[Valor (UserConfiguration)](value-userconfiguration.md) <br/> |Especifica o valor do objeto dictionary como uma cadeia de caracteres.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Especifica o conteúdo de uma propriedade de entrada do dicionário único.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

