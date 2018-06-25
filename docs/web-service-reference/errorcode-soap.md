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
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752088"
---
# <a name="errorcode-soap"></a>ErrorCode (SOAP)

O elemento **ErrorCode** representa um código de erro retornado pelo serviço de descoberta automática. 
  
```XML
<ErrorCode/>
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
|[Resposta SOAP)](response-soap.md) <br/> |Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md).  <br/> |
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Representa um erro retornado ao recuperar uma configuração de usuário.  <br/> |
|[Resposta SOAP)](userresponse-soap.md) <br/> |Representa uma resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o código de erro para uma resposta de erro de descoberta automática. A tabela a seguir lista os valores de texto possíveis para o elemento **ErrorCode** . 
  
|**Valor de texto de código de erro**|**Descrição**|
|:-----|:-----|
|NoError  <br/> |Não houve nenhum erro.  <br/> |
|RedirectAddress  <br/> |O chamador deve seguir o redirecionamento de endereço de email que foi retornado por descoberta automática.  <br/> |
|RedirectUrl  <br/> |O chamador deve seguir o redirecionamento de URL que foi retornado por descoberta automática.  <br/> |
|InvalidUser  <br/> |O usuário que foi passado na solicitação é inválido.  <br/> |
|InvalidRequest  <br/> |A solicitação é inválida.  <br/> |
|InvalidSetting  <br/> |Uma configuração especificada é inválida.  <br/> |
|SettingIsNotAvailable  <br/> |Uma configuração especificada não está disponível.  <br/> |
|ServerBusy  <br/> |O servidor está muito ocupado para processar a solicitação.  <br/> |
|InvalidDomain  <br/> |O domínio solicitado não é válido.  <br/> |
|NotFederated  <br/> |A organização não é federada.  <br/> |
|InternalServerError  <br/> |Não há um erro interno do servidor.  <br/> |
   
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

