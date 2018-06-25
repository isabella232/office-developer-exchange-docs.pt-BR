---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: Elemento ErrorMessage representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752098"
---
# <a name="errormessage-soap"></a>ErrorMessage (SOAP)

Elemento **ErrorMessage** representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática. 
  
```XML
<ErrorMessage/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Representa o tipo de base para todas as respostas que são retornados pelo serviço de descoberta automática.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Contém a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contém a resposta a uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[Resposta SOAP)](response-soap.md) <br/> |Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Representa um erro retornado ao recuperar uma configuração de usuário.  <br/> |
|[Resposta SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a mensagem de erro.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

