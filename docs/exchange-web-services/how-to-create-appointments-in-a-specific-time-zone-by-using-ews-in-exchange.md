---
title: Criar compromissos em um fuso horário específico usando o EWS em Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Saiba como criar compromissos em fusos horário específicos usando a API Gerenciada do EWS ou o EWS Exchange.
ms.openlocfilehash: 589c72982fdda568170468c376b8a6d9f598aa36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521141"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Criar compromissos em um fuso horário específico usando o EWS em Exchange

Saiba como criar compromissos em fusos horário específicos usando a API Gerenciada do EWS ou o EWS Exchange.
  
Quando um compromisso ou reunião é criado em um calendário Exchange, o fuso horário usado para especificar os horários de início e término é salvo como o fuso horário de criação do compromisso. Esse fuso horário também é usado para interpretar valores de data e hora que não têm um fuso horário explícito [especificado,](time-zones-and-ews-in-exchange.md)portanto, é importante entender suas opções para especificar o fuso horário.
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>Criar compromissos em fusos horário diferentes usando a API Gerenciada do EWS

Ao criar compromissos ou reuniões usando a API Gerenciada do EWS, você tem três opções para especificar o fuso horário:
  
- Para usar o fuso horário do computador onde sua API Gerenciada do EWS está sendo executada, não especifique um fuso horário ao criar o [objeto ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) 
    
- Para usar um fuso horário específico para todas as propriedades de data/hora, incluindo propriedades ao criar um novo compromisso ou reunião, especifique um fuso horário no construtor do **objeto ExchangeService.** 
    
- Para usar um fuso horário diferente do especificado na propriedade [ExchangeService.TimeZone,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) use as propriedades [Appointment.StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) e [Appointment.EndTimeZone.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) 
    
    > [!NOTE]
    > A **propriedade EndTimeZone** só estará disponível quando a [propriedade ExchangeService.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) estiver definida como **Exchange2010** ou posterior. Se não estiver disponível, a definição do **StartTimeZone** se aplica aos horários de início e término do compromisso. 
  
No exemplo a seguir, a API Gerenciada do EWS é usada para criar três compromissos. Cada compromisso está definido para começar às 13:00, daqui a dois dias, em um fuso horário não especificado e termina uma hora depois. O primeiro compromisso é criado no fuso horário do computador cliente usando o comportamento padrão da API Gerenciada do EWS. O segundo é criado no fuso horário Central usando as **propriedades Appointment.StartTimeZone** e **Appointment.EndTimeZone.** O terceiro é criado no fuso horário de Mountain usando a **propriedade ExchangeService.TimeZone.** 
  
```cs
using Microsoft.Exchange.WebServices.Data;
using System.Security;
static void CreateAppointments(string userEmail, SecureString userPass)
{
    // *****************************************************
    // Create an appointment using the client computer's time zone.
    // *****************************************************
    // Do not specify a time zone when creating the ExchangeService.
    ExchangeService clientTZService = new ExchangeService(ExchangeVersion.Exchange2010);
    clientTZService.Credentials = new NetworkCredential(userEmail, userPass);
    clientTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment clientTZAppt = new Appointment(clientTZService);
    clientTZAppt.Subject = "Appointment created using client time zone";
    clientTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", clientTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    DateTime startTime = new DateTime(DateTime.Now.Year, DateTime.Now.Month, DateTime.Now.Day + 2);
    startTime = startTime.AddHours(13);
    clientTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    DateTime endTime = startTime.AddHours(1);
    clientTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        clientTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Central time zone by
    // using the StartTimeZone property.
    // *****************************************************
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Create the appointment.
    Appointment centralTZAppt = new Appointment(clientTZService);
    centralTZAppt.Subject = "Appointment created using Central time zone";
    centralTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", centralTZ.DisplayName));
    // Set the time zone on the appointment.
    centralTZAppt.StartTimeZone = centralTZ;
    centralTZAppt.EndTimeZone = centralTZ;
    // Set the start time to 1:00 PM two days from today.
    centralTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    centralTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        centralTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Mountain time zone by
    // using the ExchangeService.TimeZone property.
    // *****************************************************
    // Specify the Mountain time zone when creating the ExchangeService.
    TimeZoneInfo mountainTZ = TimeZoneInfo.FindSystemTimeZoneById("Mountain Standard Time");
    ExchangeService mountainTZService = new ExchangeService(ExchangeVersion.Exchange2010, mountainTZ);
    mountainTZService.Credentials = new NetworkCredential(userEmail, userPass);
    mountainTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment mountainTZAppt = new Appointment(mountainTZService);
    mountainTZAppt.Subject = "Appointment created using Mountain time zone";
    mountainTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", mountainTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    mountainTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    mountainTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        mountainTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
}
```

Quando este exemplo é executado em um computador cliente configurado no fuso horário do Leste e os três compromissos que ele cria são exibidos de um cliente configurado no fuso horário do Leste, eles aparecem às 13:00, 14:00 e 15:00, respectivamente.
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a>Criar compromissos em fusos horário diferentes usando o EWS

Ao criar compromissos ou reuniões usando o EWS, você tem três opções para especificar o fuso horário:
  
- Para usar o UTC (Tempo Universal Coordenado), não inclua um elemento [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) o [elemento MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (somente Exchange 2007) ou os elementos [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) e [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 e posteriores) na solicitação de operação [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
- Para usar um fuso horário específico para todas as propriedades de data/hora, incluindo propriedades ao criar um novo compromisso ou reunião, especifique um fuso horário no elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) na solicitação de operação [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
- Para usar um fuso horário diferente do especificado no elemento [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) inclua um elemento [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) o elemento [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (somente Exchange 2007) ou os elementos [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) e [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 e posterior) na solicitação de operação [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
O exemplo a seguir [Solicitação de operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) cria um compromisso usando UTC. Observe que o **elemento TimeZoneContext,** o **elemento StartTimeZone** e o **elemento EndTimeZone** estão ausentes. Os **valores dos** elementos Start e **End** são expressos em UTC. 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using UTC</t:Subject>
          <t:Body BodyType="HTML">Time zone: UTC</t:Body>
          <t:Start>2014-06-07T17:00:00.000Z</t:Start>
          <t:End>2014-06-07T18:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir [Solicitação de operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) usa os **elementos StartTimeZone** e **EndTimeZone** para especificar o fuso horário Central do compromisso. Observe que o **elemento TimeZoneContext** está ausente. No entanto, se estivesse presente, os valores dos elementos **StartTimeZone** e **EndTimeZone** substituiriam seu valor. Novamente, os **valores dos** elementos Start **e End** são expressos em UTC. 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Central time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-06:00) Central Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T18:00:00.000Z</t:Start>
          <t:End>2014-06-07T19:00:00.000Z</t:End>
          <t:StartTimeZone Id="Central Standard Time" />
          <t:EndTimeZone Id="Central Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir [a solicitação de operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) define o **elemento TimeZoneContext** como o fuso horário de Mountain. Observe que os **elementos StartTimeZone** **e EndTimeZone** estão ausentes. Novamente, os **valores dos** elementos Start **e End** são expressos em UTC. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Mountain Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Mountain time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-07:00) Mountain Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T19:00:00.000Z</t:Start>
          <t:End>2014-06-07T20:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Quando os três compromissos criados pelas solicitações de exemplo anteriores do EWS são exibidos de um cliente configurado no fuso horário do Leste, eles aparecem às 13:00, 14:00 e 15:00, respectivamente.
  
## 

Agora que você sabe como criar compromissos em fusos horário específicos, talvez você queira atualizar os fusos horário [em compromissos existentes](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) para outro. 
  
## <a name="see-also"></a>Confira também


- [Fuso horário e EWS no Exchange](time-zones-and-ews-in-exchange.md)
    
- [Atualize o fuso horário para um compromisso usando o EWS no Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

