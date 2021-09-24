---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: O elemento ConflictingMeetingCount representa o número de reuniões que conflitam com o item de calendário.
ms.openlocfilehash: e6929160dacdf026ba8551bbcf6f991fbdc0b909
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536879"
---
# <a name="conflictingmeetingcount"></a>ConflictingMeetingCount

O **elemento ConflictingMeetingCount** representa o número de reuniões que conflitam com o item de calendário. 
  
```xml
<ConflictingMeetingCount/>
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
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um inteiro. Essa propriedade é somente leitura.
  
## <a name="remarks"></a>Comentários

Um item de calendário é considerado conflitante se ocorrer, pelo menos em parte, ao mesmo tempo que outro item de calendário na mesma pasta de calendário. Se um item de calendário estiver em uma pasta noncalendar, ele será comparado com itens de calendário na pasta de calendário padrão. As solicitações de reunião são comparadas com itens de calendário na pasta de calendário padrão.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

