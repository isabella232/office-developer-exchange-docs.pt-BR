---
title: Excluir compromissos em uma série recorrente usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Saiba como excluir compromissos em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 5646a30d218ed4d795044aefe5efea1399d19a79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528122"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="d4ca8-103">Excluir compromissos em uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ca8-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="d4ca8-104">Saiba como excluir compromissos em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="d4ca8-105">Você pode usar a API gerenciada do EWS ou o EWS para excluir uma série de compromissos ou reuniões ou apenas uma instância na série.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="d4ca8-106">O processo que você usa para excluir uma série inteira é essencialmente o mesmo que o processo que você usa para excluir apenas uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="d4ca8-107">Você usa os mesmos métodos da API gerenciada do EWS ou as operações do EWS que você usa para [excluir um único compromisso ou reunião de instância](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="d4ca8-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="d4ca8-108">A diferença está na ID do item incluída no método ou na operação.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="d4ca8-109">Vamos começar examinando como os dois cenários são os mesmos.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="d4ca8-110">Para excluir uma série recorrente ou uma única ocorrência em uma série recorrente, você precisa localizar a ocorrência ou a série que deseja excluir e, em seguida, chamar o método ou a operação apropriado para removê-lo.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-110">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it.</span></span> <span data-ttu-id="d4ca8-111">Embora seja possível simplesmente excluir qualquer tipo de compromisso, recomendamos que você mantenha todos os participantes ou o organizador atualizado e cancele as reuniões que o usuário organizou e recuse reuniões que o usuário não organizou.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-111">While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="d4ca8-112">Então, como os cenários são diferentes?</span><span class="sxs-lookup"><span data-stu-id="d4ca8-112">So how are the scenarios different?</span></span> <span data-ttu-id="d4ca8-113">É tudo sobre o objeto [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) usado para invocar o método (para a API gerenciada do EWS) ou a ID do item incluída na solicitação de operação (para EWS).</span><span class="sxs-lookup"><span data-stu-id="d4ca8-113">It's all about the [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="d4ca8-114">Para excluir uma série inteira, você precisa do objeto **compromisso** ou ID do item para o mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="d4ca8-115">Para excluir uma única ocorrência, você precisará do objeto **compromisso** ou da ID do item da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="d4ca8-116">Excluir um compromisso recorrente usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d4ca8-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="d4ca8-117">Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="d4ca8-118">O parâmetro _recurringItem_ é um objeto de **compromisso** para o mestre recorrente ou uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="d4ca8-119">O parâmetro _deleteEntireSeries_ indica se é para excluir a série inteira à qual o _recurringItem_ faz parte.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
```cs
public static bool DeleteRecurringItem(ExchangeService service, Appointment recurringItem, bool deleteEntireSeries)
{
    Appointment appointmentToDelete = null;
    // If the item is a single appointment, fail.
    if (recurringItem.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        if (!deleteEntireSeries)
        {
            // The item is the recurring master, so deleting it will delete
            // the entire series. The caller indicated that the entire series
            // should not be deleted, so fail.
            Console.WriteLine("ERROR: The item to delete is the recurring master of the series. Deleting it will delete the entire series.");
            return false;
        }
        else
        {
            appointmentToDelete = recurringItem;
        }
    }
    else
    {
        if (deleteEntireSeries)
        {
            // The item passed is not the recurring master, but the caller
            // wants to delete the entire series. Bind to the recurring
            // master to delete it.
            try
            {
                appointmentToDelete = Appointment.BindToRecurringMaster(service, recurringItem.Id);
            }
            catch (Exception ex)
            {
                Console.WriteLine("ERROR: {0}", ex.Message);
                return false;
            }
        }
        else
        {
            // The item passed is not the recurring master, but the caller
            // only wants to delete the occurrence, so just
            // delete the passed item.
            appointmentToDelete = recurringItem;
        }
    }
    if (appointmentToDelete != null)
    {
        // Remove the item, depending on the scenario. 
        if (appointmentToDelete.IsMeeting)
        {
            CalendarActionResults results;
            // If it's a meeting and the user is the organizer, cancel it.
            // Determine this by testing the AppointmentState bitmask for 
            // the presence of the second bit. This bit indicates that the appointment
            // was received, which means that someone sent it to the user. Therefore,
            // they're not the organizer.
            int isReceived = 2;
            if ((appointmentToDelete.AppointmentState &amp; isReceived) == 0)
            {
                results = appointmentToDelete.CancelMeeting("Cancelling this meeting.");
                return true;
            }
            // If it's a meeting and the user is not the organizer, decline it.
            else
            {
                results = appointmentToDelete.Decline(true);
                return true;
            }
        }
        else
        {
            // The item isn't a meeting, so just delete it.
            appointmentToDelete.Delete(DeleteMode.MoveToDeletedItems);
            return true;
        }
    }
    return false;
}
```

<span data-ttu-id="d4ca8-120">Para usar este exemplo, você precisa [associar a uma ocorrência ou ao mestre recorrente](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)e passar o objeto de **compromisso** resultante para o método.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="d4ca8-121">Tenha em mente que, se você acessar compromissos usando uma classe [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , os itens resultantes serão todas as ocorrências únicas.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-121">Keep in mind that if you access appointments by using a [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="d4ca8-122">Por outro lado, se você usar a classe [doview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , os itens resultantes serão todos os mestres recorrentes.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-122">Conversely, if you use the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="d4ca8-123">Excluir um compromisso recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d4ca8-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="d4ca8-124">Excluir uma série recorrente usando o EWS é o mesmo que [excluir uma reunião de instância única](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="d4ca8-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="d4ca8-125">Na verdade, as solicitações SOAP têm o mesmo formato.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="d4ca8-126">Novamente, a chave é a ID do item usada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="d4ca8-127">Se a ID do item corresponder ao mestre recorrente, a série inteira será excluída.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="d4ca8-128">Se a ID do item corresponder a uma única ocorrência, apenas essa ocorrência será excluída.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d4ca8-129">Nos exemplos de código a seguir, os atributos **ItemId**, **ChangeKey**e **recurringMasterId** são reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="d4ca8-130">Este exemplo usa a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) com um elemento [CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) para cancelar uma reunião para a qual o usuário é o organizador.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-130">This example uses the [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="d4ca8-131">O valor do elemento [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indica o item a ser cancelado e pode ser a ID de item de um mestre recorrente ou uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-131">The value of the [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:NewBodyContent BodyType="HTML">Cancelling this meeting.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d4ca8-132">Este exemplo usa a **operação CreateItem** com um elemento [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) para recusar uma reunião para a qual o usuário não é o organizador.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-132">This example uses the **CreateItem operation** with a [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="d4ca8-133">Como no exemplo anterior, o valor do elemento **ReferenceItemId** indica o item a ser recusado e pode ser a ID do item de um mestre recorrente ou uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:DeclineItem>
          <t:ReferenceItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
        </t:DeclineItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d4ca8-134">Este exemplo usa a [Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) para excluir uma única ocorrência de um compromisso sem participantes.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-134">This example uses the [DeleteItem operation](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="d4ca8-135">A ocorrência a ser excluída é especificada pelo elemento [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , que é construído a partir da ID de item do mestre recorrente e do índice da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-135">The occurrence to delete is specified by the [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d4ca8-136">Observe que você pode obter o mesmo resultado substituindo o elemento **OccurrenceItemId** por um elemento [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) que contém a ID do item da ocorrência, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="d4ca8-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="d4ca8-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="d4ca8-137">See also</span></span>


- [<span data-ttu-id="d4ca8-138">Padrões de recorrência e EWS</span><span class="sxs-lookup"><span data-stu-id="d4ca8-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="d4ca8-139">Acessar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ca8-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d4ca8-140">Criar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ca8-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d4ca8-141">Atualizar uma série recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d4ca8-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="d4ca8-142">Atualizar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ca8-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d4ca8-143">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ca8-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="d4ca8-144">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d4ca8-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="d4ca8-145">Excluir compromissos e cancelar reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ca8-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

