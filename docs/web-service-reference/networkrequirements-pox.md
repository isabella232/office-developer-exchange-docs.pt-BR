---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: O elemento NetworkRequirements contém os critérios usados para determinar se o computador cliente está em uma rede que atenda aos requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor.
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462721"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

O elemento **NetworkRequirements** contém os critérios usados para determinar se o computador cliente está em uma rede que atenda aos requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="remarks"></a>Comentários

Se o cliente de email não corresponder aos requisitos de rede, ele deverá tentar outros tipos de protocolo. Os ISPs podem fornecer um conjunto de marcas de servidor com [pox (com o protocolo)](protocol-pox.md) que não exigem autenticação, mas precisam estar na rede do provedor de Internet. Os ISPs podem listar outro conjunto de servidores que exijam autenticação, mas que não precisam estar em uma rede específica. 
  
O elemento **NetworkRequirements** é opcional. 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

