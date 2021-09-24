---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: O elemento SPA indica se a Autenticação de Senha Segura (SPA) é necessária.
ms.openlocfilehash: 8737a5b923d4f59c2819f7574924352223ac3673
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540409"
---
# <a name="spa-pox"></a>SPA (POX)

O **elemento SPA** indica se a Autenticação de Senha Segura (SPA) é necessária. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[SPA (POX)](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto indica se o SPA é necessário. Se o valor do texto **estiver em**, SPA será necessário.
  
## <a name="remarks"></a>Comentários

Se esse elemento não estiver presente, o valor padrão será definido como **em**.
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

