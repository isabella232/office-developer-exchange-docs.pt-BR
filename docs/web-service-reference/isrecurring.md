---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: O elemento IsRecurring indica se um item de calendário, uma solicitação de reunião ou uma tarefa é parte de um item recorrente. Este elemento é somente leitura.
ms.openlocfilehash: 72c71c1955b69f1c0df855ce4bd0ed02d4c89122
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526484"
---
# <a name="isrecurring"></a>IsRecurring

O elemento **IsRecurring** indica se um item de calendário, uma solicitação de reunião ou uma tarefa é parte de um item recorrente. Este elemento é somente leitura. 
  
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
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor booliano é necessário.
  
## <a name="remarks"></a>Comentários

A tabela a seguir mostra como a propriedade **IsRecurring** é definida para diferentes tipos de item de calendário para os organizadores e participantes e para solicitações de reunião e atualizações. 
  
|**Tipo CalendarItem**|**Organizador <br/> (IsRecurring)**|**Participante <br/> (IsRecurring)**|**Solicitação de reunião/atualização <br/> (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|Ocorrência única  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|Mestre recorrente  <br/> |**FALSE** <br/> |**VERDADEIRO** <br/> |**VERDADEIRO** <br/> |
|Exceção recorrente  <br/> |**VERDADEIRO** <br/> |**VERDADEIRO** <br/> |**VERDADEIRO** <br/> |
   
O valor da propriedade **IsRecurring** que é definido para itens de calendário mestre recorrentes para o organizador está incorreto; Esse valor deve ser definido como **true**. 
  
> [!NOTE]
> A operação GetUserAvailability também tem um elemento [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[TaskType. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType. IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType. IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

