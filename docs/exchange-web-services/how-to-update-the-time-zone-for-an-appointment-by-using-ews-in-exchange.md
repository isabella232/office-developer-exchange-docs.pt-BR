---
title: Atualizar o fuso horário para um compromisso usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Saiba como atualizar o fuso horário para uma reunião ou compromisso existente usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 535eb9f546d9a4353408579f3a24750f32237699
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750836"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a><span data-ttu-id="33a11-103">Atualizar o fuso horário para um compromisso usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="33a11-103">Update the time zone for an appointment by using EWS in Exchange</span></span>

<span data-ttu-id="33a11-104">Saiba como atualizar o fuso horário para uma reunião ou compromisso existente usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="33a11-104">Learn how to update the time zone for an existing appointment or meeting by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="33a11-105">Quando um compromisso ou reunião é criado em um calendário do Exchange, o fuso horário usado para especificar os horários de início e término é salvo como o fuso horário de criação para o compromisso.</span><span class="sxs-lookup"><span data-stu-id="33a11-105">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment.</span></span> <span data-ttu-id="33a11-106">Você pode alterar o fuso horário correspondente usando a API gerenciada de EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="33a11-106">You can change that time zone by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="33a11-107">No entanto, a alteração do fuso horário em um compromisso tem outros efeitos sobre a hora de início e término do compromisso.</span><span class="sxs-lookup"><span data-stu-id="33a11-107">However, changing the time zone on an appointment has other effects on the start and end time of the appointment.</span></span>
  
<span data-ttu-id="33a11-108">Valores de hora são armazenados no servidor do Exchange em coordene UTC (Tempo Universal).</span><span class="sxs-lookup"><span data-stu-id="33a11-108">Time values are stored on the Exchange server in Coordinate Universal Time (UTC).</span></span> <span data-ttu-id="33a11-109">Portanto, se um compromisso for definido como começar às 13:00 (13:00) no fuso horário do Leste (UTC-05:00), que o valor é armazenado como 6:00 PM (18:00) no servidor, supondo que o fuso horário esteja em sua fase de hora padrão.</span><span class="sxs-lookup"><span data-stu-id="33a11-109">So if an appointment is set to start at 1:00 PM (13:00) in the Eastern time zone (UTC-05:00), that value is stored as 6:00 PM (18:00) on the server, assuming that the time zone is in its standard time phase.</span></span> <span data-ttu-id="33a11-110">Quando esse compromisso for exibido em outros fusos horários, o número apropriado de horas é adicionado ou subtraído do valor para determinar o tempo específicas do fuso horário UTC.</span><span class="sxs-lookup"><span data-stu-id="33a11-110">When that appointment is viewed in other time zones, the appropriate number of hours is added or subtracted from the UTC value to determine the time zone-specific time.</span></span> <span data-ttu-id="33a11-111">Por exemplo, se um compromisso tem uma hora de início às 13:00 Leste (6:00 PM UTC) e é visualizado a partir de um cliente no fuso horário do Pacífico (UTC-08:00), específicos do fuso horário hora de início para que o cliente seria 10:00 AM (18:00-08:00).</span><span class="sxs-lookup"><span data-stu-id="33a11-111">For example, if an appointment has a start time at 1:00 PM Eastern (6:00 PM UTC), and is viewed from a client in the Pacific time zone (UTC-08:00), the time-zone specific start time for that client would be 10:00 AM (18:00 - 08:00).</span></span>
  
<span data-ttu-id="33a11-112">Quando você atualiza o fuso horário do compromisso sem atualizar a hora de início e término, o servidor atualiza os valores de UTC armazenados no servidor para manter a hora de início e término como os tempos de fuso horário específico mesmos.</span><span class="sxs-lookup"><span data-stu-id="33a11-112">When you update the time zone of the appointment without updating the start and end time, the server updates the UTC values stored on the server to keep the start and end time as the same time zone-specific times.</span></span> <span data-ttu-id="33a11-113">Por exemplo, considere o compromisso de 1:00 PM do Leste.</span><span class="sxs-lookup"><span data-stu-id="33a11-113">For example, consider the 1:00 PM Eastern appointment.</span></span> <span data-ttu-id="33a11-114">O tempo é armazenado como 18:00 UTC no servidor.</span><span class="sxs-lookup"><span data-stu-id="33a11-114">The time is stored as 18:00 UTC on the server.</span></span> <span data-ttu-id="33a11-115">Se o fuso horário do compromisso for alterado para o fuso horário do Pacífico, o servidor desloca a hora de início para 1:00 PM Pacífico (UTC 21:00).</span><span class="sxs-lookup"><span data-stu-id="33a11-115">If the time zone of the appointment is changed to the Pacific time zone, the server shifts the start time to 1:00 PM Pacific (21:00 UTC).</span></span>
  
<span data-ttu-id="33a11-116">Você pode alterar esse comportamento, definindo explicitamente os horários de início e término.</span><span class="sxs-lookup"><span data-stu-id="33a11-116">You can change this behavior by explicitly setting the start and end times.</span></span>
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="33a11-117">Atualizando o fuso horário em um compromisso existente usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="33a11-117">Updating the time zone on an existing appointment by using the EWS Managed API</span></span>

<span data-ttu-id="33a11-118">No exemplo a seguir, a API gerenciada de EWS é usada para atualizar o fuso horário em um compromisso existente para o fuso horário Central atualizando os **Appointment.StartTimeZone** e as propriedades de **Appointment.EndTimeZone** .</span><span class="sxs-lookup"><span data-stu-id="33a11-118">In the following example, the EWS Managed API is used to update the time zone on an existing appointment to the Central time zone by updating the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="33a11-119">Se o parâmetro _shiftAppointnment_ é definido como **true**, o código não definir explicitamente os horários de início e término no compromisso.</span><span class="sxs-lookup"><span data-stu-id="33a11-119">If the  _shiftAppointnment_ parameter is set to **true**, the code does not explicitly set the start and end times on the appointment.</span></span> <span data-ttu-id="33a11-120">Nesse caso, o servidor mudará os horários de início e término para mantê-los nos momentos mesmos relativa de fuso horário no novo fuso horário.</span><span class="sxs-lookup"><span data-stu-id="33a11-120">In this case, the server will shift the start and end times to keep them at the same time zone-relative times in the new time zone.</span></span> <span data-ttu-id="33a11-121">Se definido como **false**, o código converte os horários de início e término explicitamente para manter o compromisso ao mesmo tempo em UTC.</span><span class="sxs-lookup"><span data-stu-id="33a11-121">If set to **false**, the code converts the start and end times explicitly to keep the appointment at the same time in UTC.</span></span> 

<span data-ttu-id="33a11-122">Este exemplo pressupõe que o objeto **ExchangeService** foi inicializado com valores válidos nas propriedades [credenciais](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="33a11-122">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void UpdateAppointmentTimeZone(ExchangeService service, ItemId apptId, bool shiftAppointment)
{
    PropertySet includeTimeZones = new PropertySet(AppointmentSchema.Subject,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.ReminderDueBy,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.StartTimeZone,
                                                   AppointmentSchema.EndTimeZone);
    Appointment apptToUpdate;
    // Load the existing appointment.
    // This will result in a call to EWS.
    try
    {
        apptToUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("Before update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptToUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptToUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptToUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptToUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptToUpdate.EndTimeZone.DisplayName);
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Update the time zones on the appointment.
    apptToUpdate.StartTimeZone = centralTZ;
    apptToUpdate.EndTimeZone = centralTZ;
    if (!shiftAppointment)
    {
        // Set the start and end times explicitly so that the appointment
        // will start and end at the same UTC time.
        // Convert the times to then Central time zone. This
        // will keep them at the same time in UTC.
        // For example, 1:00 PM Eastern becomes 12:00 PM Central.
        DateTime newStartTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.Start, centralTZ);
        DateTime newEndTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.End, centralTZ);
        apptToUpdate.Start = newStartTime;
        apptToUpdate.End = newEndTime;
    }
    try
    {
        // Save the changes. This will result in a call to EWS.
        apptToUpdate.Update(ConflictResolutionMode.AlwaysOverwrite, 
            SendInvitationsOrCancellationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error updating appointment: {0}", ex.Message);
        return;
    }
    // Now rebind to the appointment to get the new values.
    Appointment apptAfterUpdate;
    
    try
    {
        // This will result in a call to EWS.
        apptAfterUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("After update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptAfterUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptAfterUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptAfterUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptAfterUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptAfterUpdate.EndTimeZone.DisplayName);
}
```

<span data-ttu-id="33a11-123">Quando o exemplo é usado para atualizar um compromisso que começa às 13:00 Leste e terminará às 2:00 PM Leste, com o parâmetro _shiftAppointment_ definido como true e a propriedade [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) definida como o fuso horário do Leste, a saída se parece semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="33a11-123">When the example is used to update an appointment that starts at 1:00 PM Eastern and ends at 2:00 PM Eastern, with the  _shiftAppointment_ parameter set to true, and the [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property set to the Eastern time zone, the output looks like the following.</span></span> 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 2:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 2:00:00 PM
  End: 6/20/2014 3:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

<span data-ttu-id="33a11-124">Quando o exemplo é usado para atualizar o mesmo compromisso com o parâmetro _shiftAppointment_ definido como false e com a propriedade de **fuso horário** novamente definida para o fuso horário do Leste, a saída se parece um pouco diferente.</span><span class="sxs-lookup"><span data-stu-id="33a11-124">When the example is used to update the same appointment with the  _shiftAppointment_ parameter set to false, and with the **TimeZone** property again set to the Eastern time zone, the output looks a little different.</span></span> 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

<span data-ttu-id="33a11-125">Observe que os horários de início e término não foram alterado.</span><span class="sxs-lookup"><span data-stu-id="33a11-125">Notice that the start and end times did not change.</span></span> <span data-ttu-id="33a11-126">Isso ocorre porque os tempos são interpretados no tempo do Leste (porque a propriedade **TimeZone** está definida para o fuso horário do Leste) de zona, e os valores de hora foram atualizados para impedir que o compromisso da mudança.</span><span class="sxs-lookup"><span data-stu-id="33a11-126">This is because the times are being interpreted in the Eastern time zone (because the **TimeZone** property is set to the Eastern time zone), and the time values were updated to prevent the appointment from shifting.</span></span> 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a><span data-ttu-id="33a11-127">Atualizando o fuso horário em um compromisso existente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="33a11-127">Updating the time zone on an existing appointment by using EWS</span></span>

<span data-ttu-id="33a11-128">A solicitação EWS [UpdateItem operação](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) exemplo a seguir atualiza o fuso horário em um compromisso.</span><span class="sxs-lookup"><span data-stu-id="33a11-128">The following example EWS [UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) request updates the time zone on an appointment.</span></span> <span data-ttu-id="33a11-129">Este exemplo atualiza apenas os elementos [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) e [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) , para que o servidor mudará os horários de início e término do compromisso mantê-la ao mesmo tempo relativa de fuso horário no novo fuso horário.</span><span class="sxs-lookup"><span data-stu-id="33a11-129">This example only updates the [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements, so the server will shift the start and end times of the appointment to keep it at the same time-zone-relative time in the new time zone.</span></span> <span data-ttu-id="33a11-130">O valor do elemento **ItemId** é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="33a11-130">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="33a11-131">A solicitação de exemplo a seguir atualiza o fuso horário do compromisso e também atualiza os horários de início e término, definindo explicitamente os elementos **Start** e **End** .</span><span class="sxs-lookup"><span data-stu-id="33a11-131">The following example request updates the time zone of the appointment, and also updates the start and end times by explicitly setting the **Start** and **End** elements.</span></span> <span data-ttu-id="33a11-132">O valor do elemento **ItemId** é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="33a11-132">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-06-20T17:00:00.000Z</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-06-20T18:00:00.000Z</t:End>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="33a11-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="33a11-133">See also</span></span>

- [<span data-ttu-id="33a11-134">Fusos horários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="33a11-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)   
- [<span data-ttu-id="33a11-135">Criar compromissos em um fuso horário específico usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="33a11-135">Create appointments in a specific time zone by using EWS in Exchange</span></span>](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="33a11-136">Atualizar compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="33a11-136">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

