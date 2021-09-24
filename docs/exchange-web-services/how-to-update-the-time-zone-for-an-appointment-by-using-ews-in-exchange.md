---
title: Atualize o fuso horário para um compromisso usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Saiba como atualizar o fuso horário de um compromisso ou reunião existente usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 525feb1c7e37914ef4105312e89af8f1a8cf856b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521064"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a>Atualize o fuso horário para um compromisso usando o EWS no Exchange

Saiba como atualizar o fuso horário de um compromisso ou reunião existente usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Quando um compromisso ou reunião é criado em um calendário Exchange, o fuso horário usado para especificar os horários de início e término é salvo como o fuso horário de criação do compromisso. Você pode alterar esse fuso horário usando a API Gerenciada do EWS ou o EWS. No entanto, alterar o fuso horário em um compromisso tem outros efeitos no início e na hora de término do compromisso.
  
Os valores de tempo são armazenados no servidor Exchange em Tempo Universal de Coordenadas (UTC). Portanto, se um compromisso for definido para começar às 13:00 (13:00) no fuso horário leste (UTC-05:00), esse valor será armazenado como 18:00 (18:00) no servidor, pressupondo que o fuso horário está em sua fase de tempo padrão. Quando esse compromisso é exibido em outros fusos horários, o número apropriado de horas é adicionado ou subtraído do valor UTC para determinar o horário específico do fuso horário. Por exemplo, se um compromisso tiver uma hora de início às 13:00 HORAS leste (18:00 UTC) e for exibido de um cliente no fuso horário do Pacífico (UTC-08:00), o horário de início específico do fuso horário para esse cliente seria 10:00 (18:00 - 08:00).
  
Quando você atualiza o fuso horário do compromisso sem atualizar a hora inicial e de término, o servidor atualiza os valores UTC armazenados no servidor para manter a hora de início e término como os mesmos horários específicos do fuso horário. Por exemplo, considere o compromisso leste das 13:00. O tempo é armazenado como 18:00 UTC no servidor. Se o fuso horário do compromisso for alterado para o fuso horário do Pacífico, o servidor mudará o horário de início para 13:00 PACÍFICO (21:00 UTC).
  
Você pode alterar esse comportamento definindo explicitamente os horários de início e término.
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a>Atualizando o fuso horário em um compromisso existente usando a API Gerenciada do EWS

No exemplo a seguir, a API Gerenciada do EWS é usada para atualizar o fuso horário em um compromisso existente para o fuso horário Central atualizando as propriedades **Appointment.StartTimeZone** e **Appointment.EndTimeZone.** Se o  _parâmetro shiftAppointnment_ for definido como **true**, o código não definirá explicitamente os horários de início e término no compromisso. Nesse caso, o servidor deslocará os horários de início e término para mantê-los nos mesmos horários relativos ao fuso horário no novo fuso horário. Se definido como **false**, o código converte os horários de início e término explicitamente para manter o compromisso ao mesmo tempo em UTC. 

Este exemplo supõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). 
  
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

Quando o exemplo é usado para atualizar um compromisso que começa às 13:00 pm eastern e termina às 14:00 PM Eastern, com o parâmetro  _shiftAppointment_ definido como true e a propriedade [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) definida como o fuso horário leste, a saída se parece com o seguinte. 
  
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

Quando o exemplo é usado para atualizar o mesmo compromisso com o parâmetro  _shiftAppointment_ definido como false e com a propriedade **TimeZone** novamente definida como o fuso horário do Leste, a saída parece um pouco diferente. 
  
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

Observe que os horários de início e término não mudaram. Isso porque os horários estão sendo interpretados no fuso horário do Leste (porque a propriedade **TimeZone** está definida como o fuso horário do Leste) e os valores de hora foram atualizados para impedir que o compromisso seja deslocada. 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a>Atualizando o fuso horário em um compromisso existente usando o EWS

O exemplo a seguir A solicitação de operação [updateItem do](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS atualiza o fuso horário em um compromisso. Este exemplo apenas atualiza os elementos [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) e [EndTimeZone,](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) para que o servidor mude os horários de início e término do compromisso para mantê-lo no mesmo horário relativo ao fuso horário no novo fuso horário. O valor do **elemento ItemId** é reduzido para capacidade de leitura. 
  
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

A solicitação de exemplo a seguir atualiza o fuso horário do compromisso e também atualiza os horários de início e término definindo explicitamente os elementos **Start** e **End.** O valor do **elemento ItemId** é reduzido para capacidade de leitura. 
  
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

## <a name="see-also"></a>Confira também

- [Fuso horário e EWS no Exchange](time-zones-and-ews-in-exchange.md)   
- [Criar compromissos em um fuso horário específico usando o EWS em Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

