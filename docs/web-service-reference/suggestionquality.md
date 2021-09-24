---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: O elemento SuggestionQuality representa a qualidade do tempo de reunião sugerido.
ms.openlocfilehash: 4d8a504e60e8f043bfb120080a89733e78b16b9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531549"
---
# <a name="suggestionquality"></a>SuggestionQuality

O **elemento SuggestionQuality** representa a qualidade do tempo de reunião sugerido. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[Sugestão](suggestion.md)
  
[SuggestionQuality](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 **SuggestionQuality**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Sugestão](suggestion.md) <br/> |Representa uma única sugestão de hora de reunião.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um **valor SuggestionQuality** é necessário. Veja a seguir os valores possíveis: 
  
- **Excelentes** 100% dos usuários e recursos estão disponíveis para o horário de reunião sugerido. 
    
- **Bom** A porcentagem mínima de usuários e recursos disponíveis é igual ou maior que o valor do [elemento GoodThreshold](goodthreshold.md) mais 50. 
    
- **Fair** A porcentagem máxima de usuários e recursos disponíveis para um tempo de reunião sugerido é igual ao valor do [elemento GoodThreshold](goodthreshold.md) mais 50. O valor mínimo para um **tempo de** reunião de qualidade justo é 50%. 
    
- **Ruim** Menos de 50% dos usuários e recursos estão disponíveis para o horário de reunião sugerido. 
    
## <a name="remarks"></a>Comentários

O **tipo SuggestionQuality** também é o tipo para os elementos [DayQuality](dayquality.md) e [MinimumSuggestionQuality.](minimumsuggestionquality.md) 
  
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

