---
title: Excluir compromissos em uma série recorrente usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Aprenda a excluir compromissos em uma série recorrente, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 5e4d95058808adf8db159000bdf90c1f92945338
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750728"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="9d1c0-103">Excluir compromissos em uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1c0-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="9d1c0-104">Aprenda a excluir compromissos em uma série recorrente, usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="9d1c0-105">Você pode usar a API gerenciada de EWS ou o EWS para excluir uma série de compromissos ou reuniões, ou apenas uma instância na série.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="9d1c0-106">O processo usado para excluir uma série inteira é essencialmente o mesmo que o processo que você usa para excluir apenas uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="9d1c0-107">Você usa os mesmos métodos de API gerenciada de EWS ou operações do EWS que você usa para [Excluir uma reunião ou um compromisso de única instância](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="9d1c0-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="9d1c0-108">A diferença é a ID do item que está incluído no método ou a operação.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="9d1c0-109">Vamos começar examinando como dois cenários são iguais.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="9d1c0-110">Para excluir uma série recorrente ou uma única ocorrência de uma série recorrente, você precisa encontrar a ocorrência ou série que você deseja excluir e, em seguida, chame o método apropriado ou operação para removê-lo.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-110">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it.</span></span> <span data-ttu-id="9d1c0-111">Enquanto você pode simplesmente excluir qualquer tipo de compromisso, recomendamos que você mantenha qualquer participantes ou o organizador atualizado e cancelar reuniões que o usuário organizou e recusa reuniões que o usuário não organizar.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-111">While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="9d1c0-112">Assim como são os cenários diferentes?</span><span class="sxs-lookup"><span data-stu-id="9d1c0-112">So how are the scenarios different?</span></span> <span data-ttu-id="9d1c0-113">Ele é tudo sobre o objeto de [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) utilizado para chamar o método (para o EWS Managed API) ou a ID do item incluído na solicitação de operação (para o EWS).</span><span class="sxs-lookup"><span data-stu-id="9d1c0-113">It's all about the [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="9d1c0-114">Para excluir uma série inteira, a ID de objeto ou item de **compromisso** são necessários para o mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="9d1c0-115">Para excluir uma ocorrência única, será necessário o ID de objeto ou item de **compromisso** para a ocorrência.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="9d1c0-116">Excluir um compromisso recorrente usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="9d1c0-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="9d1c0-117">Este exemplo pressupõe que você tenha autenticado com um servidor Exchange e adquiriu um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) denominado **service**.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="9d1c0-118">O parâmetro _recurringItem_ é um objeto de **compromisso** para uma ocorrência única ou o mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="9d1c0-119">O parâmetro _deleteEntireSeries_ indica se você deseja excluir a série inteira que o _recurringItem_ é uma parte do.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
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

<span data-ttu-id="9d1c0-120">Para usar este exemplo, você precisa [associar a uma ocorrência ou do mestre recorrente](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)e passe o objeto resultante de **compromisso** para o método.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="9d1c0-121">Mantenha em mente que, se você acessar compromissos usando uma classe de [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , os itens resultantes são todas as ocorrências única.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-121">Keep in mind that if you access appointments by using a [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="9d1c0-122">De modo oposto, se você usar a classe [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , os itens de resultantes são todos os mestres recorrentes.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-122">Conversely, if you use the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="9d1c0-123">Excluir um compromisso recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="9d1c0-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="9d1c0-124">Excluir uma série recorrente, usando o EWS é o mesmo que [a exclusão de uma reunião de ocorrência única](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="9d1c0-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="9d1c0-125">Na verdade, as solicitações de SOAP terão o mesmo formato.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="9d1c0-126">Novamente, a chave é a ID de item usada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="9d1c0-127">Se a ID do item corresponde ao mestre recorrente, a série inteira será excluída.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="9d1c0-128">Se a ID do item corresponder a uma única ocorrência, somente essa ocorrência será excluída.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="9d1c0-129">Nos exemplos de código que seguem, os atributos **ItemId** **ChangeKey**e **RecurringMasterId** são reduzidos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="9d1c0-130">Este exemplo usa a [operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) com um elemento [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) cancelar uma reunião para o qual o usuário é o organizador.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-130">This example uses the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="9d1c0-131">O valor do elemento [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indica o item para cancelar, e pode ser a ID de item de um mestre recorrente ou uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-131">The value of the [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="9d1c0-132">Este exemplo usa a **operação CreateItem** com um elemento [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) para recusar uma reunião para o qual o usuário não for o organizador.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-132">This example uses the **CreateItem operation** with a [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="9d1c0-133">Como no exemplo anterior, o valor do elemento **ReferenceItemId** indica o item para recusar, e pode ser a ID de item de um mestre recorrente ou uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="9d1c0-134">Este exemplo usa a [operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) para excluir uma única ocorrência de um compromisso com nenhum participante.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-134">This example uses the [DeleteItem operation](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="9d1c0-135">Para excluir a ocorrência é especificada pelo elemento [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , que é construído a partir do mestre recorrente a ID do item e o índice da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-135">The occurrence to delete is specified by the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="9d1c0-136">Observe que você pode obter o mesmo resultado, substituindo o elemento **OccurrenceItemId** por um elemento [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) que contém a ID do item da ocorrência, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="9d1c0-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="9d1c0-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="9d1c0-137">See also</span></span>


- [<span data-ttu-id="9d1c0-138">Padrões de recorrência e EWS</span><span class="sxs-lookup"><span data-stu-id="9d1c0-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="9d1c0-139">Acessar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1c0-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9d1c0-140">Criar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1c0-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9d1c0-141">Atualizar uma série recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="9d1c0-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="9d1c0-142">Atualizar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1c0-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9d1c0-143">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1c0-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="9d1c0-144">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9d1c0-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="9d1c0-145">Excluir compromissos e cancelar reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d1c0-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

