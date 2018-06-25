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
description: O elemento LegacyDN identifica a caixa de correio de um usuário por nome distinto herdado.
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824243"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

O elemento **LegacyDN** identifica a caixa de correio de um usuário por nome distinto herdado. 
  
```xml
<LegacyDN/>
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
|[Solicitação (POX)](request-pox.md) <br/> |Contém a solicitação para o serviço Descoberta automática.  <br/> |
|[Usuário (POX)](user-pox.md) <br/> |Fornece informações específicas do usuário.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o endereço de email legados de um usuário.
  
## <a name="remarks"></a>Comentários

O [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é um elemento alternativo para uma solicitação de descoberta automática. Ele é usado quando não existe uma caixa de correio em um computador que está executando o Microsoft Exchange Server 2007. 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

