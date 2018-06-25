---
title: DayQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayQuality
api_type:
- schema
ms.assetid: cd0eb239-6e7f-4a5a-b245-659f170550b7
description: O elemento DayQuality representa a qualidade do dia para conter os horários de reunião sugerido de qualidade.
ms.openlocfilehash: 156d5bc58d481c9c812793da4722272ac76adaad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751711"
---
# <a name="dayquality"></a>DayQuality

O elemento **DayQuality** representa a qualidade do dia para contendo qualidade sugerida horários de reuniões. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)  
- [SuggestionsResponse](suggestionsresponse.md) 
- [SuggestionDayResultArray](suggestiondayresultarray.md)  
- [SuggestionDayResult](suggestiondayresult.md) 
- [DayQuality](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

**SuggestionQuality**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SuggestionDayResult](suggestiondayresult.md) <br/> |Representa um único dia que contém os horários de reunião sugeridas.  <br/><br/>Este é a expressão XPath 2.0 para esse elemento:<br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. Estes são os valores possíveis para esse elemento:
  
- **Excelente**   
- **BOM**    
- **Justo**    
- **Baixa**
    
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

- [Operação GetUserAvailability](getuseravailability-operation.md)  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

