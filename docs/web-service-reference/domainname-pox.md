---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: O elemento DomainName especifica o domínio do usuário.
ms.openlocfilehash: 9242c867d684bf9803f8c6ed1082d578cca05505
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526430"
---
# <a name="domainname-pox"></a>DomainName (POX)

O **elemento DomainName** especifica o domínio do usuário. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md)  
- [Account (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [DomainName (POX)](domainname-pox.md)
  
```xml
<DomainName/>
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

O valor de texto especifica o domínio do usuário.
  
## <a name="remarks"></a>Comentários

Se nenhum valor for especificado, a autenticação padrão será usar o endereço de email como um formato UPN (nome principal do usuário). Por exemplo: \<Username\> @ \<Domain\> .
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

