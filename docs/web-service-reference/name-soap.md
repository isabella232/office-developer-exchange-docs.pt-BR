---
title: Name (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: dce6d823-dc33-4a47-babe-6370a15ac7b4
description: O elemento Name representa o nome de uma configuração.
ms.openlocfilehash: 39bb2b6bbf7e29dedb13a9bf828f130c076dfb6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541991"
---
# <a name="name-soap"></a>Name (SOAP)

O **elemento Name** representa o nome de uma configuração. 
  
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
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Contém configurações de domínio que são retornadas pela solicitação [da operação GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
|[DomainStringSetting (SOAP)](domainstringsetting-soap.md) <br/> |Representa um domínio que configura o valor do qual é da cadeia de caracteres de tipo.  <br/> |
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização.  <br/> |
|[UserSetting (SOAP)](usersetting-soap.md) <br/> |Representa uma única configuração de usuário.  <br/> |
|[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md) <br/> |Representa uma coleção de configurações de conexão de protocolo de servidor.  <br/> |
|[StringSetting (SOAP)](stringsetting-soap.md) <br/> |Representa um usuário definindo o valor para o qual é da cadeia de caracteres de tipo.  <br/> |
|[WebClientUrlCollectionSetting (SOAP)](webclienturlcollectionsetting-soap.md) <br/> |Representa uma configuração de usuário que é uma coleção de URLs Exchange cliente Web.  <br/> |
|[AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md) <br/> |Contém uma coleção de configurações de caixa de correio alternativa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Name** é o nome de uma configuração. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
- [Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

