---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: O elemento DayOfWeekIndex descreve qual semana em um mês é usada em um padrão de recorrência relativa.
ms.openlocfilehash: 3b9af396bbd5c51b365da6a95b40b00718d47c3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542516"
---
# <a name="dayofweekindex"></a>DayOfWeekIndex

O **elemento DayOfWeekIndex** descreve qual semana em um mês é usada em um padrão de recorrência relativa. 
  
```xml
<DayOfWeekIndex/>
```

**DayOfWeekIndexType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão de recorrência anual relativo.  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |Descreve um padrão de recorrência mensal relativo.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Veja a seguir os valores possíveis:
  
- Primeiro    
- Segundo    
- Terceira    
- Quarto    
- Último
    
## <a name="remarks"></a>Comentários

Por exemplo, a segunda segunda segunda-feira de um mês pode ocorrer na terceira semana desse mês. Se um mês começar em uma sexta-feira, a primeira semana do mês conterá apenas alguns dias e não conterá uma segunda-feira. Portanto, a primeira segunda-feira teria que ocorrer na segunda semana.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

