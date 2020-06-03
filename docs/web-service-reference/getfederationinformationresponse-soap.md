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
description: O elemento GetFederationInformationResponse contém a resposta de operação do GetFederationInformation (SOAP).
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460040"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

O elemento **GetFederationInformationResponse** contém a resposta de [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) . 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Define o local de um aplicativo.  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Representa uma coleção de tokens de segurança, que contêm identificadores de serviço de token de segurança e pontos de extremidade.  <br/> |
|[Domínios (SOAP)](domains-soap.md) <br/> |Representa os domínios em que as configurações para as quais são retornadas em uma operação [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou os domínios que a organização tem federado em uma operação de **GetFederationInformation** de [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

