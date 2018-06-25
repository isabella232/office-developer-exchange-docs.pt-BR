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
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837805"
---
# <a name="ttl-pox"></a>TTL (POX)

O elemento **TTL** Especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[TTL (POX)](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador do Exchange Server 2007 em que a função de servidor acesso para cliente está instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o tempo de vida, em horas, durante o qual as configurações permanecem válidas. Um valor de zero indica que redescoberta não é necessária. Se nenhum valor for especificado, o valor padrão para esse elemento é 1 hora.
  
## <a name="remarks"></a>Comentários

Após a hora em que é representada pelo elemento **TTL** decorrido, as configurações devem ser redescobertas usando uma solicitação de descoberta automática. 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

