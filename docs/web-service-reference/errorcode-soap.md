---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: O elemento ErrorCode representa um código de erro retornado pelo serviço descoberta automática.
ms.openlocfilehash: fa40cb8b7a2ec80ecf752058f540969013748d39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530770"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

O **elemento ErrorCode** representa um código de erro retornado pelo serviço descoberta automática. 
  
```XML
<ErrorCode/>
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

O valor de texto representa o código de erro de uma resposta de erro de Descoberta Automática. A tabela a seguir lista os valores de texto possíveis para o **elemento ErrorCode.** 
  
|**Valor de texto do código de erro**|**Descrição**|
|:-----|:-----|
|NoError  <br/> |Não houve nenhum erro.  <br/> |
|RedirectAddress  <br/> |O chamador deve seguir o redirecionamento de endereço de email retornado pela Descoberta Automática.  <br/> |
|RedirectUrl  <br/> |O chamador deve seguir o redirecionamento de URL retornado pela Descoberta Automática.  <br/> |
|InvalidUser  <br/> |O usuário que foi passado na solicitação é inválido.  <br/> |
|InvalidRequest  <br/> |A solicitação é inválida.  <br/> |
|InvalidSetting  <br/> |Uma configuração especificada é inválida.  <br/> |
|SettingIsNotAvailable  <br/> |Uma configuração especificada não está disponível.  <br/> |
|ServerBusy  <br/> |O servidor está muito ocupado para processar a solicitação.  <br/> |
|InvalidDomain  <br/> |O domínio solicitado não é válido.  <br/> |
|NotFederated  <br/> |A organização não é federada.  <br/> |
|InternalServerError  <br/> |Há um erro de servidor interno.  <br/> |
   
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

