---
title: Padrões de recorrência e EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Saiba mais sobre os padrões de recorrência e série recorrente no Exchange.
ms.openlocfilehash: ac10e9b9a347abb5907b77f0e0e7315e4e86d97a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750954"
---
# <a name="recurrence-patterns-and-ews"></a>Padrões de recorrência e EWS

Saiba mais sobre os padrões de recorrência e série recorrente no Exchange.
  
Uma série recorrente é um compromisso ou reunião que se repete acordo com um padrão definido. Uma série recorrente pode têm um número específico de ocorrências ou pode repetir indefinidamente. Além disso, uma série recorrente pode ter exceções que não seguem o padrão do restante das ocorrências e podem ter ocorrências que foram excluídas do padrão. Você pode usar a API gerenciada de EWS e o EWS para trabalhar com a série recorrente e seus itens de calendário associado.
  
## <a name="recurring-calendar-items"></a>Itens de calendário recorrente

Todos os itens de calendário se encaixam em uma das quatro categorias a seguir:
  
- Itens de calendário não recorrentes
    
- Mestres recorrentes
    
- Ocorrências de uma série
    
- Ocorrências de modificação de uma série, conhecido como exceções
    
Neste artigo, veremos os três tipos de itens de calendário que fazem parte de uma série recorrente.
  
É útil compreender como recorrente série são implementadas no servidor Exchange. Em vez de criar um item distinto separado para cada ocorrência de uma série recorrente, o servidor cria somente um item real no calendário, conhecido como o mestre recorrente. O formato de um mestre recorrente é muito semelhante a um compromisso recorrente, com a adição de informações de padrão de recorrência. O servidor, em seguida, gera ocorrências com base no padrão de recorrência em resposta às solicitações de informações do compromisso, usando um processo chamado expansão dos clientes. Essas ocorrências geradas permanentemente não são armazenadas no servidor. Isso é importante compreender como o modo como você procurar itens de calendário determina quais informações você receber e se expansão ocorre.
  
## <a name="recurrence-patterns"></a>Padrões de recorrência

A informação-chave a uma série recorrente que possibilita a expansão é o padrão de recorrência. O padrão de recorrência for encontrado no mestre recorrente e descreve um conjunto de critérios para calcular ocorrências com base na data e hora do mestre recorrente.
  
**Tabela 1. Padrões de recorrência disponíveis**

|**Classe de API gerenciada de EWS**|**Elemento EWS**|**Exemplos**|
|:-----|:-----|:-----|
|[Recurrence.DailyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](http://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Repita a cada dia.  <br/> Repita a todos os outros dias.  <br/> |
|[Recurrence.MonthlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](http://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Repetir mensalmente no décimo dia do mês.  <br/> Repetir a cada dois meses no vigésimo primeiro dia do mês.  <br/> |
|[Recurrence.RelativeMonthlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](http://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Repita a segunda terça-feira de cada mês.  <br/> Repita o terceiro quinta-feira do mês a cada três meses.  <br/> |
|[Recurrence.RelativeYearlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](http://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Repita na primeira segunda-feira de agosto a cada ano.  <br/> |
|[Recurrence.WeeklyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](http://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Repita as segundas-feiras.  <br/> Repetir cada terça-feira e quinta-feira a cada duas semanas.  <br/> |
|[Recurrence.YearlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](http://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Repita em 1º de setembro a cada ano.  <br/> |
   
A informação importante das informações para um padrão de recorrência é quando a recorrência terminará. Isso pode ser expresso como um número definido de ocorrências, como uma data de término ou como não tendo nenhum end.
  
**Tabela 2. Opções para o final de uma série recorrente**

|**Método/propriedade da API gerenciada de EWS**|**Elemento EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Recurrence.NumberOfOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](http://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |O valor dessa propriedade ou um elemento Especifica o número de ocorrências.  <br/> |
|[Recurrence.EndDate](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](http://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |A última ocorrência na série cai em ou antes da data especificada por esta propriedade ou elemento.  <br/> |
|[Recurrence.HasEnd](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence.NeverEnds](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](http://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |A série não tiver nenhum end.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Expandida versus não expandida modos de exibição

Usando o método **FindAppointments** no EWS Managed API (ou a operação **FindItem** com um elemento de **exibição de calendário** no EWS) invoca o processo de expansão. Isso oculta os compromissos recorrentes de mestres do conjunto de resultados e, em vez disso, apresenta uma visão expandida dessa série recorrente. Ocorrências de e exceções ao mestre recorrente que ficam dentro os parâmetros do modo de exibição calendário estão incluídas no conjunto de resultados. Por outro lado, usando o método **FindItems** no EWS Managed API (ou a operação **FindItem** com um elemento **IndexedPageItemView** ou **FractionalPageItemView** no EWS), não invoca o processo de expansão e ocorrências e exceções não são incluídas. Vamos ver um exemplo comparando os dois métodos. 
  
**Tabela 3. Métodos e as operações para localizar os compromissos**

|**Método API gerenciada de EWS**|**Operação do EWS**|**Expande a série?**|**Incluído nos resultados de itens**|
|:-----|:-----|:-----|:-----|
|[ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento de [exibição de calendário](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Sim  <br/> |Compromissos não recorrentes, único ocorrências de série recorrente e exceções a série recorrente  <br/> |
|[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou um elemento de [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Não  <br/> |Compromissos não recorrentes e compromissos recorrentes de mestres  <br/> |
   
Sadie apenas assinou seu filho para esse swim equipe. A equipe tem prática toda quarta-feira às 8:30 AM, iniciando 2 de julho com o último sendo prática em 6 de agosto. Sadie não querer esquecer prática, adiciona um compromisso recorrente para o seu calendário para lembrá-lhe.
  
**Tabela 4. Compromisso recorrente de Sadie**

|**Campo de compromisso**|**Valor**|
|:-----|:-----|
|Assunto  <br/> |Nadar prática de equipe  <br/> |
|Início  <br/> |2 de julho de 2014 8:30 AM  <br/> |
|End  <br/> |2 de julho de 2014 10:00 AM  <br/> |
|Reaparecer  <br/> |Toda quarta-feira  <br/> |
|Última ocorrência  <br/> |6 de agosto de 2014 8:30 AM  <br/> |
   
Uma visão rápida de um calendário mostra que a equipe terá um total de seis práticas. No entanto, não há seis itens de compromisso distintos no calendário. Em vez disso, há apenas um compromisso mestre recorrente representando a série.
  
Agora vejamos Localizando compromissos no calendário de Sadie que ocorrem desde o mês de julho. O exemplo de código a seguir usa o método **FindItems** na API gerenciada do Exchange para produzir um modo de exibição não expandida de calendário de Sadie. 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

Se o código resultará na seguinte solicitação [FindItem operação](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

A resposta do servidor inclui apenas um único item, o mestre recorrente, indicado pelo valor do elemento de [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) da **RecurringMaster**. O valor do elemento [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Agora vamos comparar com uma exibição expandida. O exemplo de código a seguir usa o método **FindAppointments** na API gerenciada do EWS para criar uma exibição expandida de calendário de Sadie. 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

Este código resultará na seguinte solicitação [FindItem operação](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento de [exibição de calendário](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Neste momento, a resposta do servidor inclui cinco ocorrências, um para cada quarta-feira em julho. Os elementos [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) nesses itens todos têm um valor de **ocorrência**. Observe que o mestre recorrente não está presente na resposta. Os valores dos elementos [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foram diminuídos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Depois que um mestre recorrente, uma ocorrência ou uma exceção, você sempre pode [recuperar os outros itens relacionados](how-to-access-a-recurring-series-by-using-ews-in-exchange.md). Considerando uma ocorrência ou uma exceção, é possível recuperar o mestre recorrente e vice-versa.
  
## <a name="working-with-recurring-calendar-items"></a>Trabalhando com itens de calendário recorrente

Você usar todos os mesmos métodos e as operações para trabalhar com a série recorrente como você usa para trabalhar com itens de calendário não recorrentes. A diferença é que, dependendo do item que você pode usar para chamar esses métodos ou operações, as ações relacionadas a podem aplicar a série inteira ou apenas uma única ocorrência. [Ações tomadas no mestre recorrente](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) será aplicada a todas as ocorrências da série, enquanto as [ações tomadas para uma única ocorrência ou exceção](how-to-update-a-recurring-series-by-using-ews.md) será aplicada somente a essa ocorrência ou uma exceção. 
  
## <a name="in-this-section"></a>Nesta se��o

- [Acessar uma série recorrente usando o EWS no Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Criar uma série recorrente usando o EWS no Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Excluir compromissos em uma série recorrente usando o EWS no Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Atualizar uma série recorrente usando o EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Atualizar uma série recorrente usando o EWS no Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Obtenha os compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

