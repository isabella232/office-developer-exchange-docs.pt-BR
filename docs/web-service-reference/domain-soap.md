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
description: O elemento de domínio contém um domínio federado em uma resposta GetFederationInformation ou contém um domínio em que as definições de configuração para o qual são solicitadas em uma solicitação de GetDomainSettings.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751913"
---
# <a name="domain-soap"></a>Domínio (SOAP)

O elemento de **domínio** contém um domínio federado em uma resposta **GetFederationInformation** ou contém um domínio em que as definições de configuração para o qual são solicitadas em uma solicitação de **GetDomainSettings** . 
  
```XML
<Domain/> 
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
|[Domínios (SOAP)](domains-soap.md) <br/> |Representa os domínios que as definições de configuração para o qual são retornadas em uma operação de **GetDomainSettings** ou os domínios que a organização tem federados em uma operação de **GetFederationInformation** .  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento **domínio** representa um nome de domínio. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

