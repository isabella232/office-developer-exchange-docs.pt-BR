---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: O elemento de MinimumSuggestionQuality define a qualidade das sugestões de reunião a serem retornados na resposta.
ms.openlocfilehash: ac79682bd761f678f23fc2d698a50fd7704f6fab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824468"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

O elemento de **MinimumSuggestionQuality** define a qualidade das sugestões de reunião a serem retornados na resposta. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contém as opções para a obtenção de informações de sugestão de reunião.  <br/> Este é o XPath a este elemento:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. A tabela a seguir lista os valores possíveis para esse elemento:
  
|**Valor**|**Descrição**|
|:-----|:-----|
|**Excelente** <br/> |0% dos participantes têm um conflito com o tempo de reunião sugeridas.  <br/> |
|**BOM** <br/> |A porcentagem é considerada boa for definida usando o elemento [GoodThreshold](goodthreshold.md) .  <br/> |
|**Justo** <br/> |A porcentagem que é considerada justa for definida usando o elemento [GoodThreshold](goodthreshold.md) .  <br/> |
|**Baixa** <br/> |50% ou mais dos participantes têm um conflito com o tempo de reunião sugeridas.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obtenção de disponibilidade do usuário](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

