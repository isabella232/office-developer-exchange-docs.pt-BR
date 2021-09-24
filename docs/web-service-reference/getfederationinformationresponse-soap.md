---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: O elemento GetFederationInformationResponse contém a resposta getFederationInformation operation (SOAP).
ms.openlocfilehash: 20d00f047acae6c9eba1347ae7e8110656fefb4b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529876"
---
# <a name="getfederationinformationresponse-soap"></a>GetFederationInformationResponse (SOAP)

O **elemento GetFederationInformationResponse** contém a [resposta getFederationInformation operation (SOAP).](getfederationinformation-operation-soap.md) 
  
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
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem associada a um código de erro retornado pelo serviço de Descoberta Automática.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Define o local de um aplicativo.  <br/> |
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Representa uma coleção de tokens de segurança, que contêm identificadores e pontos de extremidade do serviço de token de segurança.  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |Representa os domínios para os quais as configurações são retornadas em uma operação [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou os domínios que a organização federou em uma operação [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operação.  <br/> |
   
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



[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

