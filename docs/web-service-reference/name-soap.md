---
title: Nome (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: O elemento name representa o nome de uma configuração.
ms.openlocfilehash: 74e6d6b59d972d7230c23b38cd3f4a8591401bbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466882"
---
# <a name="name-soap"></a>Nome (SOAP)

O elemento **Name** representa o nome de uma configuração. 
  
```XML
<Name/>
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
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Contém as configurações de domínio retornadas pela solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |Representa um domínio que define o valor do tipo cadeia de caracteres.  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização.  <br/> |
|[Usersetting (SOAP)](usersetting-soap.md) <br/> |Representa uma configuração de usuário único.  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Representa uma coleção de configurações de conexão de protocolo de servidor.  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |Representa uma configuração de usuário do valor para o qual é do tipo cadeia de caracteres.  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Representa uma configuração de usuário que é uma coleção de URLs de cliente da Web do Exchange.  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Contém uma coleção de configurações de caixa de correio alternativas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Name** é o nome de uma configuração. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

