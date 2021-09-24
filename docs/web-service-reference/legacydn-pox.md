---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: O elemento LegacyDN identifica a caixa de correio de um usuário por nome diferenciado herdado.
ms.openlocfilehash: bd65e18daf1b05f66ebd767635cbe6a3135f1abf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540829"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

O **elemento LegacyDN** identifica a caixa de correio de um usuário por nome diferenciado herdado. 
  
```xml
<LegacyDN/>
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
|[Request (POX)](request-pox.md) <br/> |Contém a solicitação para o serviço descoberta automática.  <br/> |
|[User (POX)](user-pox.md) <br/> |Fornece informações específicas do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o endereço de email herddo de um usuário.
  
## <a name="remarks"></a>Comentários

O [elemento EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é um elemento alternativo para uma solicitação de Descoberta Automática. Ela é usada quando uma caixa de correio existe em um computador que está executando Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

