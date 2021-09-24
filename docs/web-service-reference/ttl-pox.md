---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: O elemento TTL especifica a hora de vida, em horas, durante a qual as configurações permanecem válidas.
ms.openlocfilehash: 6850f104fe90ae941f9d1d522fa3d3641e433c5f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515100"
---
# <a name="ttl-pox"></a>TTL (POX)

O **elemento TTL** especifica a hora de vida, em horas, durante a qual as configurações permanecem válidas. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[TTL (POX)](ttl-pox.md)
  
```xml
<TTL/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador Exchange Server 2007 no qual a função de servidor de Acesso para Cliente está instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa a hora de vida, em horas, durante as quais as configurações permanecem válidas. Um valor zero indica que a descoberta não é necessária. Se nenhum valor for especificado, o valor padrão para esse elemento será 1 hora.
  
## <a name="remarks"></a>Comentários

Após o tempo representado pelo elemento **TTL** ter decorrido, as configurações devem ser redescobertas usando uma solicitação de Descoberta Automática. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

