---
title: Criar eventos de dia inteiro usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Saiba como criar eventos de dia inteiro usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 0547fdf0ca92ba0648caeb5de6940d90d2a8ff46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750699"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Criar eventos de dia inteiro usando o EWS no Exchange

Saiba como criar eventos de dia inteiro usando a API gerenciada de EWS ou EWS no Exchange.
  
Eventos de dia inteiro fornecem uma maneira para representar algo que acontece para um dia inteiro ou vários dias — por exemplo, um feriado ou dias de férias. Criar eventos de dia inteiro com a API gerenciada de EWS ou o EWS é muito fácil. É como [a criação de compromissos](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mas com algumas pequenas alterações.
  
## <a name="setting-start-and-end-times"></a>Definindo os horários de início e término

Por definição, os eventos de dia inteiro iniciar à meia-noite em um determinado dia e end 24 horas (ou um múltiplo de 24 horas) posteriormente. No entanto, a API gerenciada de EWS e EWS permitem especificar horários que não seja a meia-noite ao criar eventos de dia inteiro. Isso pode levar à comportamento acidentais se não ter ciência de como esses horários obtém convertidos no servidor.
  
Quando uma solicitação for recebida para criar um novo evento de dia inteiro com o início de não-meia-noite (na [zona de tempo da solicitação ou compromisso](time-zones-and-ews-in-exchange.md)) e/ou de término, esses horários obtém ajustados para meia-noite no fuso horário apropriado conforme as regras a seguintes:
  
- Horas de início de não-meia-noite são ajustadas para a meia-noite antes da hora especificada. Por exemplo, 1:00 PM em 6 de junho obtém ajustada para 12:00 AM em 6 de junho.
    
- Encerramento de não-meia-noite é ajustados para a meia-noite após o tempo especificado. Por exemplo, 1:00 PM em 6 de junho obtém ajustada para 12:00 AM em 7 de junho.
    
Portanto, o evento de dia inteiro que você criar é sempre inclui a hora de início e término que você especifica, mas talvez mais tempo de declaração no usuário do calendário devido à mudança para a meia-noite. Porque o servidor irá ajustar a hora de início e término para meia-noite, recomendamos que você especifique seu horário de início e término à meia-noite para evitar quaisquer alterações indesejadas para os horários.
  
Também é importante considerar os fusos horários ao criar eventos de dia inteiro. Como o Exchange server impõe um meia-noite início e hora no fuso horário do compromisso ou solicitação de término, exibindo desse evento de dia inteiro em um cliente configurado para um fuso horário diferente pode gerar resultados inesperados. Dependendo do cliente, ele pode ser exibido como um evento de dia inteiro com dias adicionais que você não pretende incluir ou ela pode não aparecer como um evento de dia inteiro todo. Por isso, é recomendável que você use fuso de horário preferencial do usuário sempre que possível, quando você criar eventos de dia inteiro.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Criar um evento de dia inteiro usando a API gerenciada de EWS

O exemplo a seguir mostra como usar a API gerenciada de EWS para criar um evento de dia inteiro, começando na data especificada pelo parâmetro _startDate_ e que dura para o número de dias especificado pelo parâmetro _numDays_ . Observe que o compromisso será criado no fuso horário especificado pela propriedade [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Este exemplo pressupõe que o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) passado no parâmetro _serviço_ foi inicializado com os valores válidos para as propriedades de [credenciais](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
```cs
static void CreateAllDayAppointment(ExchangeService service, DateTime startDate, int numDays)
{
    // Best practice is to set the start date to midnight
    // on the first day of the all-day event.
    DateTime startDateMidnight = startDate.Date;
    // The end date should be midnight on the first day
    // after the event.
    DateTime endDateMidnight = startDateMidnight.AddDays(numDays);
    Appointment allDayEvent = new Appointment(service);
    // Set IsAllDayEvent to true.
    allDayEvent.IsAllDayEvent = true;
    // Set other properties.
    allDayEvent.Subject = "Vacation";
    allDayEvent.LegacyFreeBusyStatus = LegacyFreeBusyStatus.OOF;
    allDayEvent.Start = startDateMidnight;
    allDayEvent.End = endDateMidnight;
    // Save the appointment.
    try
    {
        allDayEvent.Save(WellKnownFolderName.Calendar, SendInvitationsMode.SendToNone);
        Console.WriteLine("All day event created.");
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving all day event: {0}", ex.Message);
    }
}
```

## <a name="create-an-all-day-event-by-using-ews"></a>Criar um evento de dia inteiro usando o EWS

O exemplo a seguir mostra uma solicitação EWS [operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar um evento de dia inteiro. O compromisso é criado no fuso horário do Leste, conforme indicado pelo elemento [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) . Observe que a parte de tempo dos valores dos elementos [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) estão ambas 04:00Z, que converte a meia-noite no fuso horário do Leste durante o horário de verão. 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Vacation</t:Subject>
          <t:Start>2014-06-09T04:00:00.000Z</t:Start>
          <t:End>2014-06-10T04:00:00.000Z</t:End>
          <t:IsAllDayEvent>true</t:IsAllDayEvent>
          <t:LegacyFreeBusyStatus>OOF</t:LegacyFreeBusyStatus>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Fusos horários e EWS no Exchange](time-zones-and-ews-in-exchange.md)
    

