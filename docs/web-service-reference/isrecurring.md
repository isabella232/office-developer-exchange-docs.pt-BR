---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: O elemento IsRecurring indica se um item de calendário, solicitação de reunião ou tarefa faz parte de um item recorrente. Esse elemento é somente leitura.
ms.openlocfilehash: ea910b78e962906285a73c869e394147c324372c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532723"
---
# <a name="isrecurring"></a>IsRecurring

O **elemento IsRecurring** indica se um item de calendário, solicitação de reunião ou tarefa faz parte de um item recorrente. Esse elemento é somente leitura. 
  
```xml
<IsRecurring/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor Boolean é necessário.
  
## <a name="remarks"></a>Comentários

A tabela a seguir mostra como a **propriedade IsRecurring** é definida para diferentes tipos de item de calendário para organizadores e participantes e para solicitações de reunião e atualizações. 
  
|**Tipo CalendarItem**|**Organizer  <br/> (IsRecurring)**|**Participante  <br/> (IsRecurring)**|**Solicitação/atualização de  <br/> reunião (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|Ocorrência única  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|Mestre Recorrente  <br/> |**FALSE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
|Exceção Recorrente  <br/> |**TRUE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
   
O **valor da propriedade IsRecurring** definido para itens de calendário mestre recorrentes para o organizador está incorreto; esse valor deve ser definido como **VERDADEIRO**. 
  
> [!NOTE]
> A operação GetUserAvailability também tem um [elemento IsRecurring (CalendarEventDetails).](isrecurring-calendareventdetails.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[TaskType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

