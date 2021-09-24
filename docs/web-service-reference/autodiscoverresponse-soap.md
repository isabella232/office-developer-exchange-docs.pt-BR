---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: O elemento AutodiscoverResponse (SOAP) representa o elemento base para todas as respostas retornadas pelo serviço descoberta automática.
ms.openlocfilehash: 71bbb0f1aa6602a260c163ccfdfd3c3d38442e31
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514869"
---
# <a name="autodiscoverresponse-soap"></a>AutodiscoverResponse (SOAP)

O **elemento AutodiscoverResponse (SOAP)** representa o elemento base para todas as respostas retornadas pelo serviço descoberta automática. 
  
- [AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 **AutodiscoverResponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UserResponses (SOAP)](userresponses-soap.md) <br/> |Representa uma coleção de [elementos UserResponse (SOAP).](userresponse-soap.md)  <br/> |
|[UserSettingErrors (SOAP)](usersettingerrors-soap.md) <br/> |Representa uma coleção de [elementos UserSettingError (SOAP).](usersettingerror-soap.md)  <br/> |
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Representa uma coleção de [elementos UserSetting (SOAP).](usersetting-soap.md)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

