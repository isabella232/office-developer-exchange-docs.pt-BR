---
title: Domínio (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: O elemento Domain contém um domínio federado em uma resposta GetFederationInformation ou contém um domínio as definições de configuração para as quais são solicitadas em uma solicitação GetDomainSettings.
ms.openlocfilehash: f90c608ee1fc3356a227bca6411eaeff0c1e8b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456980"
---
# <a name="domain-soap"></a>Domínio (SOAP)

O elemento **Domain** contém um domínio federado em uma resposta **GetFederationInformation** ou contém um domínio as definições de configuração para as quais são solicitadas em uma solicitação **GetDomainSettings** . 
  
```XML
<Domain/> 
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
|[Domínios (SOAP)](domains-soap.md) <br/> |Representa os domínios em que as definições de configuração para as quais são retornadas em uma operação **GetDomainSettings** ou os domínios que a organização federaram em uma operação **GetFederationInformation** .  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Domain** representa um nome de domínio. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

