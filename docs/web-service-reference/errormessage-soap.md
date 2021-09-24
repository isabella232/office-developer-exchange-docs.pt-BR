---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: O elemento ErrorMessage representa uma mensagem associada a um código de erro retornado pelo serviço de Descoberta Automática.
ms.openlocfilehash: ebaa20f796787862ce3438bd496e29f88cb6ec6a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517074"
---
# <a name="errormessage-soap"></a>ErrorMessage (SOAP)

O **elemento ErrorMessage** representa uma mensagem associada a um código de erro retornado pelo serviço de Descoberta Automática. 
  
```XML
<ErrorMessage/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Representa o tipo base para todas as respostas retornadas pelo serviço de Descoberta Automática.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Contém a resposta a [uma chamada de operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contém a resposta a uma [solicitação getFederationInformation operation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
|[Response (SOAP)](response-soap.md) <br/> |Contém a resposta a [uma solicitação de operação GetUserSettings (SOAP).](getusersettings-operation-soap.md)  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Representa um erro retornado durante a recuperação de uma configuração do usuário.  <br/> |
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação de operação [GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a mensagem de erro.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

