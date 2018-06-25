---
title: Adicione os compromissos, usando a representação do Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Aprenda a usar representação com a API gerenciada de EWS ou o EWS no Exchange para adicionar compromissos a calendários de usuários.
ms.openlocfilehash: fe737658b88aca66d8b4c2860245db000888ba17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750707"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Adicione os compromissos, usando a representação do Exchange

Aprenda a usar representação com a API gerenciada de EWS ou o EWS no Exchange para adicionar compromissos a calendários de usuários.
  
Você pode criar um aplicativo de serviço que insere compromissos diretamente em um calendário do Exchange usando uma conta de serviço que tem o **AppplicationImpersonation**[função habilitada](how-to-configure-impersonation.md). Quando você usa representação, o aplicativo está agindo como o usuário; é como se o usuário adicionado o compromisso no calendário usando um cliente como o Outlook. 
  
Quando você estiver usando a representação, tenha em mente o seguinte:
  
- Seu objeto [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) deve ser vinculado à conta de serviço. Você pode usar o mesmo objeto **ExchangeService** para representar várias contas, alterando a propriedade [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para cada conta que você deseja representar. 
    
- Qualquer item que você salve em uma conta representada só pode ser usado uma vez. Por exemplo, se você deseja salvar o mesmo compromisso em várias contas, você precisa criar um objeto de [compromisso](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) para cada conta. 
    
## <a name="prerequisites"></a>Pré-requisitos

Seu aplicativo precisa de uma conta a ser usada para se conectar ao servidor do Exchange para que ele possa usar representação. Sugerimos que você use uma conta de serviço para o aplicativo que recebeu a função de representação do aplicativo para as contas que ele acessará. Para obter mais informações, consulte [Configure representação](how-to-configure-impersonation.md)
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>Adicione os compromissos, usando a representação com a API gerenciada de EWS

O exemplo a seguir adiciona uma reunião ou compromisso no calendário de uma ou mais contas do Exchange. O método admite três parâmetros.
  
-  _serviço_ — um objeto **ExchangeService** vinculado à conta do aplicativo de serviço no servidor Exchange. 
    
-  _emailAddresses_ — um objeto [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) contendo uma lista de cadeias de caracteres de endereço de email SMTP. 
    
-  _alocador_ — um objeto que implementa a interface **IAppointmentFactory** . Essa interface possui um método, **GetAppointment** que utiliza um objeto **ExchangeService** como um parâmetro e retorna um objeto de **compromisso** . A interface **IAppointmentFactory** é definida [IAppointmentFactory interface](#bk_IAppointmentFactory).
    
```cs
private static void CreateAppointments(ExchangeService service, List<string> emailAddresses, IAppointmentFactory factory)
{
  // Loop through the list of email addresses to add the appointment.
  foreach (var emailAddress in emailAddresses)
  {
    Console.WriteLine(string.Format("  Placing appointment in calendar for {0}.", emailAddress));
    // Set the email address of the account to get the appointment.
    service.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, emailAddress);
    // Get the appointment to add.
    Appointment appointment = factory.GetAppointment(service);
    // Save the appointment.
    try
    {
      if (appointment.RequiredAttendees.Count > 0)
      {
        // The appointment has attendees so send them the meeting request.
        appointment.Save(SendInvitationsMode.SendToAllAndSaveCopy);
      }
      else
      {
        // The appointment does not have attendees, so just save to calendar.
        appointment.Save(SendInvitationsMode.SendToNone);
      }
    }
    catch (ServiceResponseException ex)
    {
      Console.WriteLine(string.Format("Could not create appointment for {0}", emailAddress));
      Console.WriteLine(ex.Message);
    }
  }
}
```

Quando você salva o compromisso, o código verifica para determinar se qualquer participantes foram adicionados à propriedade [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) . Se eles tiverem, o método [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) é chamado com o valor de enumeração [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que os participantes recebem solicitações de reunião; Caso contrário, o método **Appointment.Save** é chamado com o valor de enumeração [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que o compromisso é salvo no calendário do usuário representada com a propriedade [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) definida como **false**.
  
### <a name="iappointmentfactory-interface"></a>Interface de IAppointmentFactory
<a name="bk_IAppointmentFactory"> </a>

Porque é necessário um novo objeto de **compromisso** toda vez que você deseja salvar um compromisso no calendário do usuário um representada, a interface **IAppointmentFactory** abstrai o objeto usado para popular a cada objeto de **compromisso** . Esta versão é uma interface simples que contém apenas um método, **GetAppointment**, que utiliza um objeto **ExchangeService** como um parâmetro e retorna um novo objeto de **compromisso** associado a esse objeto **ExchangeService** . 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

O exemplo de classe **AppointmentFactory** a seguir mostra uma implementação da interface **IAppointmentFactory** que retorna um compromisso simples que ocorre três dias a partir de agora. Se você não comentar o `appointment.RequiredAttendees.Add` linha, o método **GetAppointment** retornará uma reunião e o endereço de email especificado nessa linha receberá uma solicitação de reunião com o usuário representado listado como o organizador. 
  
```cs
class AppointmentFactory : IAppointmentFactory
{
  public Appointment GetAppointment(ExchangeService service)
  {
    // First create the appointment to add.
    Appointment appointment = new Appointment(service);
    // Set the properties on the appointment.
    appointment.Subject = "Tennis lesson";
    appointment.Body = "Focus on backhand this week.";
    appointment.Start = DateTime.Now.AddDays(3);
    appointment.End = appointment.Start.AddHours(1);
    appointment.Location = "Tennis club";
    // appointment.RequiredAttendees.Add(new Attendee("sonyaf@contoso1000.onmicrosoft.com"));
    return appointment;
  }
}

```

## <a name="add-appointments-by-using-impersonation-with-ews"></a>Adicione os compromissos, usando a representação EWS

EWS permite que você aplicativo utilizam a representação para adicionar itens a um calendário em nome de proprietário do calendário. Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para adicionar um compromisso no calendário de uma conta representada. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Observe que, que não seja a adição do elemento **ExchangeImpersonation** no cabeçalho SOAP para especificar a conta que podemos são representando, essa é a mesma solicitação XML usada para criar um compromisso sem usar representação. 
  
O exemplo a seguir mostra a resposta XML retornada pela operação de **CreateItem** . 
  
> [!NOTE]
> Os atributos **ItemId** e **ChangeKey** são reduzidos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

Novamente, este é o mesmo XML que é retornado quando você usar a operação **CreateItem** sem usar representação. 
  
## <a name="see-also"></a>Confira também


- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
    
- [Função ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [Configurar representação](how-to-configure-impersonation.md)
    
- [Identificar a conta para representar](how-to-identify-the-account-to-impersonate.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Operação CreateItem (item de calendário)](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [Propriedade ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    

