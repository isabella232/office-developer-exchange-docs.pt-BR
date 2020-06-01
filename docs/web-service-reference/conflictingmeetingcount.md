---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: O elemento ConflictingMeetingCount representa o número de reuniões que entram em conflito com o item do calendário.
ms.openlocfilehash: d53245e1b5d1f0182b28b15bf55ba9742bbb2a07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463857"
---
# <a name="conflictingmeetingcount"></a>ConflictingMeetingCount

O elemento **ConflictingMeetingCount** representa o número de reuniões que entram em conflito com o item do calendário. 
  
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
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um inteiro. Essa propriedade é somente leitura.
  
## <a name="remarks"></a>Comentários

Um item de calendário é considerado conflitante se ocorrer, pelo menos em parte, ao mesmo tempo que outro item de calendário na mesma pasta do calendário. Se um item de calendário estiver em uma pasta que não seja de calendário, ele será comparado com os itens de calendário na pasta de calendário padrão. As solicitações de reunião são comparadas com os itens de calendário na pasta padrão calendário.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

