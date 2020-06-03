---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: O elemento LegacyDN identifica a caixa de correio de um usuário com o nome diferenciado herdado.
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526379"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

O elemento **LegacyDN** identifica a caixa de correio de um usuário com o nome diferenciado herdado. 
  
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
|[Solicitação (POX)](request-pox.md) <br/> |Contém a solicitação para o serviço de descoberta automática.  <br/> |
|[Usuário (POX)](user-pox.md) <br/> |Fornece informações específicas do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o endereço de email herdado de um usuário.
  
## <a name="remarks"></a>Comentários

O elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é um elemento alternativo para uma solicitação de descoberta automática. Ele é usado quando uma caixa de correio existe em um computador que esteja executando o Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

