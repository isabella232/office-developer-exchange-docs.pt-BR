---
title: Userconfigurationproperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: O elemento userconfigurationproperties especifica os tipos de propriedade a serem obtidos em uma operação GetUserConfiguration.
ms.openlocfilehash: af6bee64516a7410d96ecc7581e8e819f550ddc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466490"
---
# <a name="userconfigurationproperties"></a>Userconfigurationproperties

O elemento **Userconfigurationproperties** especifica os tipos de propriedade a serem obtidos em uma operação GetUserConfiguration. 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **UserConfigurationPropertyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Especifica uma solicitação para obter um objeto de configuração do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **Userconfigurationproperties** . 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Especifica a propriedade Identifier.  <br/> |
|Dictionary  <br/> |Especifica os tipos de propriedade de dicionário.  <br/> |
|Nota XMLDATA  <br/> |Especifica os tipos de propriedade de dados XML.  <br/> |
|BinaryData  <br/> |Especifica tipos de propriedade de dados binários.  <br/> |
|Todos  <br/> |Especifica os tipos de propriedade de identificador, dicionário, dados XML e dados binários.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

