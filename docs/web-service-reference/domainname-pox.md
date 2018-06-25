---
title: DomainName POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: O elemento DomainName Especifica o domínio do usuário.
ms.openlocfilehash: c38d2e470bd174ab6dd7e5e1dd3eee23daea5e69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751918"
---
# <a name="domainname-pox"></a>DomainName POX)

O elemento **DomainName** Especifica o domínio do usuário. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)  
- [Resposta POX)](response-pox.md)  
- [Conta (POX)](account-pox.md) 
- [Protocolo (POX)](protocol-pox.md) 
- [DomainName POX)](domainname-pox.md)
  
```xml
<DomainName/>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto Especifica o domínio do usuário.
  
## <a name="remarks"></a>Comentários

Se nenhum valor for especificado, a autenticação padrão é usar o endereço de email como um formato de nome principal (UPN) do usuário. Por exemplo: \<Username\>@\<domínio\>.
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

