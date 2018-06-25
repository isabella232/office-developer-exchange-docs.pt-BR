---
title: Acessar uma série recorrente usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Saiba como acessar os itens do calendário em uma série recorrente, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 9f78ef5b51766a69d23fce3f36c55fbb9422fb16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750668"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a>Acessar uma série recorrente usando o EWS no Exchange

Saiba como acessar os itens do calendário em uma série recorrente, usando a API gerenciada de EWS ou EWS no Exchange.
  
Uma série recorrente de compromissos ou reuniões é composta por um mestre recorrente, um número de ocorrências de uma série que repetem de acordo com um padrão definido e, opcionalmente, conjuntos de ocorrências que foram alteradas e que foram excluídos. Você pode usar a API gerenciada de EWS ou o EWS para acessar itens do calendário em uma série recorrente. Isso permite que você:
  
- Verificar se um item de calendário associado a uma ID de item é um mestre recorrente, uma ocorrência de uma série ou uma exceção a uma série.
    
- Pesquise pasta Calendário os compromissos de recorrência.
    
- Obter itens de calendário de recorrência relacionada
    
- Percorrer ocorrências em uma série, exceções de ocorrência ou exclusões de ocorrência.
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a>Obter uma coleção de itens de calendário recorrentes usando a API gerenciada de EWS

Se você deseja recuperar uma coleção de compromissos, você pode usar o método [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para recuperar todos os compromissos entre uma determinada data de início e término e, em seguida, adicionar todos os itens de calendário com um tipo de compromisso de **ocorrência **ou **exceção** a uma coleção, conforme mostrado no exemplo a seguir. 
  
Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**. 
  
```cs
public static Collection<Appointment> FindRecurringCalendarItems(ExchangeService service, 
                                                                    DateTime startSearchDate, 
                                                                    DateTime endSearchDate)
{
    // Instantiate a collection to hold occurrences and exception calendar items.
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a calendar view to search the calendar folder and specify the properties to return.
    CalendarView calView = new CalendarView(startSearchDate, endSearchDate);
    calView.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                            AppointmentSchema.Subject, 
                                            AppointmentSchema.Start, 
                                            AppointmentSchema.IsRecurring, 
                                            AppointmentSchema.AppointmentType);
    // Retrieve a collection of calendar items.
    FindItemsResults<Appointment> findResults = service.FindAppointments(WellKnownFolderName.Calendar, calView);
    // Add all calendar items in your view that are occurrences or exceptions to your collection.
    foreach (Appointment appt in findResults.Items)
    {
        if (appt.AppointmentType == AppointmentType.Occurrence || appt.AppointmentType == AppointmentType.Exception)
        {
            foundAppointments.Add(appt);
        }
        else
        {
            Console.WriteLine("Discarding calendar item of type {0}.", appt.AppointmentType);
        }
    }
    return foundAppointments;
}

```

Observe que os itens de calendário mestre recorrentes não são retornados em uma chamada para **FindAppointments**. Se você deseja recuperar mestres recorrentes ou quiser uma abordagem mais geral para recuperar itens de calendário, você precisará usar [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx). Em seguida, você pode usar um filtro de pesquisa para recuperar apenas os itens com uma data de início, maior ou igual a data que você escolher e um modo de exibição de item para limitar o número de itens para retornar. Observe que um mestre recorrente com um início data mais cedo do que a data de início de sua pesquisa não será encontrada, mesmo se ocorrerem de ocorrências nesse intervalo.
  
Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**. 
  
```cs
public static Collection<Appointment> FindCalendarItemsByAppointmentType(ExchangeService service, 
                                                                         AppointmentType myAppointmentType, 
                                                                         DateTime startSearchDate)
{
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a search filter based on the start search date.
    SearchFilter.SearchFilterCollection searchFilter = new SearchFilter.SearchFilterCollection();
    searchFilter.Add(new SearchFilter.IsGreaterThanOrEqualTo(AppointmentSchema.Start, startSearchDate));
    // Create an item view to specify which properties to return.
    ItemView view = new ItemView(20);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                       AppointmentSchema.Subject, 
                                       AppointmentSchema.Start, 
                                       AppointmentSchema.AppointmentType,
                                       AppointmentSchema.IsRecurring);
    // Get the appointment items from the server with the properties we specified.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Calendar, searchFilter, view);
    // Add each of the appointments of the type you want to the collection.
    foreach (Item item in findResults.Items)
    {
        Appointment appt = item as Appointment;
        if (appt.AppointmentType == myAppointmentType)
        {
            foundAppointments.Add(appt);
        }
    }
    return foundAppointments;
}

```

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a>Obter itens de calendário de recorrência relacionada usando a API gerenciada de EWS

Em alguns casos, você tem uma peça do quebra-cabeça, mas para resolvê-lo, você precisa o restante das partes. Se você tiver o ID de item para um item de calendário de recorrência, você pode obter as outras partes que precisa usando um dos vários métodos ou propriedades de API gerenciada de EWS.
  
**Tabela 1. API gerenciada de EWS propriedade ou método usar para obter itens de calendário de recorrência relacionada**

|**Se você tiver o ID de item para …**|**Você pode obter …**|**Usando o …**|
|:-----|:-----|:-----|
|O item de calendário mestre recorrente  <br/> | A primeira ocorrência de uma série  <br/>  A última ocorrência de uma série  <br/>  As exceções a uma série  <br/>  Os compromissos excluídos em uma série  <br/>  Qualquer ocorrência (concedida a seu índice)  <br/> |Propriedade [Appointment.FirstOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx)  <br/> Propriedade [Appointment.LastOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx)  <br/> Propriedade [Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx)  <br/> Propriedade [Appointment.DeletedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx)  <br/> Método [Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx)  <br/> |
|Uma única ocorrência de uma série  <br/> |O mestre recorrente  <br/> |Método [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)  <br/> |
|Qualquer item de calendário (um objeto de [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) )  <br/> |O valor de enumeração do [tipo de compromisso](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)  <br/> |Propriedade [Appointment.AppointmentType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx)  <br/> |
   
O exemplo de código a seguir mostra como obter uma ocorrência dado seu índice, a primeira ou a última ocorrência em uma série ou um mestre recorrente.
  
Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**. 
  
```cs
public static void GetRelatedRecurrenceCalendarItems(ExchangeService service, ItemId itemId)
{
    Appointment calendarItem = Appointment.Bind(service, itemId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    PropertySet props = new PropertySet(AppointmentSchema.AppointmentType,
                                        AppointmentSchema.Subject,
                                        AppointmentSchema.FirstOccurrence,
                                        AppointmentSchema.LastOccurrence,
                                        AppointmentSchema.ModifiedOccurrences,
                                        AppointmentSchema.DeletedOccurrences);
    // If the item ID is not for a recurring master, retrieve the recurring master for the series.
    switch (calendarItem.AppointmentType)
    {
        // Calendar item is a recurring master so use Appointment.Bind
        case AppointmentType.RecurringMaster:
            recurrMaster = Appointment.Bind(service, itemId, props);
            break;
        // The calendar item is a single instance meeting, so there are no instances to modify or delete.
        case AppointmentType.Single:
            Console.WriteLine("Item id must reference a calendar item that is part of a recurring series.");
            return;
        // The calendar item is an occurrence in the series, so use BindToRecurringMaster.
        case AppointmentType.Occurrence:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
        // The calendar item is an exception to the series, so use BindToRecurringMaster.                
        case AppointmentType.Exception:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
    }
    // View the first occurrence, last occurrence, and number of modified and deleted occurrences associated with the recurring master.
    Console.WriteLine("Information for the {0} recurring series:", recurrMaster.Subject);
    Console.WriteLine("The start time for the first appointment with id \t{0} was on \t{1}.", 
                        recurrMaster.FirstOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.FirstOccurrence.Start.ToString());
    Console.WriteLine("The start time for the last appointment with id \t{0} will be on \t{1}.", 
                        recurrMaster.LastOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.LastOccurrence.Start.ToString());
    Console.WriteLine("There are {0} modified occurrences and {1} deleted occurrences.", 
                        recurrMaster.ModifiedOccurrences == null ? "no" : recurrMaster.ModifiedOccurrences.Count.ToString(), 
                        recurrMaster.DeletedOccurrences == null ? "no" : recurrMaster.DeletedOccurrences.Count.ToString());
    // Bind to the first occurrence of a series by using its index.
    Appointment firstOccurrence = Appointment.BindToOccurrence(service, 
                                                                recurrMaster.Id, 
                                                                1, // Index of first item is 1, not 0.
                                                                new PropertySet(AppointmentSchema.AppointmentType,
                                                                                AppointmentSchema.Start));
    Console.WriteLine("Compare the start times for a recurring master's first occurrence " + 
                        "and the occurrence found at index 1 using the BindToOccurrence method:");
    Console.WriteLine("The appointment at index 1 has a start time of\t\t\t\t {0}\n" +
                        "Which matches that of the first occurrence on the recurring master: \t {1}",
                        firstOccurrence.Start.ToString(),
                        recurrMaster.FirstOccurrence.Start.ToString());
}

```

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a>Itens do calendário do Access em uma série recorrente usando o EWS

Acessar os itens do calendário em uma série recorrente é muito semelhante à acessando única instâncias dos itens de calendário. Você usar uma solicitação de operação [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) , especificando as propriedades desejadas, com o [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) da instância do compromisso, que você precisa. O [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contém o **ItemID** do mestre de recorrente a ocorrência, bem como seu valor de índice da série. 
  
O XML a seguir mostra a solicitação de [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) usada para retornar uma ocorrência de uma série especificada pelo índice. Observe que o **ItemID** do mestre recorrente foi reduzida para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Start" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkA" InstanceIndex="1" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, que indica se o email foi criado com êxito e o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do recentemente mensagem criada. 
  
## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
- [Obtenha os compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

