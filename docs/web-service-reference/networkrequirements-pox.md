---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: O elemento NetworkRequirements contém os critérios usados para determinar se o computador cliente está em uma rede que atende aos requisitos do provedor de serviços da Internet (ISP) para se conectar ao servidor.
ms.openlocfilehash: 07a258ad48b74c614ce367db0f893ed884cf3f75
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509509"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

O **elemento NetworkRequirements** contém os critérios usados para determinar se o computador cliente está em uma rede que atende aos requisitos do provedor de serviços da Internet (ISP) para se conectar ao servidor. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[NetworkRequirements (POX)](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Identifica o início de um intervalo de endereços IP versão 4 (IPv4) usados para identificar um computador em uma rede.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Identifica o final de um intervalo de endereços IP versão 4 (IPv4) usados para identificar um computador na rede.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Identifica o início de um intervalo de endereços IP versão 6 (IPv6) usados para identificar um computador em uma rede.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Identifica o final de um intervalo de endereços IP versão 6 (IPv6) usados para identificar um computador em uma rede.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="remarks"></a>Comentários

Se o cliente de email não corresponder aos requisitos de rede, ele deverá tentar outros tipos de protocolo. Os ISPs podem fornecer um conjunto de servidores com marcas [de Protocolo (POX)](protocol-pox.md) que não exigem autenticação, mas são necessários para estar na rede ISP. OS ISPs podem listar outro conjunto de servidores que exigem autenticação, mas não são necessários para estar em uma rede específica. 
  
O **elemento NetworkRequirements** é opcional. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

