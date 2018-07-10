---
title: Calendários e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Saiba mais sobre pastas de calendário, calendários e itens, compromissos e reuniões no Exchange.
ms.openlocfilehash: bb9702118ff1db66862a5788c2d8f58dd55c4d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750644"
---
# <a name="calendars-and-ews-in-exchange"></a><span data-ttu-id="81207-103">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-103">Calendars and EWS in Exchange</span></span>

<span data-ttu-id="81207-104">Saiba mais sobre pastas de calendário, calendários e itens, compromissos e reuniões no Exchange.</span><span class="sxs-lookup"><span data-stu-id="81207-104">Learn about calendars, calendar folders and items, appointments, and meetings in Exchange.</span></span>
  
<span data-ttu-id="81207-105">Você provavelmente está familiarizado com muitos dos recursos de calendário em clientes de email como o Outlook, que permitem controlar compromissos, agendar reuniões, verifique a disponibilidade de pessoas, convidar participantes e alterar ou cancelar reuniões.</span><span class="sxs-lookup"><span data-stu-id="81207-105">You're probably familiar with many of the calendar features in email clients like Outlook, which enable you to track appointments, schedule meetings, check people's availability, invite attendees, and change or cancel meetings.</span></span>
  
<span data-ttu-id="81207-106">Recursos relacionados ao calendário no Exchange são um pouco diferentes do que você vê um cliente como o Outlook.</span><span class="sxs-lookup"><span data-stu-id="81207-106">Calendar-related features in Exchange are a little different than what you see in a client like Outlook.</span></span> <span data-ttu-id="81207-107">Em vez de exiba informações, EWS no Exchange permite que você faça coisas como criar, armazenar, enviar ou alterar as informações.</span><span class="sxs-lookup"><span data-stu-id="81207-107">Instead of displaying information, EWS in Exchange enables you to do things like create, store, send, or change information.</span></span> <span data-ttu-id="81207-108">Para usar o EWS para trabalhar com calendários, você precisará estar familiarizado com os conceitos, como o armazenamento de informações, tempo, recorrência e fluxo de mensagens.</span><span class="sxs-lookup"><span data-stu-id="81207-108">To use EWS to work with calendars, you'll need to be familiar with concepts such as information storage, time, recurrence, and message flow.</span></span> <span data-ttu-id="81207-109">Mais especificamente, você precisará estar familiarizado com os seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="81207-109">More specifically, you'll need to be familiar with the following:</span></span>
  
- <span data-ttu-id="81207-110">Pastas de calendário, itens de calendário e exibições de calendário</span><span class="sxs-lookup"><span data-stu-id="81207-110">Calendar folders, calendar items, and calendar views</span></span>
    
- <span data-ttu-id="81207-111">Solicitações de reunião, respostas, agendamento, participantes, recursos, salas e disponibilidade</span><span class="sxs-lookup"><span data-stu-id="81207-111">Meeting requests, responses, scheduling, attendees, resources, rooms, and availability</span></span>
    
- <span data-ttu-id="81207-112">Durações de tempo, fusos horários e as horas de início e término de reuniões e compromissos</span><span class="sxs-lookup"><span data-stu-id="81207-112">Time durations, time zones, and start and end times of meetings and appointments</span></span>
    
- <span data-ttu-id="81207-113">Série recorrente, os padrões de recorrência, exceções e compromissos de única instância e reuniões</span><span class="sxs-lookup"><span data-stu-id="81207-113">Recurring series, recurrence patterns, exceptions, and single instance appointments and meetings</span></span>
    
<span data-ttu-id="81207-114">Felizmente, EWS e a API gerenciada de EWS fornecem um rico conjunto de operações e métodos que permitem que você realize uma ampla variedade de tarefas relacionadas ao calendário.</span><span class="sxs-lookup"><span data-stu-id="81207-114">Fortunately, EWS and the EWS Managed API provide a rich set of operations and methods that enable you to perform a wide range of calendar-related tasks.</span></span> <span data-ttu-id="81207-115">Por exemplo, usando a API gerenciada de EWS, você pode criar uma reunião e enviar convites para os participantes com apenas algumas linhas de código, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="81207-115">For example, using the EWS Managed API, you can create a meeting and send invitations to attendees with just a few lines of code, as shown in the following example.</span></span>
  
```cs
            Appointment meeting = new Appointment(service);
            // Set the properties on the meeting object to create the meeting.
            meeting.Subject = "Team building exercise";
            meeting.Body = "Let's learn to really work as a team and then have lunch!";
            meeting.Start = DateTime.Now.AddDays(2);
            meeting.End = meeting.Start.AddHours(2);
            meeting.Location = "Conference Room 12";
            meeting.RequiredAttendees.Add("Mack.Chaves@contoso.com");
            meeting.RequiredAttendees.Add("Sadie.Daniels@contoso.com");
            meeting.OptionalAttendees.Add("Magdalena.Kemp@contoso.com");
            meeting.ReminderMinutesBeforeStart = 60;
            // Send the meeting request
            meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);

```

## <a name="calendar-folders-and-calendar-items"></a><span data-ttu-id="81207-116">Pastas de calendário e itens de calendário</span><span class="sxs-lookup"><span data-stu-id="81207-116">Calendar folders and calendar items</span></span>
<span data-ttu-id="81207-117"><a name="bk_CalendarFolder"> </a></span><span class="sxs-lookup"><span data-stu-id="81207-117"></span></span>

<span data-ttu-id="81207-118">Pastas de calendário contêm itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="81207-118">Calendar folders contain calendar items.</span></span> <span data-ttu-id="81207-119">Pastas de calendário têm uma [classe de pasta](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) de **IPF. Compromisso**e pode incluir apenas os itens definidos pela propriedade [ItemClass](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API, que é associada a um objeto de [Classe de compromisso](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou o elemento do EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="81207-119">Calendar folders have a [folder class](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) of **IPF.Appointment**, and can include only the items defined by the [ItemClass](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API property, which is associated with an [Appointment Class](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, or the EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="81207-120">Itens em uma pasta de calendário são um pouco diferentes de itens em outras pastas em uma caixa de correio, pois ocorrências em uma série recorrente e exceções a uma série recorrente não são reais itens na caixa de correio, mas em vez disso, são armazenadas internamente como anexos para um recorrente mestre.</span><span class="sxs-lookup"><span data-stu-id="81207-120">Items in a Calendar folder are a little different from items in other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master.</span></span> <span data-ttu-id="81207-121">Portanto, para recuperar todos os compromissos em um intervalo de datas determinado, você precisará usar um modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="81207-121">Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view.</span></span> <span data-ttu-id="81207-122">Para saber mais sobre como recuperar compromissos e modos de exibição de calendário, consulte [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="81207-122">To learn more about retrieving appointments and calendar views, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="meetings-and-appointments"></a><span data-ttu-id="81207-123">Reuniões e compromissos</span><span class="sxs-lookup"><span data-stu-id="81207-123">Meetings and appointments</span></span>
<span data-ttu-id="81207-124"><a name="bk_meetings"> </a></span><span class="sxs-lookup"><span data-stu-id="81207-124"></span></span>

<span data-ttu-id="81207-125">A diferença essencial entre reuniões e compromissos é que reuniões possuem participantes, e não de compromissos.</span><span class="sxs-lookup"><span data-stu-id="81207-125">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="81207-126">Internamente, o Exchange usa o mesmo objeto para reuniões e compromissos.</span><span class="sxs-lookup"><span data-stu-id="81207-126">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="81207-127">Use a API gerenciada de EWS [classe de compromisso](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou o elemento do EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) para trabalhar com compromissos e reuniões.</span><span class="sxs-lookup"><span data-stu-id="81207-127">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="81207-128">Compromissos e reuniões podem ser instâncias única ou parte de uma [série recorrente](recurrence-patterns-and-ews.md), mas como compromissos não incluem os participantes, salas ou recursos, eles não exigem uma mensagem a ser enviada.</span><span class="sxs-lookup"><span data-stu-id="81207-128">Both appointments and meetings can be single instances or part of a [recurring series](recurrence-patterns-and-ews.md), but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span>
  
<span data-ttu-id="81207-129">Como reuniões incluem o envio e responder às solicitações e atualizações, eles envolvem acessando mais do que apenas os itens em uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="81207-129">Because meetings include sending and responding to requests and updates, they involve more than just accessing items in a Calendar folder.</span></span> <span data-ttu-id="81207-130">Eles também têm um fluxo de trabalho associado.</span><span class="sxs-lookup"><span data-stu-id="81207-130">They also have an associated workflow.</span></span> <span data-ttu-id="81207-131">Reuniões devem ser agendados quando os participantes estão disponíveis e também podem envolver reservar uma sala de reunião ou recursos como um projetor ou outros equipamentos.</span><span class="sxs-lookup"><span data-stu-id="81207-131">Meetings must be scheduled when attendees are available, and can also involve reserving a meeting room, or resources such as a projector or other equipment.</span></span>
  
<span data-ttu-id="81207-132">O fluxo de trabalho de reunião geralmente envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="81207-132">The meeting workflow typically involves the following steps:</span></span>
  
1. <span data-ttu-id="81207-133">Uma reunião é criada e preenchida com informações como início e hora de término, local e corpo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="81207-133">A meeting is created and populated with information such as start and end time, location, and a message body.</span></span>
    
2. <span data-ttu-id="81207-134">Uma lista de participantes em potencial, recursos e salas é criada.</span><span class="sxs-lookup"><span data-stu-id="81207-134">A list of prospective attendees, resources, and rooms is created.</span></span>
    
3. <span data-ttu-id="81207-135">O status de disponibilidade dos participantes é verificado.</span><span class="sxs-lookup"><span data-stu-id="81207-135">The availability status of attendees is checked.</span></span> 
    
4. <span data-ttu-id="81207-136">Uma solicitação de reunião é enviada aos participantes.</span><span class="sxs-lookup"><span data-stu-id="81207-136">A meeting request is sent to attendees.</span></span>
    
5. <span data-ttu-id="81207-137">Participantes respondam à solicitação de reunião com seu intenção participar ou não.</span><span class="sxs-lookup"><span data-stu-id="81207-137">Attendees reply to the meeting with their intention to attend or not.</span></span> <span data-ttu-id="81207-138">Os participantes também podem propor um novo horário para a reunião.</span><span class="sxs-lookup"><span data-stu-id="81207-138">Attendees may also propose a new time for the meeting.</span></span>
    
6. <span data-ttu-id="81207-139">Reuniões podem ser cancelados ou atualizados, que normalmente acionam novas mensagens sejam enviadas aos participantes.</span><span class="sxs-lookup"><span data-stu-id="81207-139">Meetings can be canceled or updated, which typically trigger new messages to be sent to attendees.</span></span>
    
## <a name="calendars-and-time"></a><span data-ttu-id="81207-140">Calendários e hora</span><span class="sxs-lookup"><span data-stu-id="81207-140">Calendars and time</span></span>
<span data-ttu-id="81207-141"><a name="bk_Time"> </a></span><span class="sxs-lookup"><span data-stu-id="81207-141"></span></span>

<span data-ttu-id="81207-142">Funcionalidade de tempo é parte do calendário.</span><span class="sxs-lookup"><span data-stu-id="81207-142">Time-related functionality is integral to calendaring.</span></span> <span data-ttu-id="81207-143">Compromissos e reuniões tem início e término, durações e outras propriedades relacionadas ao tempo, como a hora em que uma mensagem é criada, enviada e recebida.</span><span class="sxs-lookup"><span data-stu-id="81207-143">Appointments and meetings have start and end times, durations, and other time-related properties, such as the time at which a message is created, sent, and received.</span></span> <span data-ttu-id="81207-144">Reuniões e compromissos existentes podem ser recuperadas de uma pasta de calendário com base em uma hora de início e término.</span><span class="sxs-lookup"><span data-stu-id="81207-144">Existing appointments and meetings can be retrieved from a Calendar folder based on a start and end time.</span></span> <span data-ttu-id="81207-145">Série recorrente tem inícios e terminará.</span><span class="sxs-lookup"><span data-stu-id="81207-145">Recurring series have beginnings and ends.</span></span> <span data-ttu-id="81207-146">E reuniões ocorrerem em uma zona de tempo determinada, que é cada vez mais importante em uma economia global.</span><span class="sxs-lookup"><span data-stu-id="81207-146">And meetings occur within a given time zone, which is increasingly important in a global economy.</span></span>
  
<span data-ttu-id="81207-147">Horas são armazenadas internamente em um servidor do Exchange no tempo Universal Coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="81207-147">Times are stored internally on an Exchange server in Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="81207-148">Exchange converte-los para o fuso horário local com base nas configurações de cliente.</span><span class="sxs-lookup"><span data-stu-id="81207-148">Exchange converts them to local time zone based on client settings.</span></span> <span data-ttu-id="81207-149">Propriedades de [DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) limitam-se à zona de hora local do computador.</span><span class="sxs-lookup"><span data-stu-id="81207-149">[DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) properties are scoped to the computer's local time zone.</span></span> 
  
## <a name="recurring-series"></a><span data-ttu-id="81207-150">Série recorrente</span><span class="sxs-lookup"><span data-stu-id="81207-150">Recurring series</span></span>
<span data-ttu-id="81207-151"><a name="bk_recurrence"> </a></span><span class="sxs-lookup"><span data-stu-id="81207-151"></span></span>

<span data-ttu-id="81207-152">Uma série recorrente de compromissos ou reuniões é composta de um mestre recorrente, um conjunto de itens de ocorrência e, opcionalmente, um conjunto de itens de exceção.</span><span class="sxs-lookup"><span data-stu-id="81207-152">A recurring series of appointments or meetings is comprised of a recurring master, a set of occurrence items, and optionally, a set of exception items.</span></span> <span data-ttu-id="81207-153">Informações de recorrência são armazenadas no item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="81207-153">Recurrence information is stored on the recurring master item.</span></span> <span data-ttu-id="81207-154">O elemento EWS [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) é associado a ocorrências e exceções em uma série ou você pode usar o método [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/pt-br/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API para obter o recorrente mestre.</span><span class="sxs-lookup"><span data-stu-id="81207-154">The [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS element is associated with occurrences and exceptions in a series, or you can use the [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/pt-br/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API method to get the recurring master.</span></span> <span data-ttu-id="81207-155">Usando uma instância de uma série, você pode encontrar todos os elementos e informações associadas a série.</span><span class="sxs-lookup"><span data-stu-id="81207-155">Using an instance of a series, you can find all the elements and information associated with the series.</span></span> 
  
<span data-ttu-id="81207-156">Observe que as propriedades de recorrência existirem em todos os itens de calendário, mas eles são preenchidos somente em itens recorrentes de mestres.</span><span class="sxs-lookup"><span data-stu-id="81207-156">Note that recurrence properties exist on all calendar items, but they are populated only on recurring master items.</span></span> <span data-ttu-id="81207-157">Além de um índice de todas as ocorrências de uma série, o mestre recorrente tem uma referência ao ocorrências excluídas e modificadas e o padrão de recorrência de uma série (por exemplo, diariamente, semanalmente, mensalmente ou anualmente).</span><span class="sxs-lookup"><span data-stu-id="81207-157">In addition to an index of all occurrences in a series, the recurring master has a reference to modified and deleted occurrences and the recurrence pattern of a series (for example, daily, weekly, monthly, or yearly).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="81207-158">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="81207-158">In this section</span></span>
<span data-ttu-id="81207-159"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="81207-159"></span></span>

- [<span data-ttu-id="81207-160">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="81207-160">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="81207-161">Criar eventos de dia inteiro usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-161">Create all-day events by using EWS in Exchange</span></span>](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-162">Obtenha os compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-163">Atualizar compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-164">Excluir compromissos e cancelar reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-165">Obter listas de sala, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-165">Get room lists by using EWS in Exchange</span></span>](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-166">Obter informações de disponibilidade usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-166">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-167">Propor um novo horário de reunião usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-167">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81207-168">Processar itens de calendário em lotes no Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-168">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [<span data-ttu-id="81207-169">Padrões de recorrência e EWS</span><span class="sxs-lookup"><span data-stu-id="81207-169">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a><span data-ttu-id="81207-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="81207-170">See also</span></span>


- [<span data-ttu-id="81207-171">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="81207-172">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-172">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="81207-173">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="81207-173">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

