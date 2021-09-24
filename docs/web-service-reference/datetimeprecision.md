---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: O elemento DateTimePrecision especifica a precisão dos valores de data/hora retornados.
ms.openlocfilehash: 075e37bfdd2c61f56352e000ef6cc5810dd81bbb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535707"
---
# <a name="datetimeprecision"></a>DateTimePrecision

O **elemento DateTimePrecision** especifica a precisão dos valores de data/hora retornados. 
  
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

O **elemento DateTimePrecision** está localizado no header SOAP. 
  
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Veja a seguir os valores possíveis:
  
- Segundos
    
- Milissegundos
    
## <a name="remarks"></a>Comentários

Quando um header SOAP com o **elemento DateTimePrecision** definido como "Seconds" é usado, os valores de data/hora são retornados para os segundos mais próximos (00:00:00). Quando "Milissegundos" é usado, os valores de data/hora são retornados para o milissegundo mais próximo (00:00:00.0000). 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

