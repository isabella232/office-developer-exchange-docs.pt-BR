---
title: Request (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: O elemento de solicitação contém a solicitação para o serviço Descoberta automática.
ms.openlocfilehash: 3f5d5258a92840fe79c4936370323b78aa4715b3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354425"
---
# <a name="request-pox"></a>Request (POX)

O elemento de **solicitação** contém a solicitação para o serviço Descoberta automática. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Request (POX)](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |Identifica o esquema de uma resposta de descoberta automática.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Identifica o endereço de email do usuário.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifica a caixa de correio de um usuário por nome distinto herdado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AutoDiscover (POX)](autodiscover-pox.md) <br/> |O elemento raiz em uma solicitação de descoberta automática.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

