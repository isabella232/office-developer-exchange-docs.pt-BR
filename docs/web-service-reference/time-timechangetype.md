---
title: Tempo (TimeChangeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: be12e41e-6871-4f6b-b2d4-3dfa404f9ea1
description: O elemento de tempo descreve a hora de quando o tempo é alterado entre o período padrão e o horário de verão.
ms.openlocfilehash: db44ef494561b75dc55c93229cec3901f04235ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837717"
---
# <a name="time-timechangetype"></a>Tempo (TimeChangeType)

O elemento de **tempo** descreve a hora de quando o tempo é alterado entre o período padrão e o horário de verão. 
  
```xml
<Time/>
```

 **Time**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Horário de verão](daylight.md) <br/> |Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.  <br/> |
|[Standard](standard.md) <br/> |Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a hora quando o tempo é alterado entre o período padrão e o horário de verão.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

