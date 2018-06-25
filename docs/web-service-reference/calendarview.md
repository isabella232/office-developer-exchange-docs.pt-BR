---
title: Exibição de calendário
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: O elemento CalendarView define uma operação FindItem como retornar itens de calendário em um conjunto que aparecem em um calendário.
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751369"
---
# <a name="calendarview"></a>Exibição de calendário

O elemento **CalendarView** define uma [operação FindItem](finditem-operation.md) como retornar itens de calendário em um conjunto que aparecem em um calendário. 
  
[FindItem](finditem.md)
  
[Exibição de calendário](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**Exibição de calendário**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de resultados a serem retornados na resposta FindItem.  <br/> |
|**StartDate** <br/> |Identifica o início de um período de tempo consultado para itens de calendário. Todos os itens de calendário que têm uma hora de término que seja antes **StartDate** não serão retornados. O valor da **StartDate** pode ser especificado no formato tempo universal coordenado (UTC), como de 2006-01-02T12:00:00Z, ou em um formato que o deslocamento de hora local e fuso horário estiver especificado, como 2006-01-02T04:00:00-08:00.  <br/><br/>Este atributo é necessário.  <br/> |
|**EndDate** <br/> |Identifica o final de um período de tempo consultado para itens de calendário. Todos os itens de calendário que têm uma hora de início em ou após **EndDate** não serão retornados. O valor da **EndDate** pode ser especificado no formato UTC, como de 2006-02-02T12:00:00Z, ou em um formato que o deslocamento de hora local e fuso horário estiver especificado, como 2006-02-02T04:00:00-08:00.  <br/><br/>**EndDate** deve ser maior ou igual a **StartDate**; Caso contrário, um erro será retornado. Este atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.<br/><br/> Este é a expressão XPath para esse elemento:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

Se o elemento de **exibição de calendário** for especificado em uma solicitação de FindItem, o serviço Web retorna uma lista de itens de calendário único e ocorrências de itens de calendário recorrentes dentro do intervalo especificado pelo **StartDate** e **EndDate**.
  
Se o elemento de **exibição de calendário** não for especificado em uma solicitação de FindItem, o serviço Web retorna uma lista de itens de calendário único e itens de calendário mestre recorrente. Ocorrências de calendário de um item de calendário recorrente não são expandidas. 
  
Consultas CalendarView só devem fazer use das propriedades a seguir, desde que eles oferecem suporte a consultas de calendário mais rápidas.
  
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
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Calculado a partir do blob de recorrência principal ou do mestre
  
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
  
- EntryId
    
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

O exemplo a seguir mostra uma solicitação FindItem. Uma solicitação bem-sucedida retornará uma resposta que inclui itens de calendário iniciados de 2006-05-18T00:00:00-08:00 ou depois e finalizada antes de 2006-05-19T00:00:00-08:00.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação FindItem](finditem-operation.md)
- [Localizando itens](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

