---
title: Padrões de recorrência e EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Saiba mais sobre padrões de recorrência e séries recorrentes em Exchange.
ms.openlocfilehash: fcd6cf847efedd3bc48a26ad7866a0221de59371
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541585"
---
# <a name="recurrence-patterns-and-ews"></a>Padrões de recorrência e EWS

Saiba mais sobre padrões de recorrência e séries recorrentes em Exchange.
  
Uma série recorrente é um compromisso ou reunião que se repete de acordo com um padrão definido. Uma série recorrente pode ter um número específico de ocorrências ou pode se repetir indefinidamente. Além disso, uma série recorrente pode ter exceções que não seguem o padrão do restante das ocorrências e podem ter ocorrências que foram excluídas do padrão. Você pode usar a API Gerenciada EWS e o EWS para trabalhar com séries recorrentes e seus itens de calendário associados.
  
## <a name="recurring-calendar-items"></a>Itens de calendário recorrentes

Todos os itens de calendário se enquadram em uma das quatro categorias a seguir:
  
- Itens de calendário não recorrentes
    
- Mestres recorrentes
    
- Ocorrências em uma série
    
- Ocorrências modificadas em uma série, conhecidas como exceções
    
Neste artigo, vamos ver os três tipos de itens de calendário que fazem parte de uma série recorrente.
  
É útil entender como as séries recorrentes são implementadas no Exchange servidor. Em vez de criar um item distinto separado para cada ocorrência em uma série recorrente, o servidor cria apenas um item real no calendário, conhecido como o mestre recorrente. O formato de um mestre recorrente é muito semelhante a um compromisso não recorrente, com a adição de informações de padrão de recorrência. Em seguida, o servidor gera ocorrências com base no padrão de recorrência em resposta às solicitações do cliente para informações de compromisso, usando um processo chamado expansão. Essas ocorrências geradas não são armazenadas permanentemente no servidor. Isso é importante para entender porque a maneira como você pesquisa itens de calendário determina quais informações você recebe e se ocorre expansão.
  
## <a name="recurrence-patterns"></a>Padrões de recorrência

A peça-chave para uma série recorrente que possibilita a expansão é o padrão de recorrência. O padrão de recorrência é encontrado no mestre recorrente e descreve um conjunto de critérios para calcular ocorrências com base na data e hora do mestre recorrente.
  
**Tabela 1. Padrões de recorrência disponíveis**

|**Classe api gerenciada do EWS**|**Elemento EWS**|**Exemplos**|
|:-----|:-----|:-----|
|[Recurrence.DailyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Repita todos os dias.  <br/> Repita a cada dois dias.  <br/> |
|[Recurrence.MonthlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Repita todos os meses no décimo dia do mês.  <br/> Repita a cada dois meses no vigésimo primeiro dia do mês.  <br/> |
|[Recurrence.RelativeMonthlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Repita na segunda terça-feira de cada mês.  <br/> Repita na terceira quinta-feira do mês a cada três meses.  <br/> |
|[Recurrence.RelativeYearlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Repita na primeira segunda-feira de agosto de cada ano.  <br/> |
|[Recurrence.WeeklyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Repita todas as segundas-feiras.  <br/> Repita todas as terças e quintas-feiras a cada duas semanas.  <br/> |
|[Recurrence.YearlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Repita em 1º de setembro todos os anos.  <br/> |
   
A outra informação importante para um padrão de recorrência é quando a recorrência termina. Isso pode ser expresso como um número definido de ocorrências, como uma data de término ou como sem fim.
  
**Tabela 2. Opções para o final de uma série recorrente**

|**Método/propriedade da API Gerenciada do EWS**|**Elemento EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Recurrence.NumberOfOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |O valor dessa propriedade ou elemento especifica o número de ocorrências.  <br/> |
|[Recurrence.EndDate](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |A última ocorrência na série se enquadra ou antes da data especificada por essa propriedade ou elemento.  <br/> |
|[Recurrence.HasEnd](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence.NeverEnds](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |A série não tem fim.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Exibições expandidas versus não expandidas

Usar o **método FindAppointments** na API Gerenciada do EWS (ou a operação **FindItem** com um **elemento CalendarView** no EWS) invoca o processo de expansão. Isso oculta compromissos mestras recorrentes do conjunto de resultados e, em vez disso, apresenta uma exibição expandida dessa série recorrente. As ocorrências de e exceções ao mestre recorrente que se enquadram nos parâmetros do visualização de calendário são incluídas no conjunto de resultados. Por outro lado, usar o método **FindItems** na API Gerenciada do EWS (ou a operação **FindItem** com um **elemento IndexedPageItemView** ou **FractionalPageItemView** no EWS) não invoca o processo de expansão, e as ocorrências e exceções não são incluídas. Vejamos um exemplo comparando os dois métodos. 
  
**Tabela 3. Métodos e operações para localizar compromissos**

|**Método da API Gerenciada do EWS**|**Operação do EWS**|**Expande a série?**|**Itens incluídos nos resultados**|
|:-----|:-----|:-----|:-----|
|[ExchangeService.FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um [elemento CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Sim  <br/> |Compromissos não recorrentes, ocorrências únicas de séries recorrentes e exceções a séries recorrentes  <br/> |
|[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um [elemento IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) [ou elemento FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Não  <br/> |Compromissos não recorrentes e compromissos mestras recorrentes  <br/> |
   
Sadie acabou de se inscrevar no seu filho para a equipe de nadação. A equipe tem prática toda quarta-feira de manhã às 8:30 da manhã, começando em 2 de julho, com o último treino sendo em 6 de agosto. Sem querer esquecer a prática, Sadie adiciona um compromisso recorrente ao calendário para lembrá-la.
  
**Tabela 4. Compromisso recorrente de Sadie**

|**Campo Compromisso**|**Value**|
|:-----|:-----|
|Assunto  <br/> |Prática de Equipe de Nadação  <br/> |
|Início  <br/> |2 de julho de 2014 8:30 AM  <br/> |
|End  <br/> |2 de julho de 2014 10:00 AM  <br/> |
|Recurs  <br/> |Todas as quartas-feiras  <br/> |
|Última ocorrência  <br/> |6 de agosto de 2014 8:30 AM  <br/> |
   
Uma rápida olhada em um calendário mostra que a equipe terá um total de seis práticas. No entanto, não há seis itens de compromisso distintos no calendário. Em vez disso, há apenas um compromisso mestre recorrente representando a série.
  
Agora vamos procurar encontrar compromissos no calendário de Sadie que ocorrem no mês de julho. O exemplo de código a seguir usa o **método FindItems** na API gerenciada Exchange para produzir uma exibição não expandida do calendário de Sadie. 
  
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

Esse código resulta na seguinte solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um [elemento IndexedPageItemView.](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) 
  
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

A resposta do servidor inclui apenas um único item, o mestre recorrente, indicado pelo valor do elemento [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) **de RecurringMaster**. O valor do [elemento ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para a capacidade de leitura. 
  
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

Agora vamos comparar com um exibição expandido. O exemplo de código a seguir usa o **método FindAppointments** na API Gerenciada do EWS para criar uma exibição expandida do calendário de Sadie. 
  
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

Este código resulta na seguinte solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um [elemento CalendarView.](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) 
  
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

Desta vez, a resposta do servidor inclui cinco ocorrências, uma para cada quarta-feira de julho. Os [elementos CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) nesses itens têm um valor **de Ocorrência**. Observe que o mestre recorrente não está presente na resposta. Os valores dos [elementos ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foram reduzidos para a capacidade de leitura. 
  
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

Depois de ter um mestre recorrente, uma ocorrência ou uma exceção, você sempre pode [recuperar os outros itens relacionados.](how-to-access-a-recurring-series-by-using-ews-in-exchange.md) Dada uma ocorrência ou exceção, você pode recuperar o mestre recorrente e vice-versa.
  
## <a name="working-with-recurring-calendar-items"></a>Trabalhar com itens de calendário recorrentes

Você usa todos os mesmos métodos e operações para trabalhar com séries recorrentes que você usa para trabalhar com itens de calendário não recorrentes. A diferença é que, dependendo do item usado para invocar esses métodos ou operações, as ações realizadas podem ser aplicadas a toda a série ou apenas uma única ocorrência. [As ações tomadas no mestre](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) recorrente serão aplicadas [a](how-to-update-a-recurring-series-by-using-ews.md) todas as ocorrências na série, enquanto as ações tomadas a uma única ocorrência ou exceção só se aplicarão a essa ocorrência ou exceção. 
  
## <a name="in-this-section"></a>Nesta seção

- [Acessar uma série recorrente usando o EWS no Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Criar uma série recorrente usando o EWS no Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Excluir compromissos em uma série recorrente usando o EWS em Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Atualizar uma série recorrente usando o EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Atualizar uma série recorrente usando o EWS no Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

