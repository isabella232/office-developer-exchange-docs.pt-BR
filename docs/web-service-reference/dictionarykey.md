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
description: O elemento DictionaryKey especifica a chave de dicionário para uma propriedade Dictionary.
ms.openlocfilehash: 8d9d897c86eb5048068936433c6c0d77917ff777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462147"
---
# <a name="dictionarykey"></a>DictionaryKey

O elemento **DictionaryKey** especifica a chave de dicionário para uma propriedade Dictionary. 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 **UserConfigurationDictionaryObjectType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Tipo (userconfiguration)](type-userconfiguration.md) <br/> | Especifica um tipo de objeto Dictionary.<br/><br/>O tipo pode ser um dos seguintes valores de cadeia de caracteres:<br/><br/>-DateTime  <br/>-Boolean  <br/>-Byte  <br/>-String  <br/>- Integer32  <br/>- UnsignedInteger32  <br/>- Integer64  <br/>- UnsignedInteger64  <br/>- StringArray  <br/>-ByteArray  <br/> |
|[Valor (userconfiguration)](value-userconfiguration.md) <br/> |Especifica o valor do objeto Dictionary como uma cadeia de caracteres.  <br/> |
   
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
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

