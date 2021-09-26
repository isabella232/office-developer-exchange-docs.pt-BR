---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: O elemento AggregationRestriction especifica um valor que é aplicado a um conjunto de propriedades Persona resultantes de uma solicitação FindPeople e filtra o resultado de acordo com a restrição especificada.
ms.openlocfilehash: 6a00035f87e0f365f4551df1a6ff570e01761770
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546788"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

O **elemento AggregationRestriction** especifica um valor que é aplicado a um conjunto de propriedades Persona resultantes de uma solicitação FindPeople e filtra o resultado de acordo com a restrição especificada. 
  
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

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>Elementos pai

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Comentários

O **elemento AggregationRestriction** pode conter qualquer elemento filho que use o grupo de **substituição SearchExpression.** Os elementos que fazem parte do grupo de substituição **SearchExpression** são: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md) [,](or.md)Or , [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)e [IsLessThanOrEqualTo](islessthanorequalto.md).
  
Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

