---
title: Criar uma série recorrente usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 88ed6e87-25f7-4a54-83fa-d757a0ff2528
description: Saiba como criar reuniões recorrentes usando a API Gerenciada do EWS ou o EWS Exchange.
ms.openlocfilehash: 58dfa821774a06db540ed734f616d28f663be53d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513224"
---
# <a name="create-a-recurring-series-by-using-ews-in-exchange"></a>Criar uma série recorrente usando o EWS no Exchange

Saiba como criar reuniões recorrentes usando a API Gerenciada do EWS ou o EWS Exchange.
  
Criar um compromisso ou reunião recorrente não é muito diferente de criar um compromisso ou reunião de instância [única.](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md) Você só precisa atribuir valores a algumas propriedades relacionadas à recorrência adicionais. Eles são definidos em um objeto [Recurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) do [objeto ExchangeService.Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) (se você estiver usando a API Gerenciada do EWS) ou o elemento filho [recorrência](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) de um [elemento CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) (se você estiver usando o EWS). Uma coisa a ser considerada ao criar uma reunião recorrente, em vez de uma única instância, é que o item de calendário criado é o mestre recorrente de uma série. Várias propriedades são definidas somente em um mestre recorrente; essas propriedades podem ajudá-lo a encontrar, modificar ou excluir instâncias individuais em uma série. Por esse motivo, pode ser útil manter o controle da ID do mestre recorrente ao criar uma série recorrente. 
  
**Tabela 1. Propriedades definidas em itens de calendário mestre recorrentes**

|**Classe ou propriedade da API Gerenciada do EWS**|**Elemento XML do EWS**|**Descrição**|
|:-----|:-----|:-----|
|[Classe Recurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) <br/> A **classe Recurrence** é a classe base de uma classe de padrão derivada, [IntervalPattern,](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx) [RelativeYearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx)ou [YearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx).  <br/> |[Recurrence (RecurrenceType)](https://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) <br/> |Contém informações relacionadas à recorrência, incluindo o padrão de recorrência (diariamente, semanal, mensal e assim por diante), data de início e término, número de ocorrências e assim por diante.  <br/> |
|[Propriedade FirstOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) <br/> |[FirstOccurrence](https://msdn.microsoft.com/library/d6748860-ce0d-4d2e-b7e4-9ed834f1e45a%28Office.15%29.aspx) <br/> |Contém os horários de início e término e a ID do item da primeira reunião de uma série.  <br/> |
|[Propriedade LastOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) <br/> |[LastOccurrence](https://msdn.microsoft.com/library/c9ef0fcb-4265-4e60-9986-fff0f211d00b%28Office.15%29.aspx) <br/> |Contém os horários de início e término e a ID do item da última reunião de uma série.  <br/> |
|[Propriedade ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) <br/> |[ModifiedOccurrences](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) <br/> |Contém o conjunto de todas as reuniões da série que foram modificadas do padrão de recorrência original.  <br/> |
|[Propriedade DeletedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) <br/> |[DeletedOccurrences](https://msdn.microsoft.com/library/736fb305-9528-4be8-ad37-65d7556edbf2%28Office.15%29.aspx) <br/> |Contém o conjunto de todas as reuniões da série que foram excluídas do padrão de recorrência original.  <br/> |
   
Como as reuniões são essencialmente compromissos que incluem participantes, os exemplos de código neste artigo mostram como criar reuniões recorrentes. Se você quiser criar um compromisso recorrente, pode modificar os exemplos removendo o código relacionado aos participantes.
  
## <a name="create-a-recurring-meeting-by-using-the-ews-managed-api"></a>Criar uma reunião recorrente usando a API Gerenciada do EWS
<a name="bk_CreateMtgEWSMA"> </a>

O exemplo de código a seguir mostra como criar uma reunião recorrente. Primeiro, atribua valores às propriedades de um objeto [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) usado para criar uma reunião, use o método [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para salvar a série recorrente em sua pasta de calendário e envie solicitações de reunião para seus participantes. Por fim, use o [método Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) para ver os valores definidos no mestre recorrente da série recorrente que você acabou de criar. 
  
Este exemplo pressupõe que você tenha autenticado em um servidor Exchange e tenha adquirido um [objeto ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **service**. O método neste exemplo retorna a [ID do item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do mestre recorrente da série recorrente. 
  
```cs
public static ItemId CreateARecurringMeeting(ExchangeService service)
{        Appointment recurrMeeting = new Appointment(service);
        // Set the properties you need to create a meeting.
        recurrMeeting.Subject = "Weekly Update Meeting";
        recurrMeeting.Body = "Come hear about how the project is coming along!";
        recurrMeeting.Start = DateTime.Now.AddDays(1);
        recurrMeeting.End = recurrMeeting.Start.AddHours(1);
        recurrMeeting.Location = "Contoso Main Gallery";
        recurrMeeting.RequiredAttendees.Add("Mack@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Sadie@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Magdalena@contoso.com"); recurrMeeting.ReminderMinutesBeforeStart = 30;
             
        DayOfTheWeek[] dow = new DayOfTheWeek[] { (DayOfTheWeek)recurrMeeting.Start.DayOfWeek };
        // The following are the recurrence-specific properties for the meeting.
        recurrMeeting.Recurrence = new Recurrence.WeeklyPattern(recurrMeeting.Start.Date, 1, dow);
        recurrMeeting.Recurrence.StartDate = recurrMeeting.Start.Date;
        recurrMeeting.Recurrence.NumberOfOccurrences = 10;
        // This method results in in a CreateItem call to EWS.
        recurrMeeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
        // Retrieve the meeting subject and the properties that are set on a recurring master when a recurring series is created.
        recurrMeeting = Appointment.Bind(service, recurrMeeting.Id, new PropertySet(AppointmentSchema.Subject,
                                                                                    AppointmentSchema.AppointmentType, 
                                                                                    AppointmentSchema.Recurrence, 
                                                                                    AppointmentSchema.FirstOccurrence,
                                                                                    AppointmentSchema.LastOccurrence,
                                                                                    AppointmentSchema.ModifiedOccurrences,
                                                                                    AppointmentSchema.DeletedOccurrences));
        // Print out the recurring master properties.
        Console.WriteLine("\nAppointment created: " + recurrMeeting.Subject);
        Console.WriteLine("Appointment Type: {0}\n", recurrMeeting.AppointmentType);
        Console.WriteLine("These property values are always null unless the item is a recurring master:\n");
        Console.WriteLine("\tRecurrence pattern: {0}", recurrMeeting.Recurrence.ToString());
        Console.WriteLine("\tRecurring series start Date: {0}", recurrMeeting.Recurrence.StartDate.ToString());
        Console.WriteLine("\tRecurring series end Date: {0}", 
                        recurrMeeting.Recurrence.EndDate == null ? "Null" : recurrMeeting.Recurrence.EndDate.ToString());
        Console.WriteLine("\tHas end: {0}", recurrMeeting.Recurrence.HasEnd.ToString());
        Console.WriteLine("\tNumber of occurrances: {0}", recurrMeeting.Recurrence.NumberOfOccurrences);
        Console.WriteLine("\tLast 24 characters of the first occurrence's item ID:\t {0}", 
                        recurrMeeting.FirstOccurrence.ItemId.ToString().Substring(144));
        Console.WriteLine("\tLast 24 characters of the last occurrence's item ID:\t {0}", 
                        recurrMeeting.LastOccurrence.ItemId.ToString().Substring(144)); 
        Console.WriteLine("\tModified Occurrences: {0}", 
                        (recurrMeeting.ModifiedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString()));
        Console.WriteLine("\tDeleted Occurrences: {0}", 
                        recurrMeeting.DeletedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString());
        // Return the ID of the recurring master.
        return recurrMeeting.Id;
}

```

## <a name="create-a-recurring-meeting-by-using-ews"></a>Criar uma reunião recorrente usando o EWS
<a name="bk_CreateMtgEWS"> </a>

O XML de solicitação e resposta nos exemplos a seguir correspondem a chamadas feitas para criar uma reunião recorrente usando [a API Gerenciada do EWS.](#bk_CreateMtgEWSMA) Observe que, além de definir valores específicos de recorrência no elemento [Recurrence,](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) a solicitação é essencialmente a mesma que você usaria para criar um compromisso de instância única. O exemplo a seguir mostra o XML de solicitação quando você usa a [operação CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar uma reunião. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Name="(UTC-08:00) Pacific Time (US &amp;amp; Canada)" Id="Pacific Standard Time">
        <t:Periods>
          <t:Period Bias="P0DT8H0M0.0S" Name="Standard" Id="Std" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/1" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/2007" />
        </t:Periods>
        <t:TransitionsGroups>
          <t:TransitionsGroup Id="0">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/1</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>4</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>10</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>-1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
          <t:TransitionsGroup Id="1">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/2007</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>3</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>2</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>11</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
        </t:TransitionsGroups>
        <t:Transitions>
          <t:Transition>
            <t:To Kind="Group">0</t:To>
          </t:Transition>
          <t:AbsoluteDateTransition>
            <t:To Kind="Group">1</t:To>
            <t:DateTime>2007-01-01T08:00:00.000Z</t:DateTime>
          </t:AbsoluteDateTransition>
        </t:Transitions>
      </t:TimeZoneDefinition>
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Weekly Update Meeting</t:Subject>
          <t:Body BodyType="HTML">Come hear about how the Organized Observational Paradigm SkyNet project is coming along!</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-08T13:21:32.868-08:00</t:Start>
          <t:End>2014-03-08T14:21:32.868-08:00</t:End>
          <t:Location>Contoso Main Gallery</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Saturday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-03-08-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

 O exemplo a seguir mostra o XML de resposta retornado pela **operação CreateItem.** 
  
Os **atributos ItemId** **e ChangeKey** são reduzidos para a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

O exemplo a seguir mostra o XML de solicitação gerado quando você usa a operação [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) e **a ItemId** para a série que você criou e solicita propriedades definidas apenas em um mestre recorrente para confirmar que **ItemId** retornado pelo servidor ao criar uma série recorrente é para um mestre recorrente. 
  
Os **atributos ItemId** **e ChangeKey** são reduzidos para a capacidade de leitura. 
  
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
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Recurrence" />
          <t:FieldURI FieldURI="calendar:FirstOccurrence" />
          <t:FieldURI FieldURI="calendar:LastOccurrence" />
          <t:FieldURI FieldURI="calendar:ModifiedOccurrences" />
          <t:FieldURI FieldURI="calendar:DeletedOccurrences" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 O exemplo a seguir mostra o XML de resposta retornado pela **operação GetItem.** 
  
Os **atributos ItemId** **e ChangeKey** são reduzidos para a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
              <t:Subject>Weekly Update Meeting</t:Subject>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              <t:Recurrence>
                <t:WeeklyRecurrence>
                  <t:Interval>1</t:Interval>
                  <t:DaysOfWeek>Saturday</t:DaysOfWeek>
                </t:WeeklyRecurrence>
                <t:NumberedRecurrence>
                  <t:StartDate>2014-03-08-08:00</t:StartDate>
                  <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
                </t:NumberedRecurrence>
              </t:Recurrence>
              <t:FirstOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-03-08T21:21:00Z</t:Start>
                <t:End>2014-03-08T22:21:00Z</t:End>
                <t:OriginalStart>2014-03-08T21:21:00Z</t:OriginalStart>
              </t:FirstOccurrence>
              <t:LastOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-05-10T20:21:00Z</t:Start>
                <t:End>2014-05-10T21:21:00Z</t:End>
                <t:OriginalStart>2014-05-10T20:21:00Z</t:OriginalStart>
              </t:LastOccurrence>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Padrões de recorrência e EWS](recurrence-patterns-and-ews.md)
    
- [Acessar uma série recorrente usando o EWS no Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Excluir compromissos em uma série recorrente usando o EWS em Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Atualizar uma série recorrente usando o EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Atualizar uma série recorrente usando o EWS no Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

