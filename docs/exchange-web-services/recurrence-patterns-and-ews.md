---
title: Padrões de recorrência e EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Saiba mais sobre padrões de recorrência e séries recorrentes no Exchange.
ms.openlocfilehash: 681dfee7e0a66a483b8638810da5e4e0ac0f05ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459325"
---
# <a name="recurrence-patterns-and-ews"></a>Padrões de recorrência e EWS

Saiba mais sobre padrões de recorrência e séries recorrentes no Exchange.
  
Uma série recorrente é um compromisso ou uma reunião que se repete de acordo com um padrão definido. Uma série recorrente pode ter um número específico de ocorrências ou pode ser repetida indefinidamente. Além disso, uma série recorrente pode ter exceções que não seguem o padrão do restante das ocorrências e podem ter ocorrências que foram excluídas do padrão. Você pode usar a API gerenciada do EWS e o EWS para trabalhar com séries recorrentes e seus itens de calendário associados.
  
## <a name="recurring-calendar-items"></a>Itens de calendário recorrentes

Todos os itens de calendário se enquadram em uma das quatro categorias a seguir:
  
- Itens de calendário não recorrentes
    
- Mestres recorrentes
    
- Ocorrências em uma série
    
- Ocorrências modificadas em uma série, conhecidas como exceções
    
Neste artigo, examinaremos os três tipos de itens de calendário que fazem parte de uma série recorrente.
  
É útil entender como as séries recorrentes são implementadas no servidor Exchange. Em vez de criar um item distinto separado para cada ocorrência em uma série recorrente, o servidor cria apenas um item real no calendário, conhecido como mestre recorrente. O formato de um mestre recorrente é muito semelhante a um compromisso não recorrente, com a adição de informações de padrão de recorrência. Em seguida, o servidor gera ocorrências com base no padrão de recorrência em resposta às solicitações de cliente para informações de compromisso, usando um processo chamado expansão. Essas ocorrências geradas não são permanentemente armazenadas no servidor. Isso é importante entender, pois a forma como você pesquisa os itens de calendário determina quais informações você recebe e se a expansão ocorre.
  
## <a name="recurrence-patterns"></a>Padrões de recorrência

A parte principal de uma série recorrente que torna a expansão possível é o padrão de recorrência. O padrão de recorrência é encontrado no mestre recorrente e descreve um conjunto de critérios para calcular as ocorrências com base na data e hora do mestre recorrente.
  
**Tabela 1. Padrões de recorrência disponíveis**

|**Classe de API gerenciada do EWS**|**Elemento do EWS**|**Exemplos**|
|:-----|:-----|:-----|
|[Recurrence. DailyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Repetir todos os dias.  <br/> Repetir a cada dia.  <br/> |
|[Recurrence. MonthlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Repetir a cada mês no décimo dia do mês.  <br/> Repetir a cada mês no primeiro dia do mês.  <br/> |
|[Recurrence. RelativeMonthlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Repita a segunda terça-feira de cada mês.  <br/> Repita a terceira quinta-feira do mês a cada três meses.  <br/> |
|[Recurrence. RelativeYearlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Repita na primeira segunda-feira de agosto a cada ano.  <br/> |
|[Recurrence. WeeklyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Repetir a cada segunda-feira.  <br/> Repita todas as terças e quinta-feira a cada semana.  <br/> |
|[Recurrence. YearlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Repita no dia 1º de setembro a cada ano.  <br/> |
   
A outra informação importante para um padrão de recorrência é quando a recorrência termina. Isso pode ser expresso como um número definido de ocorrências, como uma data final ou como sem final.
  
**Tabela 2. Opções para o final de uma série recorrente**

|**Método/propriedade da API gerenciada do EWS**|**Elemento do EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Recurrence. NumberOfOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |O valor dessa propriedade ou elemento Especifica o número de ocorrências.  <br/> |
|[Recurrence. EndDate](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |A última ocorrência na série cai ou antes da data especificada por essa propriedade ou elemento.  <br/> |
|[Recurrence. HasEnd](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence. NeverEnds](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |A série não tem fim.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Exibições expandidas vs. não expandidas

O uso do método **FindAppointments** na API gerenciada do EWS (ou na operação **FindItem** com um elemento **CalendarView** no EWS) invoca o processo de expansão. Isso oculta compromissos mestre recorrentes do conjunto de resultados e, em vez disso, apresenta uma visão expandida dessa série recorrente. As ocorrências de e exceções para o mestre recorrente que estão dentro dos parâmetros do modo de exibição de calendário são incluídas no conjunto de resultados. Por outro lado, usar o método **FindItems** na API gerenciada do EWS (ou na operação **FindItem** com um elemento **IndexedPageItemView** ou **FractionalPageItemView** no EWS), não invoca o processo de expansão, e as ocorrências e exceções não estão incluídas. Vejamos um exemplo que compara os dois métodos. 
  
**Tabela 3. Métodos e operações para localizar compromissos**

|**Método de API gerenciada do EWS**|**Operação do EWS**|**Expande a série?**|**Itens incluídos nos resultados**|
|:-----|:-----|:-----|:-----|
|[ExchangeService. FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Sim  <br/> |Compromissos não recorrentes, ocorrências únicas de séries recorrentes e exceções à série recorrente  <br/> |
|[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou um elemento [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Não  <br/> |Compromissos não recorrentes e compromissos mestre recorrentes  <br/> |
   
Sadie acabou de assinar seu filho para a equipe de nada. A equipe tem a prática toda quarta-feira de manhã às 8:30 AM, a partir de 2 de julho, com a última sessão em 6 de agosto. Não quer esquecer da prática, o Sadie adiciona um compromisso recorrente ao seu calendário para lembrá-lo.
  
**Tabela 4. Compromisso recorrente do Sadie**

|**Campo de compromisso**|**Valor**|
|:-----|:-----|
|Assunto  <br/> |Prática de equipe de nada  <br/> |
|Início  <br/> |2 de julho de 2014 8:30 AM  <br/> |
|Final  <br/> |2 de julho de 2014 10:00 AM  <br/> |
|Reaparecer  <br/> |Toda quarta-feira  <br/> |
|Última ocorrência  <br/> |6 de agosto de 2014 8:30 AM  <br/> |
   
Uma visão rápida de um calendário mostra que a equipe terá um total de seis práticas. No entanto, não há seis itens de compromisso distintos no calendário. Em vez disso, há apenas um compromisso mestre recorrente que representa a série.
  
Agora, vamos examinar a localização de compromissos no calendário do Sadie que ocorrem no mês de julho. O exemplo de código a seguir usa o método **FindItems** na API gerenciada do Exchange para produzir uma visão não expandida do calendário de Sadie. 
  
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

Esse código resulta na seguinte solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

A resposta do servidor inclui apenas um único item, o mestre recorrente, indicado pelo valor do elemento [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) de **RecurringMaster**. O valor do elemento [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Agora, vamos comparar com um modo de exibição expandido. O exemplo de código a seguir usa o método **FindAppointments** na API gerenciada do EWS para criar uma exibição expandida do calendário de Sadie. 
  
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

Esse código resulta na seguinte solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Desta vez, a resposta do servidor inclui cinco ocorrências, uma para cada quarta-feira em julho. Os elementos [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) desses itens têm um valor de **ocorrência**. Observe que o mestre recorrente não está presente na resposta. Os valores dos elementos [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foram reduzidos para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Após ter um mestre recorrente, uma ocorrência ou uma exceção, você sempre poderá [recuperar os outros itens relacionados](how-to-access-a-recurring-series-by-using-ews-in-exchange.md). Devido a uma ocorrência ou exceção, você pode recuperar o mestre recorrente e vice-versa.
  
## <a name="working-with-recurring-calendar-items"></a>Trabalhar com itens de calendário recorrentes

Você usa todos os mesmos métodos e operações para trabalhar com a série recorrente ao usar o para trabalhar com itens de calendário não recorrentes. A diferença é que, dependendo do item que você usa para invocar esses métodos ou operações, as ações que você executa podem ser aplicadas à série inteira ou apenas a uma única ocorrência. [As ações realizadas no mestre recorrente](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) se aplicarão a todas as ocorrências da série, enquanto as [ações realizadas para uma única ocorrência ou exceção](how-to-update-a-recurring-series-by-using-ews.md) só serão aplicadas a essa ocorrência ou exceção. 
  
## <a name="in-this-section"></a>Nesta seção

- [Acessar uma série recorrente usando o EWS no Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Criar uma série recorrente usando o EWS no Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Excluir compromissos em uma série recorrente usando o EWS no Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Atualizar uma série recorrente usando o EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Atualizar uma série recorrente usando o EWS no Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

