---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: O elemento GoodThreshold especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo seja qualificado como um bom horário de reunião sugerido.
ms.openlocfilehash: bec5159b46a350cb01f8d573c68e1925aeb40ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533217"
---
# <a name="goodthreshold"></a>GoodThreshold

O **elemento GoodThreshold** especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo seja qualificado como um bom horário de reunião sugerido. 
  
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contém as opções para obter informações de sugestão de reunião.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Os valores inteiros esperados estão entre 0 e 50.
  
## <a name="remarks"></a>Comentários

Esse elemento será necessário se o [elemento SuggestionsViewOptions](suggestionsviewoptions.md) for usado. O **elemento GoodThreshold** também determina quais reuniões são consideradas Justas. A porcentagem de participantes com conflitos é menor do que o Limite Bom e superior a 50%, o horário de reunião sugerido se qualifica como Justo. O Limite Bom mais 50 é igual à porcentagem que define o limite Good/Fair. 
  
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

