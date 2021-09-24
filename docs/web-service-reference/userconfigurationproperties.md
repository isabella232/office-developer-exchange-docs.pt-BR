---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: O elemento UserConfigurationProperties especifica os tipos de propriedade para entrar em uma operação GetUserConfiguration.
ms.openlocfilehash: 0aed3ffc680ac881410469fe762349739ba924a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515002"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

O **elemento UserConfigurationProperties** especifica os tipos de propriedade para entrar em uma operação GetUserConfiguration. 
  
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

A tabela a seguir lista os valores possíveis para o **elemento UserConfigurationProperties.** 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Especifica a propriedade identificador.  <br/> |
|Dictionary  <br/> |Especifica tipos de propriedade de dicionário.  <br/> |
|XmlData  <br/> |Especifica tipos de propriedade de dados XML.  <br/> |
|BinaryData  <br/> |Especifica tipos de propriedade de dados binários.  <br/> |
|Todos  <br/> |Especifica o identificador, dicionário, dados XML e tipos de propriedade de dados binários.  <br/> |
   
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

