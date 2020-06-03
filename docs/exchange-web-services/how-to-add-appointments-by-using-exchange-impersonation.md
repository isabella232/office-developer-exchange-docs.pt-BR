---
title: Adicionar compromissos usando a representação do Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Saiba como usar a representação com a API gerenciada do EWS ou o EWS no Exchange para adicionar compromissos aos calendários dos usuários.
localization_priority: Priority
ms.openlocfilehash: b1473d72113f8cc07d05364a4d87fedf23c7351d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455328"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Adicionar compromissos usando a representação do Exchange

Saiba como usar a representação com a API gerenciada do EWS ou o EWS no Exchange para adicionar compromissos aos calendários dos usuários.
  
Você pode criar um aplicativo de serviço que insere compromissos diretamente em um calendário do Exchange usando uma conta de serviço que tenha a função **ApplicationImpersonation** [habilitada](how-to-configure-impersonation.md). Quando você usa a representação, o aplicativo está agindo como o usuário; é como se o usuário adicionasse o compromisso ao calendário usando um cliente como o Outlook. 
  
Quando estiver usando a representação, tenha em mente o seguinte:
  
- O objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) deve estar associado à conta de serviço. Você pode usar o mesmo objeto **ExchangeService** para representar várias contas alterando a propriedade [ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para cada conta que deseja representar. 
    
- Qualquer item que você salva em uma conta representada pode ser usado apenas uma vez. Se você deseja salvar o mesmo compromisso em várias contas, por exemplo, você precisa criar um objeto de [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) para cada conta. 
    
## <a name="prerequisites"></a>Pré-requisitos

Seu aplicativo precisa de uma conta para usar para se conectar ao servidor do Exchange antes de poder usar a representação. Sugerimos que você use uma conta de serviço para o aplicativo que recebeu a função de representação de aplicativo para as contas que ele acessará. Para obter mais informações, consulte [Configure Impersonation](how-to-configure-impersonation.md)
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>Adicionar compromissos usando representação com a API gerenciada do EWS

O exemplo a seguir adiciona um compromisso ou reunião ao calendário de uma ou mais contas do Exchange. O método usa três parâmetros.
  
-  _serviço_ — um objeto **ExchangeService** associado à conta do aplicativo de serviço no servidor Exchange. 
    
-  _EmailAddresses_ — um objeto [System. List](https://msdn.microsoft.com/library/6sh2ey19.aspx) contendo uma lista de cadeias de caracteres de endereços de email SMTP. 
    
-  _Factory_ — um objeto que implementa a interface **IAppointmentFactory** . Essa interface tem um método, **getcompromisso** que recebe um objeto **ExchangeService** como um parâmetro e retorna um objeto **compromisso** . A interface **IAppointmentFactory** é definida [IAppointmentFactory interface](#bk_IAppointmentFactory).
    
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

Ao salvar o compromisso, o código verifica para determinar se algum participante foi adicionado à propriedade [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) . Se houver, o método de [compromisso. Save](https://msdn.microsoft.com/library/dd635394.aspx) é chamado com o valor de enumeração [SendToAllAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que os participantes recebam solicitações de reunião; caso contrário, o método de **compromisso. Save** é chamado com o valor de enumeração [SendToNone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que o compromisso seja salvo no calendário do usuário representado com a propriedade [compromisso. issatisfaçing](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) definida como **false**.
  
### <a name="iappointmentfactory-interface"></a>Interface IAppointmentFactory
<a name="bk_IAppointmentFactory"> </a>

Como você precisa de um novo objeto de **compromisso** sempre que quiser salvar um compromisso no calendário de um usuário representado, a interface **IAppointmentFactory** abstrai o objeto usado para preencher cada objeto de **compromisso** . Esta versão é uma interface simples que contém apenas um método, **getcompromisso**, que usa um objeto **ExchangeService** como um parâmetro e retorna um novo objeto **compromisso** associado a esse objeto **ExchangeService** . 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

O exemplo de classe **AppointmentFactory** a seguir mostra uma implementação da interface **IAppointmentFactory** que retorna um compromisso simples que ocorre três dias a partir de agora. Se você remover o comentário da `appointment.RequiredAttendees.Add` linha, o método **getcompromisso** retornará uma reunião e o endereço de email especificado nessa linha receberá uma solicitação de reunião com o usuário representado listado como organizador. 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a>Adicionar compromissos usando representação com EWS

O EWS permite que o aplicativo use a representação para adicionar itens a um calendário em nome do proprietário do calendário. Este exemplo mostra como usar a operação [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para adicionar um compromisso ao calendário de uma conta representada. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Observe que, além da adição do elemento **ExchangeImpersonation** no cabeçalho SOAP, para especificar a conta que estamos representando, esta é a mesma solicitação XML usada para criar um compromisso sem usar representação. 
  
O exemplo a seguir mostra a resposta XML retornada pela operação **CreateItem** . 
  
> [!NOTE]
> Os atributos **ItemId** e **ChangeKey** são reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
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
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

Novamente, esse é o mesmo XML que é retornado quando você usa a operação **CreateItem** sem usar representação. 
  
## <a name="see-also"></a>Confira também


- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
    
- [Função ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)
    
- [Configurar representação](how-to-configure-impersonation.md)
    
- [Identificar a conta a ser representada](how-to-identify-the-account-to-impersonate.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Operação CreateItem (item de calendário)](../web-service-reference/createitem-operation-calendar-item.md)
    
- [Propriedade ExchangeService. ImpersonatedUserId](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)
    

