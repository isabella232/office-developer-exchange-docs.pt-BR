---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: O elemento DateTimePrecision especifica a precisão dos valores de data/hora retornados.
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529221"
---
# <a name="datetimeprecision"></a>DateTimePrecision

O elemento **DateTimePrecision** especifica a precisão dos valores de data/hora retornados. 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

O elemento **DateTimePrecision** está localizado no cabeçalho SOAP. 
  
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Veja a seguir os valores possíveis:
  
- Segundos
    
- Milissegundos
    
## <a name="remarks"></a>Comentários

Quando um cabeçalho SOAP com o elemento **DateTimePrecision** definido como "segundos" é usado, os valores de data/hora são retornados para os segundos mais próximos (00:00:00). Quando "milissegundos" é usado, os valores de data/hora são retornados para o milissegundo mais próximo (00:00:00.0000). 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

