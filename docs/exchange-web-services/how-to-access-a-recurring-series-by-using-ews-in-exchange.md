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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750668"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="6cef8-103">Acessar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6cef8-103">Access a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="6cef8-104">Saiba como acessar os itens do calendário em uma série recorrente, usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cef8-104">Learn how to access calendar items in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="6cef8-105">Uma série recorrente de compromissos ou reuniões é composta por um mestre recorrente, um número de ocorrências de uma série que repetem de acordo com um padrão definido e, opcionalmente, conjuntos de ocorrências que foram alteradas e que foram excluídos.</span><span class="sxs-lookup"><span data-stu-id="6cef8-105">A recurring series of appointments or meetings is made up of a recurring master, a number of occurrences in a series that repeat according to a set pattern, and, optionally, sets of occurrences that were changed and that were deleted.</span></span> <span data-ttu-id="6cef8-106">Você pode usar a API gerenciada de EWS ou o EWS para acessar itens do calendário em uma série recorrente.</span><span class="sxs-lookup"><span data-stu-id="6cef8-106">You can use the EWS Managed API or EWS to access calendar items in a recurring series.</span></span> <span data-ttu-id="6cef8-107">Isso permite que você:</span><span class="sxs-lookup"><span data-stu-id="6cef8-107">This enables you to:</span></span>
  
- <span data-ttu-id="6cef8-108">Verificar se um item de calendário associado a uma ID de item é um mestre recorrente, uma ocorrência de uma série ou uma exceção a uma série.</span><span class="sxs-lookup"><span data-stu-id="6cef8-108">Check to see if a calendar item associated with an item ID is a recurring master, an occurrence in a series, or an exception to a series.</span></span>
    
- <span data-ttu-id="6cef8-109">Pesquise pasta Calendário os compromissos de recorrência.</span><span class="sxs-lookup"><span data-stu-id="6cef8-109">Search your calendar folder for recurrence appointments.</span></span>
    
- <span data-ttu-id="6cef8-110">Obter itens de calendário de recorrência relacionada</span><span class="sxs-lookup"><span data-stu-id="6cef8-110">Get related recurrence calendar items</span></span>
    
- <span data-ttu-id="6cef8-111">Percorrer ocorrências em uma série, exceções de ocorrência ou exclusões de ocorrência.</span><span class="sxs-lookup"><span data-stu-id="6cef8-111">Iterate through occurrences in a series, occurrence exceptions, or occurrence deletions.</span></span>
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="6cef8-112">Obter uma coleção de itens de calendário recorrentes usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6cef8-112">Get a collection of recurring calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="6cef8-113">Se você deseja recuperar uma coleção de compromissos, você pode usar o método [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para recuperar todos os compromissos entre uma determinada data de início e término e, em seguida, adicionar todos os itens de calendário com um tipo de compromisso de **ocorrência **ou **exceção** a uma coleção, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="6cef8-113">If you want to retrieve a collection of appointments, you can use the [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve all appointments between a given start and end date, and then add all calendar items with an appointment type of **Occurrence** or **Exception** to a collection, as shown in the following example.</span></span> 
  
<span data-ttu-id="6cef8-114">Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**.</span><span class="sxs-lookup"><span data-stu-id="6cef8-114">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

<span data-ttu-id="6cef8-115">Observe que os itens de calendário mestre recorrentes não são retornados em uma chamada para **FindAppointments**.</span><span class="sxs-lookup"><span data-stu-id="6cef8-115">Note that recurring master calendar items aren't returned in a call to **FindAppointments**.</span></span> <span data-ttu-id="6cef8-116">Se você deseja recuperar mestres recorrentes ou quiser uma abordagem mais geral para recuperar itens de calendário, você precisará usar [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6cef8-116">If you want to retrieve recurring masters, or you want a more general approach to retrieving calendar items, you need to use [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="6cef8-117">Em seguida, você pode usar um filtro de pesquisa para recuperar apenas os itens com uma data de início, maior ou igual a data que você escolher e um modo de exibição de item para limitar o número de itens para retornar.</span><span class="sxs-lookup"><span data-stu-id="6cef8-117">You can then use a search filter to retrieve only items with a start date greater than or equal to a date you choose, and an item view to limit the number of items to return.</span></span> <span data-ttu-id="6cef8-118">Observe que um mestre recorrente com um início data mais cedo do que a data de início de sua pesquisa não será encontrada, mesmo se ocorrerem de ocorrências nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="6cef8-118">Note that a recurring master with a start date earlier than the start date in your search will not be found, even if occurrences occur in this range.</span></span>
  
<span data-ttu-id="6cef8-119">Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**.</span><span class="sxs-lookup"><span data-stu-id="6cef8-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="6cef8-120">Obter itens de calendário de recorrência relacionada usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6cef8-120">Get related recurrence calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="6cef8-121">Em alguns casos, você tem uma peça do quebra-cabeça, mas para resolvê-lo, você precisa o restante das partes.</span><span class="sxs-lookup"><span data-stu-id="6cef8-121">Sometimes you have one piece of the puzzle, but to solve it you need the rest of the pieces.</span></span> <span data-ttu-id="6cef8-122">Se você tiver o ID de item para um item de calendário de recorrência, você pode obter as outras partes que precisa usando um dos vários métodos ou propriedades de API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="6cef8-122">If you have the item ID for a recurrence calendar item, you can get the other pieces you need by using one of several EWS Managed API properties or methods.</span></span>
  
<span data-ttu-id="6cef8-123">**Tabela 1. API gerenciada de EWS propriedade ou método usar para obter itens de calendário de recorrência relacionada**</span><span class="sxs-lookup"><span data-stu-id="6cef8-123">**Table 1. EWS Managed API property or method to use to get related recurrence calendar items**</span></span>

|<span data-ttu-id="6cef8-124">**Se você tiver o ID de item para …**</span><span class="sxs-lookup"><span data-stu-id="6cef8-124">**If you have the item ID for…**</span></span>|<span data-ttu-id="6cef8-125">**Você pode obter …**</span><span class="sxs-lookup"><span data-stu-id="6cef8-125">**You can get…**</span></span>|<span data-ttu-id="6cef8-126">**Usando o …**</span><span class="sxs-lookup"><span data-stu-id="6cef8-126">**By using the…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6cef8-127">O item de calendário mestre recorrente</span><span class="sxs-lookup"><span data-stu-id="6cef8-127">The recurring master calendar item</span></span>  <br/> | <span data-ttu-id="6cef8-128">A primeira ocorrência de uma série</span><span class="sxs-lookup"><span data-stu-id="6cef8-128">The first occurrence in a series</span></span>  <br/>  <span data-ttu-id="6cef8-129">A última ocorrência de uma série</span><span class="sxs-lookup"><span data-stu-id="6cef8-129">The last occurrence in a series</span></span>  <br/>  <span data-ttu-id="6cef8-130">As exceções a uma série</span><span class="sxs-lookup"><span data-stu-id="6cef8-130">The exceptions to a series</span></span>  <br/>  <span data-ttu-id="6cef8-131">Os compromissos excluídos em uma série</span><span class="sxs-lookup"><span data-stu-id="6cef8-131">The deleted appointments in a series</span></span>  <br/>  <span data-ttu-id="6cef8-132">Qualquer ocorrência (concedida a seu índice)</span><span class="sxs-lookup"><span data-stu-id="6cef8-132">Any occurrence (given its index)</span></span>  <br/> |<span data-ttu-id="6cef8-133">Propriedade [Appointment.FirstOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-133">[Appointment.FirstOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="6cef8-134">Propriedade [Appointment.LastOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-134">[Appointment.LastOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="6cef8-135">Propriedade [Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-135">[Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="6cef8-136">Propriedade [Appointment.DeletedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-136">[Appointment.DeletedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="6cef8-137">Método [Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-137">[Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="6cef8-138">Uma única ocorrência de uma série</span><span class="sxs-lookup"><span data-stu-id="6cef8-138">A single occurrence in a series</span></span>  <br/> |<span data-ttu-id="6cef8-139">O mestre recorrente</span><span class="sxs-lookup"><span data-stu-id="6cef8-139">The recurring master</span></span>  <br/> |<span data-ttu-id="6cef8-140">Método [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-140">[Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="6cef8-141">Qualquer item de calendário (um objeto de [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) )</span><span class="sxs-lookup"><span data-stu-id="6cef8-141">Any calendar item (an [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object)</span></span>  <br/> |<span data-ttu-id="6cef8-142">O valor de enumeração do [tipo de compromisso](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-142">The [appointment type](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx) enumeration value</span></span>  <br/> |<span data-ttu-id="6cef8-143">Propriedade [Appointment.AppointmentType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6cef8-143">[Appointment.AppointmentType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) property</span></span>  <br/> |
   
<span data-ttu-id="6cef8-144">O exemplo de código a seguir mostra como obter uma ocorrência dado seu índice, a primeira ou a última ocorrência em uma série ou um mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="6cef8-144">The following code example shows how to get a recurring master, the first or last occurrence in a series, or an occurrence given its index.</span></span>
  
<span data-ttu-id="6cef8-145">Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**.</span><span class="sxs-lookup"><span data-stu-id="6cef8-145">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a><span data-ttu-id="6cef8-146">Itens do calendário do Access em uma série recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6cef8-146">Access calendar items in a recurring series by using EWS</span></span>

<span data-ttu-id="6cef8-147">Acessar os itens do calendário em uma série recorrente é muito semelhante à acessando única instâncias dos itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="6cef8-147">Accessing calendar items in a recurring series is very similar to accessing single instances of calendar items.</span></span> <span data-ttu-id="6cef8-148">Você usar uma solicitação de operação [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) , especificando as propriedades desejadas, com o [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) da instância do compromisso, que você precisa.</span><span class="sxs-lookup"><span data-stu-id="6cef8-148">You use a [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request, specifying the properties you want, with the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) of the appointment instance you need.</span></span> <span data-ttu-id="6cef8-149">O [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contém o **ItemID** do mestre de recorrente a ocorrência, bem como seu valor de índice da série.</span><span class="sxs-lookup"><span data-stu-id="6cef8-149">The [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contains the **ItemID** of the occurrence's recurring master, as well as its index value in the series.</span></span> 
  
<span data-ttu-id="6cef8-150">O XML a seguir mostra a solicitação de [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) usada para retornar uma ocorrência de uma série especificada pelo índice.</span><span class="sxs-lookup"><span data-stu-id="6cef8-150">The following XML shows the [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) request used to return an occurrence in a series specified by its index.</span></span> <span data-ttu-id="6cef8-151">Observe que o **ItemID** do mestre recorrente foi reduzida para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6cef8-151">Note that the **ItemID** of the recurring master has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="6cef8-152">O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, que indica se o email foi criado com êxito e o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do recentemente mensagem criada.</span><span class="sxs-lookup"><span data-stu-id="6cef8-152">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6cef8-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="6cef8-153">See also</span></span>


- [<span data-ttu-id="6cef8-154">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6cef8-154">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
- [<span data-ttu-id="6cef8-155">Obtenha os compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6cef8-155">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

