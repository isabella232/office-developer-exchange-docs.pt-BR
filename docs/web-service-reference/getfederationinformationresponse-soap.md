---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: O elemento GetFederationInformationResponse contém a resposta de operação (SOAP) GetFederationInformation.
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752498"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

O elemento **GetFederationInformationResponse** contém a resposta de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Define o local de um aplicativo.  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Representa uma coleção de tokens de segurança, que contêm pontos de extremidade e identificadores de serviço de token de segurança.  <br/> |
|[Domínios (SOAP)](domains-soap.md) <br/> |Representa os domínios que as configurações para o qual são retornadas em uma operação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou os domínios que a organização tem federados em uma [operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) Operação **GetFederationInformation** .  <br/> |
   
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



[Operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

