---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: O elemento DomainRequired indica se o domínio é necessário para autenticação.
ms.openlocfilehash: 906c99ff7a8428404ee6045b749cdb0afed882b7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540059"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

O **elemento DomainRequired** indica se o domínio é necessário para autenticação. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md) 
- [Account (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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

O valor de texto indica se o domínio é necessário para autenticação. Os valores possíveis **estão on** e **off**. Se o valor estiver **em**, a solicitação subsequente deverá conter o domínio da conta do usuário.
  
## <a name="remarks"></a>Comentários

Se o domínio não for especificado no [elemento LoginName (POX)](loginname-pox.md) ou o **elemento LoginName** não tiver sido especificado, o usuário deverá inserir o domínio antes que a autenticação seja bem-sucedida. 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

