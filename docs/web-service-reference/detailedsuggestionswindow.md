---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: O elemento DetailedSuggestionsWindow identifica o período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.
ms.openlocfilehash: 56f66d9ee7be25de20a892823a02174c75b40601
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545332"
---
# <a name="detailedsuggestionswindow"></a>DetailedSuggestionsWindow

O **elemento DetailedSuggestionsWindow** identifica o período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md) 
- [SuggestionsViewOptions](suggestionsviewoptions.md) 
- [DetailedSuggestionsWindow](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 **Duration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Representa o início do período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.  <br/> |
|[EndTime](endtime.md) <br/> |Representa o fim do período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contém as opções para obter informações de sugestão de reunião.  <br/> Veja a seguir o XPath para este elemento:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento não é necessário.
  
> [!NOTE]
> O esquema que descreve esse elemento está localizado no diretório /EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserAvailability](getuseravailability-operation.md)
- [Obter Disponibilidade do Usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

