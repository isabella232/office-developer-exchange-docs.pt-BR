---
title: Criar eventos de dia inteiro usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Saiba como criar eventos de dia inteiro usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 6be638c17cc0e0c86fa6b4217169aa7259dfd4aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456861"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Criar eventos de dia inteiro usando o EWS no Exchange

Saiba como criar eventos de dia inteiro usando a API gerenciada do EWS ou o EWS no Exchange.
  
Os eventos de dia inteiro fornecem uma maneira de representar algo que acontece para um dia inteiro ou vários dias — por exemplo, um feriado ou dias de férias. Criar eventos de dia inteiro com a API gerenciada do EWS ou o EWS é um instantâneo. É como [criar compromissos](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mas com algumas pequenas alterações.
  
## <a name="setting-start-and-end-times"></a>Definir horários de início e término

Por definição, os eventos de dia inteiro começam à meia-noite em um dia específico e terminam 24 horas (ou um múltiplo de 24 horas) mais tarde. No entanto, a API gerenciada do EWS e o EWS permitem que você especifique horários diferentes da meia-noite ao criar eventos de dia inteiro. Isso pode levar a um comportamento inesperado se você não estiver ciente de como essas horas são traduzidas no servidor.
  
Quando uma solicitação é recebida para criar um novo evento de dia inteiro com não-meia-noite (no [fuso horário das horas de](time-zones-and-ews-in-exchange.md)início e/ou de término do compromisso), essas horas são ajustadas à meia-noite no fuso horário apropriado, de acordo com as seguintes regras:
  
- Horários de início sem meia-noite são ajustados à meia-noite antes do tempo especificado. Por exemplo, 1:00 PM em 6 de junho é ajustado para 12:00 AM 6 de junho.
    
- Horários de término sem meia-noite são ajustados à meia-noite após o tempo especificado. Por exemplo, 1:00 PM em 6 de junho é ajustado para 12:00 A.M. em 7 de junho.
    
Portanto, o evento de dia inteiro que você cria é sempre inclusivo da hora de início e de término que você especificar, mas pode solicitar tempo adicional no calendário do usuário devido à meia-noite. Como o servidor ajustará o tempo de início e de término à meia-noite, recomendamos que você especifique o horário de início e de término à meia-noite para evitar qualquer alteração não intencional nos horários.
  
Também é importante considerar os fusos horários ao criar eventos de dia inteiro. Como o Exchange Server impõe uma hora de início e de término da meia-noite no fuso horário da solicitação ou compromisso, a exibição desse evento de dia inteiro em um cliente configurado para um fuso horário diferente pode gerar resultados inesperados. Dependendo do cliente, ele pode aparecer como um evento de dia inteiro com dias extras que você não pretende incluir ou pode não aparecer como um evento de dia inteiro completamente. Por causa disso, recomendamos que você use o fuso horário preferencial do usuário sempre que possível ao criar eventos de dia inteiro.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Criar um evento de dia inteiro usando a API gerenciada do EWS

O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um evento de dia inteiro, começando na data especificada pelo parâmetro _StartDate_ e duradoura pelo número de dias especificado pelo parâmetro _numDays_ . Observe que o compromisso será criado no fuso horário especificado pela propriedade [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Este exemplo pressupõe que o objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) passado no parâmetro _Service_ tenha sido inicializado com valores válidos para as propriedades [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

O exemplo a seguir mostra uma solicitação de operação do EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar um evento de dia inteiro. O compromisso é criado no fuso horário da costa leste, conforme indicado pelo elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) . Observe que a parte de hora dos valores dos elementos [inicial](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [final](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) são 04:00Z, que converte para meia-noite no fuso horário da costa leste durante o horário de verão. 
  
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
    

