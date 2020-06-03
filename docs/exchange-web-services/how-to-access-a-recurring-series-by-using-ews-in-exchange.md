---
title: Acessar uma série recorrente usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Saiba como acessar itens de calendário em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: dca41472b3b2f775f420b6654d7e43ef456b0583
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456889"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="b6f41-103">Acessar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6f41-103">Access a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="b6f41-104">Saiba como acessar itens de calendário em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6f41-104">Learn how to access calendar items in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b6f41-105">Uma série recorrente de compromissos ou reuniões é composta de um mestre recorrente, várias ocorrências em uma série que se repetem de acordo com um padrão definido e, opcionalmente, conjuntos de ocorrências que foram alterados e que foram excluídos.</span><span class="sxs-lookup"><span data-stu-id="b6f41-105">A recurring series of appointments or meetings is made up of a recurring master, a number of occurrences in a series that repeat according to a set pattern, and, optionally, sets of occurrences that were changed and that were deleted.</span></span> <span data-ttu-id="b6f41-106">Você pode usar a API gerenciada do EWS ou o EWS para acessar itens de calendário em uma série recorrente.</span><span class="sxs-lookup"><span data-stu-id="b6f41-106">You can use the EWS Managed API or EWS to access calendar items in a recurring series.</span></span> <span data-ttu-id="b6f41-107">Isso permite que você:</span><span class="sxs-lookup"><span data-stu-id="b6f41-107">This enables you to:</span></span>
  
- <span data-ttu-id="b6f41-108">Verifique se um item de calendário associado a uma ID de item é um mestre recorrente, uma ocorrência em uma série ou uma exceção a uma série.</span><span class="sxs-lookup"><span data-stu-id="b6f41-108">Check to see if a calendar item associated with an item ID is a recurring master, an occurrence in a series, or an exception to a series.</span></span>
    
- <span data-ttu-id="b6f41-109">Procure compromissos de recorrência na pasta calendário.</span><span class="sxs-lookup"><span data-stu-id="b6f41-109">Search your calendar folder for recurrence appointments.</span></span>
    
- <span data-ttu-id="b6f41-110">Obter itens de calendário de recorrência relacionados</span><span class="sxs-lookup"><span data-stu-id="b6f41-110">Get related recurrence calendar items</span></span>
    
- <span data-ttu-id="b6f41-111">Iterar por meio de ocorrências em uma série, exceções de ocorrência ou exclusões de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="b6f41-111">Iterate through occurrences in a series, occurrence exceptions, or occurrence deletions.</span></span>
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="b6f41-112">Obter uma coleção de itens de calendário recorrentes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="b6f41-112">Get a collection of recurring calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="b6f41-113">Se você quiser recuperar uma coleção de compromissos, você pode usar o método [ExchangeService. FindAppointments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para recuperar todos os compromissos entre uma determinada data de início e término e, em seguida, adicionar todos os itens de calendário com um tipo de compromisso de **ocorrência** ou **exceção** a uma coleção, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="b6f41-113">If you want to retrieve a collection of appointments, you can use the [ExchangeService.FindAppointments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve all appointments between a given start and end date, and then add all calendar items with an appointment type of **Occurrence** or **Exception** to a collection, as shown in the following example.</span></span> 
  
<span data-ttu-id="b6f41-114">Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**.</span><span class="sxs-lookup"><span data-stu-id="b6f41-114">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

<span data-ttu-id="b6f41-115">Observe que os itens de calendário mestre recorrentes não são retornados em uma chamada para **FindAppointments**.</span><span class="sxs-lookup"><span data-stu-id="b6f41-115">Note that recurring master calendar items aren't returned in a call to **FindAppointments**.</span></span> <span data-ttu-id="b6f41-116">Se você quiser recuperar os mestres recorrentes ou desejar uma abordagem mais geral para recuperar itens de calendário, você precisará usar [ExchangeService. FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b6f41-116">If you want to retrieve recurring masters, or you want a more general approach to retrieving calendar items, you need to use [ExchangeService.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="b6f41-117">Você pode usar um filtro de pesquisa para recuperar apenas itens com uma data de início maior ou igual a uma data que você escolher, e um modo de exibição de item para limitar o número de itens a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="b6f41-117">You can then use a search filter to retrieve only items with a start date greater than or equal to a date you choose, and an item view to limit the number of items to return.</span></span> <span data-ttu-id="b6f41-118">Observe que um mestre recorrente com uma data de início anterior à data de início da pesquisa não será localizado, mesmo se houver ocorrências nesse intervalo.</span><span class="sxs-lookup"><span data-stu-id="b6f41-118">Note that a recurring master with a start date earlier than the start date in your search will not be found, even if occurrences occur in this range.</span></span>
  
<span data-ttu-id="b6f41-119">Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**.</span><span class="sxs-lookup"><span data-stu-id="b6f41-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="b6f41-120">Obter itens de calendário de recorrência relacionados usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="b6f41-120">Get related recurrence calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="b6f41-121">Às vezes, você tem uma peça do quebra-cabeça, mas para resolver o que precisa do restante das peças.</span><span class="sxs-lookup"><span data-stu-id="b6f41-121">Sometimes you have one piece of the puzzle, but to solve it you need the rest of the pieces.</span></span> <span data-ttu-id="b6f41-122">Se você tiver a ID de item para um item de calendário de recorrência, poderá obter as outras partes necessárias usando uma das várias propriedades ou métodos da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="b6f41-122">If you have the item ID for a recurrence calendar item, you can get the other pieces you need by using one of several EWS Managed API properties or methods.</span></span>
  
<span data-ttu-id="b6f41-123">**Tabela 1. Propriedade ou método da API gerenciada do EWS a ser usado para obter itens de calendário de recorrência relacionados**</span><span class="sxs-lookup"><span data-stu-id="b6f41-123">**Table 1. EWS Managed API property or method to use to get related recurrence calendar items**</span></span>

|<span data-ttu-id="b6f41-124">**Se você tiver a ID do item para...**</span><span class="sxs-lookup"><span data-stu-id="b6f41-124">**If you have the item ID for…**</span></span>|<span data-ttu-id="b6f41-125">**Você pode obter...**</span><span class="sxs-lookup"><span data-stu-id="b6f41-125">**You can get…**</span></span>|<span data-ttu-id="b6f41-126">**Usando a...**</span><span class="sxs-lookup"><span data-stu-id="b6f41-126">**By using the…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b6f41-127">O item de calendário mestre recorrente</span><span class="sxs-lookup"><span data-stu-id="b6f41-127">The recurring master calendar item</span></span>  <br/> | <span data-ttu-id="b6f41-128">A primeira ocorrência em uma série</span><span class="sxs-lookup"><span data-stu-id="b6f41-128">The first occurrence in a series</span></span>  <br/>  <span data-ttu-id="b6f41-129">A última ocorrência em uma série</span><span class="sxs-lookup"><span data-stu-id="b6f41-129">The last occurrence in a series</span></span>  <br/>  <span data-ttu-id="b6f41-130">As exceções de uma série</span><span class="sxs-lookup"><span data-stu-id="b6f41-130">The exceptions to a series</span></span>  <br/>  <span data-ttu-id="b6f41-131">Os compromissos excluídos em uma série</span><span class="sxs-lookup"><span data-stu-id="b6f41-131">The deleted appointments in a series</span></span>  <br/>  <span data-ttu-id="b6f41-132">Qualquer ocorrência (dado seu índice)</span><span class="sxs-lookup"><span data-stu-id="b6f41-132">Any occurrence (given its index)</span></span>  <br/> |<span data-ttu-id="b6f41-133">Propriedade [compromisso. FirstOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-133">[Appointment.FirstOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="b6f41-134">Propriedade [compromisso. LastOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-134">[Appointment.LastOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="b6f41-135">Propriedade [compromisso. ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-135">[Appointment.ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="b6f41-136">Propriedade [compromisso. DeletedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-136">[Appointment.DeletedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="b6f41-137">Método de [compromisso. BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-137">[Appointment.BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="b6f41-138">Uma única ocorrência em uma série</span><span class="sxs-lookup"><span data-stu-id="b6f41-138">A single occurrence in a series</span></span>  <br/> |<span data-ttu-id="b6f41-139">O mestre recorrente</span><span class="sxs-lookup"><span data-stu-id="b6f41-139">The recurring master</span></span>  <br/> |<span data-ttu-id="b6f41-140">Método de [compromisso. BindToRecurringMaster](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-140">[Appointment.BindToRecurringMaster](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="b6f41-141">Qualquer item de calendário (um objeto [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) )</span><span class="sxs-lookup"><span data-stu-id="b6f41-141">Any calendar item (an [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object)</span></span>  <br/> |<span data-ttu-id="b6f41-142">O valor de enumeração de [tipo de compromisso](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-142">The [appointment type](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx) enumeration value</span></span>  <br/> |<span data-ttu-id="b6f41-143">Propriedade [compromisso. compromissotype](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b6f41-143">[Appointment.AppointmentType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) property</span></span>  <br/> |
   
<span data-ttu-id="b6f41-144">O exemplo de código a seguir mostra como obter um mestre recorrente, a primeira ou a última ocorrência em uma série ou uma ocorrência de acordo com o índice.</span><span class="sxs-lookup"><span data-stu-id="b6f41-144">The following code example shows how to get a recurring master, the first or last occurrence in a series, or an occurrence given its index.</span></span>
  
<span data-ttu-id="b6f41-145">Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**.</span><span class="sxs-lookup"><span data-stu-id="b6f41-145">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a><span data-ttu-id="b6f41-146">Acessar itens de calendário em uma série recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="b6f41-146">Access calendar items in a recurring series by using EWS</span></span>

<span data-ttu-id="b6f41-147">O acesso a itens de calendário em uma série recorrente é muito semelhante ao acesso a instâncias únicas de itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="b6f41-147">Accessing calendar items in a recurring series is very similar to accessing single instances of calendar items.</span></span> <span data-ttu-id="b6f41-148">Use uma solicitação de operação [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) , especificando as propriedades desejadas, com o [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) da instância de compromisso de que você precisa.</span><span class="sxs-lookup"><span data-stu-id="b6f41-148">You use a [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request, specifying the properties you want, with the [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) of the appointment instance you need.</span></span> <span data-ttu-id="b6f41-149">O [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contém o **ItemId** do mestre recorrente da ocorrência, bem como seu valor de índice na série.</span><span class="sxs-lookup"><span data-stu-id="b6f41-149">The [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contains the **ItemID** of the occurrence's recurring master, as well as its index value in the series.</span></span> 
  
<span data-ttu-id="b6f41-150">O XML a seguir mostra a solicitação [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) usada para retornar uma ocorrência em uma série especificada pelo índice.</span><span class="sxs-lookup"><span data-stu-id="b6f41-150">The following XML shows the [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) request used to return an occurrence in a series specified by its index.</span></span> <span data-ttu-id="b6f41-151">Observe que o **ItemId** do mestre recorrente foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6f41-151">Note that the **ItemID** of the recurring master has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b6f41-152">O servidor responde à solicitação **GetItem** com uma mensagem [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que o email foi criado com êxito e o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem recém-criada.</span><span class="sxs-lookup"><span data-stu-id="b6f41-152">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b6f41-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="b6f41-153">See also</span></span>


- [<span data-ttu-id="b6f41-154">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6f41-154">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
- [<span data-ttu-id="b6f41-155">Obter compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6f41-155">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

