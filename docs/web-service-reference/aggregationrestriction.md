---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: O elemento AggregationRestriction Especifica um valor que é aplicado a um conjunto de propriedades de pessoa resultante de uma solicitação de FindPeople e filtra o resultado de acordo com a restrição especificada.
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751077"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

O elemento **AggregationRestriction** Especifica um valor que é aplicado a um conjunto de propriedades de pessoa resultante de uma solicitação de FindPeople e filtra o resultado de acordo com a restrição especificada. 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>Elementos pai

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Comentários

O elemento **AggregationRestriction** pode conter qualquer elemento filho que usa o grupo de substituição de **SearchExpression** . Os elementos que fazem parte do grupo de substituição **SearchExpression** são: [contém](contains.md), [exclusões](excludes.md), [Exists](exists.md), [não](not.md), [ou](or.md) [e](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan ](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)e [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

