---
title: Dictionary
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Dictionary
api_type:
- schema
ms.assetid: 8309e468-115b-4d6e-b33c-c4719dcecc4c
description: O elemento de dicionário define um conjunto de entradas de propriedade de dicionário para um objeto de configuração do usuário.
ms.openlocfilehash: 151abfe7a9a9ae05b8b61af87c33675e025920ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751803"
---
# <a name="dictionary"></a>Dictionary

O elemento de **dicionário** define um conjunto de entradas de propriedade de dicionário para um objeto de configuração do usuário. 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 **UserConfigurationDictionaryType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Especifica o conteúdo de uma propriedade de entrada do dicionário único.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserConfiguration](userconfiguration.md) <br/> |Define um objeto de configuração de usuário único.  <br/> |
   
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

