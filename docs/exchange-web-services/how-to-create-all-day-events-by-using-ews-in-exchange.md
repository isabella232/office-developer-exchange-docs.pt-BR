---
title: Criar eventos de todos os dias usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Saiba como criar eventos de dia inteiro usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 8769999907df46f519355a36fdf409f9ad347330
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521218"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Criar eventos de todos os dias usando o EWS no Exchange

Saiba como criar eventos de dia inteiro usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Os eventos de todos os dias fornecem uma maneira de representar algo que acontece por um dia inteiro ou vários dias, por exemplo, feriados ou dias de férias. Criar eventos de todos os dias com a API Gerenciada do EWS ou o EWS é um snap. É como criar [compromissos](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mas com algumas pequenas alterações.
  
## <a name="setting-start-and-end-times"></a>Definindo horários de início e término

Por definição, os eventos de todo o dia começam à meia-noite em um dia específico e terminam 24 horas (ou várias de 24 horas) mais tarde. No entanto, a API Gerenciada EWS e o EWS permitem que você especifique horários diferentes da meia-noite ao criar eventos de todos os dias. Isso pode levar a um comportamento não intencional se você não estiver ciente de como essas horas são traduzidas no servidor.
  
Quando uma solicitação é recebida para criar um novo evento de todo o dia com horário não-meia-noite (no fuso horário da solicitação ou do compromisso [)](time-zones-and-ews-in-exchange.md)inicia e/ou termina, esses horários são ajustados à meia-noite no fuso horário apropriado de acordo com as seguintes regras:
  
- Os horários de início não meia-noite são ajustados à meia-noite antes da hora especificada. Por exemplo, 13:00 de 6 de junho é ajustada para 00:00 de 6 de junho.
    
- Os horários de término não meia-noite são ajustados à meia-noite após o horário especificado. Por exemplo, 13:00 de 6 de junho é ajustada para 00:00 em 7 de junho.
    
Portanto, o evento de todos os dias que você cria é sempre inclusivo da hora inicial e de término que você especificar, mas pode reivindicar tempo adicional no calendário do usuário devido à mudança para a meia-noite. Como o servidor ajustará a hora de início e término à meia-noite, recomendamos que você especifique seu horário de início e término à meia-noite para evitar alterações não intencionais nos horários.
  
Também é importante considerar fusos horário ao criar eventos de todos os dias. Como o servidor exchange impõe uma hora de início e término da meia-noite no fuso horário da solicitação ou do compromisso, a exibição desse evento o dia todo em um cliente configurado para um fuso horário diferente pode gerar resultados inesperados. Dependendo do cliente, ele pode aparecer como um evento de todo o dia com dias extras que você não pretende incluir, ou pode não aparecer como um evento de todo o dia. Por isso, recomendamos que você use o fuso horário preferencial do usuário sempre que possível ao criar eventos de dia inteiro.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Criar um evento de dia inteiro usando a API Gerenciada do EWS

O exemplo a seguir mostra como usar a API Gerenciada do EWS para criar um evento de dia inteiro, começando na data especificada pelo parâmetro _startDate_ e durando o número de dias especificado pelo parâmetro _numDays._ Observe que o compromisso será criado no fuso horário especificado pela [propriedade ExchangeService.TimeZone.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) Este exemplo pressupõe que o [objeto ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) passado no parâmetro _de_ serviço tenha sido inicializado com valores válidos para as propriedades [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) 
  
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

O exemplo a seguir mostra uma solicitação de operação [CreateItem do](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS para criar um evento de dia inteiro. O compromisso é criado no fuso horário do Leste, conforme indicado pelo [elemento TimeZoneContext.](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) Observe que a parte de hora dos valores dos elementos [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) é 04:00Z, que se converte à meia-noite no fuso horário do Leste durante o horário de verão. 
  
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
    
- [Fuso horário e EWS no Exchange](time-zones-and-ews-in-exchange.md)
    

