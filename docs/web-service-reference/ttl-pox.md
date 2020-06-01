---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: O elemento TTL especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas.
ms.openlocfilehash: 9a17cbe4e669d1afe9f3ef4a24f2a9a2889a7d52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467379"
---
# <a name="ttl-pox"></a>TTL (POX)

O elemento **TTL** especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador do Exchange Server 2007 no qual a função de servidor de acesso para cliente está instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o tempo de vida, em horas, durante o qual as configurações permanecem válidas. Um valor igual a zero indica que a redescoberta não é necessária. Se nenhum valor for especificado, o valor padrão para esse elemento será 1 hora.
  
## <a name="remarks"></a>Comentários

Após o tempo que é representado pelo elemento **TTL** ter decorrido, as configurações devem ser redescobertas usando uma solicitação de descoberta automática. 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

