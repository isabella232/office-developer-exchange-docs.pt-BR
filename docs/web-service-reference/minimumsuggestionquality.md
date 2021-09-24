---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: O elemento MinimumSuggestionQuality define a qualidade das sugestões de reunião a serem retornadas na resposta.
ms.openlocfilehash: c1126158f7a521fbefaf34fda906d60dd15c2af4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510929"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

O **elemento MinimumSuggestionQuality** define a qualidade das sugestões de reunião a serem retornadas na resposta. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contém as opções para obter informações de sugestão de reunião.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. A tabela a seguir lista os valores possíveis para este elemento:
  
|**Valor**|**Descrição**|
|:-----|:-----|
|**Excelente** <br/> |0% dos participantes têm um conflito com o horário de reunião sugerido.  <br/> |
|**Good** <br/> |A porcentagem considerada boa é definida usando o [elemento GoodThreshold.](goodthreshold.md)  <br/> |
|**Fair** <br/> |A porcentagem considerada justa é definida usando o [elemento GoodThreshold.](goodthreshold.md)  <br/> |
|**Ruim** <br/> |50% ou mais dos participantes têm um conflito com o horário de reunião sugerido.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento será necessário se o [elemento SuggestionsViewOptions](suggestionsviewoptions.md) for usado. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

