---
title: Request (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: O elemento Request contém a solicitação para o serviço descoberta automática.
ms.openlocfilehash: 91bc9cad6df976e8a8500eecc997f573a7df7289
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542830"
---
# <a name="request-pox"></a>Request (POX)

O **elemento Request** contém a solicitação para o serviço descoberta automática. 
  
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

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md) <br/> |Identifica o esquema de uma resposta de Descoberta Automática.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Identifica o endereço de email do usuário.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifica a caixa de correio de um usuário pelo nome diferenciado herdado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AutoDiscover (POX)](autodiscover-pox.md) <br/> |O elemento raiz em uma solicitação de Descoberta Automática.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

