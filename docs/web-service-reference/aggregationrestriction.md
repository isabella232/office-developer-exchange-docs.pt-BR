---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: O elemento AggregationRestriction especifica um valor que é aplicado a um conjunto de propriedades persona resultante de uma solicitação FindPeople e filtra o resultado de acordo com a restrição especificada.
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463521"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

O elemento **AggregationRestriction** especifica um valor que é aplicado a um conjunto de propriedades persona resultante de uma solicitação FindPeople e filtra o resultado de acordo com a restrição especificada. 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Pesquisa](searchexpression.md)
  
### <a name="parent-elements"></a>Elementos pai

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Comentários

O elemento **AggregationRestriction** pode conter qualquer elemento filho que usa o grupo de substituição de **pesquisa** . Os elementos que fazem parte do grupo de substituição da **pesquisa** são: [Contains](contains.md), [Exclude](excludes.md), [Exists](exists.md), [not](not.md), [or](or.md), [e](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)e [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

