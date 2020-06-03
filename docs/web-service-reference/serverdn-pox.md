---
title: ServerDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: O elemento ServerDN especifica o nome distinto do computador que está executando o Microsoft Exchange Server 2007.
ms.openlocfilehash: 16c6e7368e221b7e54c8d7d63532bb29464a7e54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461993"
---
# <a name="serverdn-pox"></a>ServerDN (POX)

O elemento **ServerDN** especifica o nome distinto do computador que está executando o Microsoft Exchange Server 2007. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[ServerDN (POX)](serverdn-pox.md)
  
```xml
<ServerDN/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o nome distinto do servidor Exchange.
  
## <a name="remarks"></a>Comentários

O valor **ServerDN** é usado somente quando o [tipo (POX)](type-pox.md) é igual a Exch. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

