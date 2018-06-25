---
title: DictionaryEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryEntry
api_type:
- schema
ms.assetid: 531ea96a-d411-43e6-9fec-11fa2c959a30
description: O elemento DictionaryEntry Especifica o conteúdo de uma propriedade de entrada do dicionário único.
ms.openlocfilehash: 75d7dd1aa82a4cc6c363b9c787cfb15b4d15b656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751805"
---
# <a name="dictionaryentry"></a>DictionaryEntry

O elemento **DictionaryEntry** Especifica o conteúdo de uma propriedade de entrada do dicionário único. 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 **UserConfigurationDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DictionaryKey](dictionarykey.md) <br/> |Especifica a chave de dicionário para uma propriedade de dicionário.  <br/> |
|[DictionaryValue](dictionaryvalue.md) <br/> |Especifica o valor do dicionário para uma propriedade de dicionário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[dicionário](dictionary.md) <br/> |Define um conjunto de entradas de propriedade de dicionário para um objeto de configuração do usuário.  <br/> |
   
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

