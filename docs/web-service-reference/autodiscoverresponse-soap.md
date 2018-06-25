---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: O elemento AutodiscoverResponse (SOAP) representa o elemento base para todas as respostas que são retornados pelo serviço de descoberta automática.
ms.openlocfilehash: b92a71deb77e2b1dee42d970e2dc43a56044487a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751244"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

O elemento **AutodiscoverResponse (SOAP)** representa o elemento base para todas as respostas que são retornados pelo serviço de descoberta automática. 
  
- [AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **AutodiscoverResponse**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Representa uma coleção de elementos de [Resposta (SOAP)](userresponse-soap.md) .  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Representa uma coleção de elementos de [UserSettingError (SOAP)](usersettingerror-soap.md) .  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Representa uma coleção de elementos de [UserSetting (SOAP)](usersetting-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

