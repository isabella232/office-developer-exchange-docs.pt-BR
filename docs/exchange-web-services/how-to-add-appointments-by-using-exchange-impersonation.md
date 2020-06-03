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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455328"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="8e101-103">Adicionar compromissos usando a representação do Exchange</span><span class="sxs-lookup"><span data-stu-id="8e101-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="8e101-104">Saiba como usar a representação com a API gerenciada do EWS ou o EWS no Exchange para adicionar compromissos aos calendários dos usuários.</span><span class="sxs-lookup"><span data-stu-id="8e101-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users' calendars.</span></span>
  
<span data-ttu-id="8e101-105">Você pode criar um aplicativo de serviço que insere compromissos diretamente em um calendário do Exchange usando uma conta de serviço que tenha a função **ApplicationImpersonation** [habilitada](how-to-configure-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="8e101-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the **ApplicationImpersonation** [role enabled](how-to-configure-impersonation.md).</span></span> <span data-ttu-id="8e101-106">Quando você usa a representação, o aplicativo está agindo como o usuário; é como se o usuário adicionasse o compromisso ao calendário usando um cliente como o Outlook.</span><span class="sxs-lookup"><span data-stu-id="8e101-106">When you use impersonation, the application is acting as the user; it's as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="8e101-107">Quando estiver usando a representação, tenha em mente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="8e101-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="8e101-108">O objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) deve estar associado à conta de serviço.</span><span class="sxs-lookup"><span data-stu-id="8e101-108">Your [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="8e101-109">Você pode usar o mesmo objeto **ExchangeService** para representar várias contas alterando a propriedade [ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para cada conta que deseja representar.</span><span class="sxs-lookup"><span data-stu-id="8e101-109">You can use the same **ExchangeService** object to impersonate multiple accounts by changing the [ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="8e101-110">Qualquer item que você salva em uma conta representada pode ser usado apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="8e101-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="8e101-111">Se você deseja salvar o mesmo compromisso em várias contas, por exemplo, você precisa criar um objeto de [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) para cada conta.</span><span class="sxs-lookup"><span data-stu-id="8e101-111">If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="8e101-112">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e101-112">Prerequisites</span></span>

<span data-ttu-id="8e101-113">Seu aplicativo precisa de uma conta para usar para se conectar ao servidor do Exchange antes de poder usar a representação.</span><span class="sxs-lookup"><span data-stu-id="8e101-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="8e101-114">Sugerimos que você use uma conta de serviço para o aplicativo que recebeu a função de representação de aplicativo para as contas que ele acessará.</span><span class="sxs-lookup"><span data-stu-id="8e101-114">We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing.</span></span> <span data-ttu-id="8e101-115">Para obter mais informações, consulte [Configure Impersonation](how-to-configure-impersonation.md)</span><span class="sxs-lookup"><span data-stu-id="8e101-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="8e101-116">Adicionar compromissos usando representação com a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="8e101-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="8e101-117">O exemplo a seguir adiciona um compromisso ou reunião ao calendário de uma ou mais contas do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e101-117">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts.</span></span> <span data-ttu-id="8e101-118">O método usa três parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8e101-118">The method takes three parameters.</span></span>
  
-  <span data-ttu-id="8e101-119">_serviço_ — um objeto **ExchangeService** associado à conta do aplicativo de serviço no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e101-119">_service_ — An **ExchangeService** object bound to the service application's account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="8e101-120">_EmailAddresses_ — um objeto [System. List](https://msdn.microsoft.com/library/6sh2ey19.aspx) contendo uma lista de cadeias de caracteres de endereços de email SMTP.</span><span class="sxs-lookup"><span data-stu-id="8e101-120">_emailAddresses_ — A [System.List](https://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="8e101-121">_Factory_ — um objeto que implementa a interface **IAppointmentFactory** .</span><span class="sxs-lookup"><span data-stu-id="8e101-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="8e101-122">Essa interface tem um método, **getcompromisso** que recebe um objeto **ExchangeService** como um parâmetro e retorna um objeto **compromisso** .</span><span class="sxs-lookup"><span data-stu-id="8e101-122">This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an **Appointment** object.</span></span> <span data-ttu-id="8e101-123">A interface **IAppointmentFactory** é definida [IAppointmentFactory interface](#bk_IAppointmentFactory).</span><span class="sxs-lookup"><span data-stu-id="8e101-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
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

<span data-ttu-id="8e101-124">Ao salvar o compromisso, o código verifica para determinar se algum participante foi adicionado à propriedade [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8e101-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="8e101-125">Se houver, o método de [compromisso. Save](https://msdn.microsoft.com/library/dd635394.aspx) é chamado com o valor de enumeração [SendToAllAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que os participantes recebam solicitações de reunião; caso contrário, o método de **compromisso. Save** é chamado com o valor de enumeração [SendToNone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que o compromisso seja salvo no calendário do usuário representado com a propriedade [compromisso. issatisfaçing](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="8e101-125">If they have, the [Appointment.Save](https://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="8e101-126">Interface IAppointmentFactory</span><span class="sxs-lookup"><span data-stu-id="8e101-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="8e101-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="8e101-127"><a name="bk_IAppointmentFactory"> </a></span></span>

<span data-ttu-id="8e101-128">Como você precisa de um novo objeto de **compromisso** sempre que quiser salvar um compromisso no calendário de um usuário representado, a interface **IAppointmentFactory** abstrai o objeto usado para preencher cada objeto de **compromisso** .</span><span class="sxs-lookup"><span data-stu-id="8e101-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user's calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object.</span></span> <span data-ttu-id="8e101-129">Esta versão é uma interface simples que contém apenas um método, **getcompromisso**, que usa um objeto **ExchangeService** como um parâmetro e retorna um novo objeto **compromisso** associado a esse objeto **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="8e101-129">This version is a simple interface that contains only one method, **GetAppointment**, that takes an **ExchangeService** object as a parameter and returns a new **Appointment** object bound to that **ExchangeService** object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="8e101-130">O exemplo de classe **AppointmentFactory** a seguir mostra uma implementação da interface **IAppointmentFactory** que retorna um compromisso simples que ocorre três dias a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="8e101-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="8e101-131">Se você remover o comentário da `appointment.RequiredAttendees.Add` linha, o método **getcompromisso** retornará uma reunião e o endereço de email especificado nessa linha receberá uma solicitação de reunião com o usuário representado listado como organizador.</span><span class="sxs-lookup"><span data-stu-id="8e101-131">If you uncomment the  `appointment.RequiredAttendees.Add` line, the **GetAppointment** method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="8e101-132">Adicionar compromissos usando representação com EWS</span><span class="sxs-lookup"><span data-stu-id="8e101-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="8e101-133">O EWS permite que o aplicativo use a representação para adicionar itens a um calendário em nome do proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="8e101-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="8e101-134">Este exemplo mostra como usar a operação [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para adicionar um compromisso ao calendário de uma conta representada.</span><span class="sxs-lookup"><span data-stu-id="8e101-134">This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
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

<span data-ttu-id="8e101-135">Observe que, além da adição do elemento **ExchangeImpersonation** no cabeçalho SOAP, para especificar a conta que estamos representando, esta é a mesma solicitação XML usada para criar um compromisso sem usar representação.</span><span class="sxs-lookup"><span data-stu-id="8e101-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="8e101-136">O exemplo a seguir mostra a resposta XML retornada pela operação **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="8e101-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8e101-137">Os atributos **ItemId** e **ChangeKey** são reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="8e101-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="8e101-138">Novamente, esse é o mesmo XML que é retornado quando você usa a operação **CreateItem** sem usar representação.</span><span class="sxs-lookup"><span data-stu-id="8e101-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8e101-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="8e101-139">See also</span></span>


- [<span data-ttu-id="8e101-140">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8e101-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="8e101-141">Função ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="8e101-141">ApplicationImpersonation role</span></span>](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="8e101-142">Configurar representação</span><span class="sxs-lookup"><span data-stu-id="8e101-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="8e101-143">Identificar a conta a ser representada</span><span class="sxs-lookup"><span data-stu-id="8e101-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="8e101-144">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8e101-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="8e101-145">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="8e101-145">CreateItem operation (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md)
    
- [<span data-ttu-id="8e101-146">Propriedade ExchangeService. ImpersonatedUserId</span><span class="sxs-lookup"><span data-stu-id="8e101-146">ExchangeService.ImpersonatedUserId property</span></span>](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)
    

