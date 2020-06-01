---
title: Solicitação (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: O elemento Request contém a solicitação para o serviço de descoberta automática.
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459543"
---
# <a name="request-pox"></a>Solicitação (POX)

O elemento **Request** contém a solicitação para o serviço de descoberta automática. 
  
- [Descoberta automática (POX)](autodiscover-pox.md) 
- [Solicitação (POX)](request-pox.md)
  
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

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |Identifica o esquema para uma resposta de descoberta automática.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Identifica o endereço de email do usuário.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifica a caixa de correio de um usuário com o nome diferenciado herdado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Descoberta automática (POX)](autodiscover-pox.md) <br/> |O elemento raiz em uma solicitação de descoberta automática.  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

