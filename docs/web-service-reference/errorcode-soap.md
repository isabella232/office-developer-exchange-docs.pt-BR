---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: O elemento ErrorCode representa um código de erro retornado pelo serviço de descoberta automática.
ms.openlocfilehash: d66167e51733ffcaa3d62a985d3e03e2ac80b715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460089"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

O elemento **ErrorCode** representa um código de erro retornado pelo serviço de descoberta automática. 
  
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
|[AutodiscoverResponse (SOAP)](autodiscoverresponse-soap.md) <br/> |Representa o tipo base para todas as respostas retornadas pelo serviço de descoberta automática.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Contém a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.  <br/> |
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contém a resposta a uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[Resposta (SOAP)](response-soap.md) <br/> |Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md).  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Representa um erro retornado ao recuperar uma configuração do usuário.  <br/> |
|[Userresponse (SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação de [operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o código de erro para uma resposta de erro de descoberta automática. A tabela a seguir lista os valores de texto possíveis para o elemento **ErrorCode** . 
  
|**Valor de texto do código de erro**|**Descrição**|
|:-----|:-----|
|NoError  <br/> |Não há erro.  <br/> |
|RedirectAddress  <br/> |O chamador deve seguir o redirecionamento de endereço de email retornado pela descoberta automática.  <br/> |
|RedirectUrl  <br/> |O chamador deve seguir o redirecionamento de URL retornado pela descoberta automática.  <br/> |
|InvalidUser  <br/> |O usuário que foi passado na solicitação é inválido.  <br/> |
|InvalidRequest  <br/> |A solicitação é inválida.  <br/> |
|InvalidSetting  <br/> |Uma configuração especificada é inválida.  <br/> |
|SettingIsNotAvailable  <br/> |Uma configuração especificada não está disponível.  <br/> |
|ServerBusy  <br/> |O servidor está muito ocupado para processar a solicitação.  <br/> |
|InvalidDomain  <br/> |O domínio solicitado não é válido.  <br/> |
|Não federado  <br/> |A organização não é federada.  <br/> |
|InternalServerError  <br/> |Há um erro interno no servidor.  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

