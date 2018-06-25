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
description: O elemento NetworkRequirements contém os critérios que são usados para determinar se o computador cliente está em uma rede que satisfaça os requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor.
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824529"
---
# <a name="networkrequirements-pox"></a>NetworkRequirements (POX)

O elemento **NetworkRequirements** contém os critérios que são usados para determinar se o computador cliente está em uma rede que satisfaça os requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[NetworkRequirements (POX)](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IPv4Start (POX)](ipv4start-pox.md) <br/> |Identifica o início de uma versão 4 (IPv4) do intervalo de IP endereços que são usados para identificar um computador em uma rede.  <br/> |
|[IPv4End (POX)](ipv4end-pox.md) <br/> |Identifica a fim de uma versão 4 (IPv4) do intervalo de IP endereços que são usados para identificar um computador na rede.  <br/> |
|[IPv6Start (POX)](ipv6start-pox.md) <br/> |Identifica o início de uma versão 6 (IPv6) do intervalo de IP endereços que são usados para identificar um computador em uma rede.  <br/> |
|[IPv6End (POX)](ipv6end-pox.md) <br/> |Identifica a fim de uma versão 6 (IPv6) do intervalo de IP endereços que são usados para identificar um computador em uma rede.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="remarks"></a>Comentários

Se o cliente de email não corresponder os requisitos de rede, ele deve tentar outros tipos de protocolo. Os provedores podem fornecer um conjunto de servidores com marcas de [Protocolo (POX)](protocol-pox.md) que não exigem autenticação, mas são necessários para a rede do provedor. Os provedores podem listar outro conjunto de servidores que exigem autenticação, mas não precisam estar em uma rede específica. 
  
O elemento **NetworkRequirements** é opcional. 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

