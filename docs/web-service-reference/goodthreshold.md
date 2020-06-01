---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: O elemento GoodThreshold especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo se qualifique como um bom horário de reunião.
ms.openlocfilehash: 34ea433ad7315d61df8cf8e22bae1166d3210af3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457309"
---
# <a name="goodthreshold"></a>GoodThreshold

O elemento **GoodThreshold** especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo se qualifique como um bom horário de reunião. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[GoodThreshold](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contém as opções para obter informações de sugestão de reunião.  <br/> Este é o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Os valores inteiros esperados estão entre 0 e 50.
  
## <a name="remarks"></a>Comentários

Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) for usado. O elemento **GoodThreshold** também determina quais reuniões são consideradas justas. A porcentagem de participantes com conflitos é menor do que o limite bom e maior que 50%, o tempo de reunião sugerido é qualificado como justo. O bom limite mais 50 equivale à porcentagem que define o limite bom/justo. 
  
> [!NOTE]
> O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserAvailability](getuseravailability-operation.md)


[Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

