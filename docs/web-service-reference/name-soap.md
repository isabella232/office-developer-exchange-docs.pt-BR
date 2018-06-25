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
description: O elemento Name representa o nome de uma configuração.
ms.openlocfilehash: 4689c306bb805a40fea0d58c9e04a5a47d3bb14d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824506"
---
# <a name="name-soap"></a>Nome (SOAP)

O elemento **Name** representa o nome de uma configuração. 
  
```XML
<Name/>
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
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Contém configurações de domínio que são retornadas por solicitação [GetDomainSettings operação (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |Representa uma configuração de domínio, o valor da qual é do tipo string.  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relacionamentos de organização para uma única organização.  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |Representa uma configuração de usuário único.  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Representa uma coleção de configurações de conexão do protocolo de servidor.  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |Representa uma configuração de usuário, o valor para o qual é do tipo string.  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Representa um usuário de configuração que é uma coleção de URLs de cliente da Web do Exchange.  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Contém uma coleção de definições de caixa de correio alternativo.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento **Name** é o nome de uma configuração. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
- [Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

