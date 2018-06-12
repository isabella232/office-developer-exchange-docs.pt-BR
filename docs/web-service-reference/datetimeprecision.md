---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: O elemento DateTimePrecision Especifica a precisão para valores de data/hora retornado.
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751686"
---
# <a name="datetimeprecision"></a>DateTimePrecision

O elemento **DateTimePrecision** Especifica a precisão para valores de data/hora retornado. 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

O elemento **DateTimePrecision** está localizado no cabeçalho SOAP. 
  
## <a name="text-value"></a>Text value

É necessário um valor de texto. Veja a seguir os valores possíveis:
  
- Segundos
    
- Milissegundos
    
## <a name="remarks"></a>Coment�rios

Data/hora de quando um cabeçalho SOAP com o elemento **DateTimePrecision** definido como "Segundos" é usado, os valores são retornados para os mais próximo segundos (00: 00:00). Data/hora de quando "Milissegundos" são usados, os valores são retornados para o milissegundo mais próximo (00:00:00.0000). 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

