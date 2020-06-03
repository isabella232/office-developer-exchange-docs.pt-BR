---
title: Domínios (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: O elemento Domains representa o conjunto de domínios que é retornado em uma operação GetDomainSettings (SOAP), os domínios que a organização tem federado em uma operação do GetFederationInformation (SOAP) ou os domínios com um relacionamento de organização, conforme retornado pela operação de GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526302"
---
# <a name="domains-soap"></a>Domínios (SOAP)

O elemento **Domains** representa o conjunto de domínios que é retornado em uma [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), os domínios que a organização tem federado em uma [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou os domínios com um relacionamento de organização, conforme RETORNADO pela operação de [GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 **Domínios**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domínio (SOAP)](domain-soap.md) <br/> |Representa um único domínio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Representa uma solicitação de [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
|[Resposta (GetFederationInformation) (SOAP)](response-getfederationinformationsoap.md) <br/> |Contém as informações de resposta da [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
|[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) <br/> |Representa uma solicitação de [operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .  <br/> |
   
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

- [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md)  
- [GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md)

