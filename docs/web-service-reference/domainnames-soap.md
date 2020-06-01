---
title: Usermainnames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: O elemento DomainNames representa a coleção de nomes de domínio. O elemento DomainNames é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 0b425b3cd4c0e7cb2427920d61feb04010a3b123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458415"
---
# <a name="domainnames-soap"></a>Usermainnames (SOAP)

O elemento **DomainNames** representa a coleção de nomes de domínio. O elemento **DomainNames** é somente para uso interno. Esse elemento não é usado por clientes. 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 **DomainNames**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domínios (SOAP)](domains-soap.md) <br/> |Representa uma coleção de domínios retornados da [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), [GETFEDERATIONINFORMATION Operation (SOAP)](getfederationinformation-operation-soap.md)ou a [operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento representa os domínios SMTP das organizações externas.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

