---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: O elemento CalendarView define uma operação FindItem como retornando itens de calendário em um conjunto conforme aparecem em um calendário.
ms.openlocfilehash: 5e0180bb5e8a6d9fcbe42380abbe32820117ae29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518824"
---
# <a name="calendarview"></a>CalendarView

O **elemento CalendarView** define uma [operação FindItem](finditem-operation.md) como retornando itens de calendário em um conjunto conforme aparecem em um calendário. 
  
[FindItem](finditem.md)
  
[Modo de exibição do Calendário](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**Modo de exibição do Calendário**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de resultados a retornar na resposta FindItem.  <br/> |
|**StartDate** <br/> |Identifica o início de um intervalo de tempo consultado para itens de calendário. Todos os itens de calendário que tenham uma hora de término antes **de StartDate** não serão retornados. O valor de **StartDate** pode ser especificado no formato UTC (tempo universal coordenado), como em 2006-01-02T12:00:00Z, ou em um formato em que o deslocamento de hora e fuso horário local é especificado, como em 2006-01-02T04:00:00-08:00.  <br/><br/>Esse atributo é necessário.  <br/> |
|**EndDate** <br/> |Identifica o fim de um intervalo de tempo consultado para itens de calendário. Todos os itens de calendário que tenham uma hora de início que está em **ou após EndDate** não serão retornados. O valor de **EndDate** pode ser especificado no formato UTC, como em 2006-02-02T12:00:00Z, ou em um formato em que o deslocamento de fuso horário e hora local é especificado, como em 2006-02-02T04:00:00-08:00.  <br/><br/>**EndDate** deve ser maior ou igual a **StartDate;** caso contrário, um erro é retornado. Esse atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar itens em uma caixa de correio.<br/><br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

Se o **elemento CalendarView** for especificado em uma solicitação FindItem, o serviço Web retornará uma lista de itens de calendário único e ocorrências de itens de calendário recorrentes dentro do intervalo especificado por **StartDate** e **EndDate**.
  
Se o **elemento CalendarView** não for especificado em uma solicitação FindItem, o serviço Web retornará uma lista de itens de calendário único e itens de calendário mestre recorrentes. As ocorrências de calendário de um item de calendário recorrente não são expandidas. 
  
As consultas CalendarView só devem usar as seguintes propriedades, pois elas suportam consultas de calendário mais rápidas.
  
### <a name="recurrence-blob-properties"></a>Propriedades de blob de recorrência
  
- MapiStartTime
    
- MapiEndTime
    
- SubjectPrefixInternal
    
- NormalizedSubjectInternal
    
- MapiSubject
    
- Local
    
- AppointmentColor
    
- MapiIsAllDayEvent
    
- MapiHasAttachment
    
- FreeBusyStatus
    
- ReminderIsSetInternal
    
- ReminderMinutesBeforeStartInternal
    
- AppointmentState
    
- AllAttachmentsHidden
    
- ChangeHighlight
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Calculado a partir do blob ou mestre de recorrência principal
  
- ItemId
    
- IsRecurring
    
- IsException
    
- AppointmentRecurring
    
- MapiStartTime
    
- MapiPRStartDate
    
- MapiEndTime
    
- MapiPREndDate
    
- CalendarItemType
    
- GlobalObjectId
    
- TimeZoneDefinitionStart
    
- TimeZoneDefinitionEnd
    
### <a name="master-calendar-item-properties"></a>Propriedades de item de calendário mestre
  
- Entryid
    
- ChangeKey
    
- ItemClass
    
- SentRepresentingEmailAddress
    
- SentRepresentingDisplayName
    
- SentRepresentingEntryId
    
- AppointmentRecurrenceBlob
    
- TimeZone
    
- TimeZoneBlob
    
- TimeZoneDefinitionRecurring
    
- CleanGlobalObjectId
    
- AppointmentRecurring
    
- IsException
    
- IsRecurring
    
- MapiSensitivity
    
- ContainerClass
    
- MapiPRStartDate
    
- MapiPREndDate
    
- Categories
    
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma solicitação FindItem. Uma solicitação bem-sucedida retorna uma resposta que inclui itens de calendário iniciados em 2006-05-18T00:00:00-08:00 ou depois e encerrados antes de 2006-05-19T00:00:00-08:00.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindItem](finditem-operation.md)
- [Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

