---
title: Domain (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: O elemento Domain contém um domínio federado em uma resposta GetFederationInformation ou contém um domínio para o qual as configurações são solicitadas em uma solicitação GetDomainSettings.
ms.openlocfilehash: a2e69dc845f9841931263fe90e39550bceb81ab8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520819"
---
# <a name="domain-soap"></a>Domain (SOAP)

O **elemento Domain** contém um domínio federado em uma resposta **GetFederationInformation** ou contém um domínio para o qual as configurações são solicitadas em uma solicitação **GetDomainSettings.** 
  
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
|[Domains (SOAP)](domains-soap.md) <br/> |Representa os domínios para os quais as configurações são retornadas em uma operação **GetDomainSettings** ou os domínios que a organização federou em uma **operação GetFederationInformation.**  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Domain** representa um nome de domínio. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

