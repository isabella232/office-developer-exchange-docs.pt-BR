---
title: SuggestionDayResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionDayResult
api_type:
- schema
ms.assetid: 916b1cbb-f2e3-471d-84b0-e33467616652
description: O elemento SuggestionDayResult representa um único dia que contém os horários de reunião sugeridos.
ms.openlocfilehash: fb24a8ce27b1f21448acc70a6c9b11927c77b8cc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543958"
---
# <a name="suggestiondayresult"></a>SuggestionDayResult

O **elemento SuggestionDayResult** representa um único dia que contém os horários de reunião sugeridos. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 **SuggestionDayResult**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Date](date.md) <br/> |Representa a data que contém os horários de reunião sugeridos.  <br/> |
|[DayQuality](dayquality.md) <br/> |Representa a qualidade do dia para conter os horários de reunião sugeridos de qualidade.  <br/> |
|[SuggestionArray](suggestionarray.md) <br/> |Contém uma matriz de sugestões de reunião.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SuggestionDayResultArray](suggestiondayresultarray.md) <br/> |Contém uma matriz de sugestões de reunião organizadas por data.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

