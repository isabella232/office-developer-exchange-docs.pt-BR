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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750707"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="f2cca-103">Adicione os compromissos, usando a representação do Exchange</span><span class="sxs-lookup"><span data-stu-id="f2cca-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="f2cca-104">Aprenda a usar representação com a API gerenciada de EWS ou o EWS no Exchange para adicionar compromissos a calendários de usuários.</span><span class="sxs-lookup"><span data-stu-id="f2cca-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users' calendars.</span></span>
  
<span data-ttu-id="f2cca-105">Você pode criar um aplicativo de serviço que insere compromissos diretamente em um calendário do Exchange usando uma conta de serviço que tem o **AppplicationImpersonation**[função habilitada](how-to-configure-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="f2cca-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the **AppplicationImpersonation**[role enabled](how-to-configure-impersonation.md).</span></span> <span data-ttu-id="f2cca-106">Quando você usa representação, o aplicativo está agindo como o usuário; é como se o usuário adicionado o compromisso no calendário usando um cliente como o Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2cca-106">When you use impersonation, the application is acting as the user; it's as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="f2cca-107">Quando você estiver usando a representação, tenha em mente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f2cca-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="f2cca-108">Seu objeto [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) deve ser vinculado à conta de serviço.</span><span class="sxs-lookup"><span data-stu-id="f2cca-108">Your [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="f2cca-109">Você pode usar o mesmo objeto **ExchangeService** para representar várias contas, alterando a propriedade [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para cada conta que você deseja representar.</span><span class="sxs-lookup"><span data-stu-id="f2cca-109">You can use the same **ExchangeService** object to impersonate multiple accounts by changing the [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="f2cca-110">Qualquer item que você salve em uma conta representada só pode ser usado uma vez.</span><span class="sxs-lookup"><span data-stu-id="f2cca-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="f2cca-111">Por exemplo, se você deseja salvar o mesmo compromisso em várias contas, você precisa criar um objeto de [compromisso](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) para cada conta.</span><span class="sxs-lookup"><span data-stu-id="f2cca-111">If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointment](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="f2cca-112">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2cca-112">Prerequisites</span></span>

<span data-ttu-id="f2cca-113">Seu aplicativo precisa de uma conta a ser usada para se conectar ao servidor do Exchange para que ele possa usar representação.</span><span class="sxs-lookup"><span data-stu-id="f2cca-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="f2cca-114">Sugerimos que você use uma conta de serviço para o aplicativo que recebeu a função de representação do aplicativo para as contas que ele acessará.</span><span class="sxs-lookup"><span data-stu-id="f2cca-114">We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing.</span></span> <span data-ttu-id="f2cca-115">Para obter mais informações, consulte [Configure representação](how-to-configure-impersonation.md)</span><span class="sxs-lookup"><span data-stu-id="f2cca-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="f2cca-116">Adicione os compromissos, usando a representação com a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="f2cca-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="f2cca-117">O exemplo a seguir adiciona uma reunião ou compromisso no calendário de uma ou mais contas do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2cca-117">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts.</span></span> <span data-ttu-id="f2cca-118">O método admite três parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f2cca-118">The method takes three parameters.</span></span>
  
-  <span data-ttu-id="f2cca-119">_serviço_ — um objeto **ExchangeService** vinculado à conta do aplicativo de serviço no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2cca-119">_service_ — An **ExchangeService** object bound to the service application's account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="f2cca-120">_emailAddresses_ — um objeto [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) contendo uma lista de cadeias de caracteres de endereço de email SMTP.</span><span class="sxs-lookup"><span data-stu-id="f2cca-120">_emailAddresses_ — A [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="f2cca-121">_alocador_ — um objeto que implementa a interface **IAppointmentFactory** .</span><span class="sxs-lookup"><span data-stu-id="f2cca-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="f2cca-122">Essa interface possui um método, **GetAppointment** que utiliza um objeto **ExchangeService** como um parâmetro e retorna um objeto de **compromisso** .</span><span class="sxs-lookup"><span data-stu-id="f2cca-122">This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an **Appointment** object.</span></span> <span data-ttu-id="f2cca-123">A interface **IAppointmentFactory** é definida [IAppointmentFactory interface](#bk_IAppointmentFactory).</span><span class="sxs-lookup"><span data-stu-id="f2cca-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
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

<span data-ttu-id="f2cca-124">Quando você salva o compromisso, o código verifica para determinar se qualquer participantes foram adicionados à propriedade [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f2cca-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="f2cca-125">Se eles tiverem, o método [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) é chamado com o valor de enumeração [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que os participantes recebem solicitações de reunião; Caso contrário, o método **Appointment.Save** é chamado com o valor de enumeração [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) para que o compromisso é salvo no calendário do usuário representada com a propriedade [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="f2cca-125">If they have, the [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="f2cca-126">Interface de IAppointmentFactory</span><span class="sxs-lookup"><span data-stu-id="f2cca-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="f2cca-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="f2cca-127"></span></span>

<span data-ttu-id="f2cca-128">Porque é necessário um novo objeto de **compromisso** toda vez que você deseja salvar um compromisso no calendário do usuário um representada, a interface **IAppointmentFactory** abstrai o objeto usado para popular a cada objeto de **compromisso** .</span><span class="sxs-lookup"><span data-stu-id="f2cca-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user's calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object.</span></span> <span data-ttu-id="f2cca-129">Esta versão é uma interface simples que contém apenas um método, **GetAppointment**, que utiliza um objeto **ExchangeService** como um parâmetro e retorna um novo objeto de **compromisso** associado a esse objeto **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="f2cca-129">This version is a simple interface that contains only one method, **GetAppointment**, that takes an **ExchangeService** object as a parameter and returns a new **Appointment** object bound to that **ExchangeService** object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="f2cca-130">O exemplo de classe **AppointmentFactory** a seguir mostra uma implementação da interface **IAppointmentFactory** que retorna um compromisso simples que ocorre três dias a partir de agora.</span><span class="sxs-lookup"><span data-stu-id="f2cca-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="f2cca-131">Se você não comentar o `appointment.RequiredAttendees.Add` linha, o método **GetAppointment** retornará uma reunião e o endereço de email especificado nessa linha receberá uma solicitação de reunião com o usuário representado listado como o organizador.</span><span class="sxs-lookup"><span data-stu-id="f2cca-131">If you uncomment the  `appointment.RequiredAttendees.Add` line, the **GetAppointment** method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="f2cca-132">Adicione os compromissos, usando a representação EWS</span><span class="sxs-lookup"><span data-stu-id="f2cca-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="f2cca-133">EWS permite que você aplicativo utilizam a representação para adicionar itens a um calendário em nome de proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="f2cca-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="f2cca-134">Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para adicionar um compromisso no calendário de uma conta representada.</span><span class="sxs-lookup"><span data-stu-id="f2cca-134">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
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

<span data-ttu-id="f2cca-135">Observe que, que não seja a adição do elemento **ExchangeImpersonation** no cabeçalho SOAP para especificar a conta que podemos são representando, essa é a mesma solicitação XML usada para criar um compromisso sem usar representação.</span><span class="sxs-lookup"><span data-stu-id="f2cca-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="f2cca-136">O exemplo a seguir mostra a resposta XML retornada pela operação de **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="f2cca-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f2cca-137">Os atributos **ItemId** e **ChangeKey** são reduzidos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f2cca-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="f2cca-138">Novamente, este é o mesmo XML que é retornado quando você usar a operação **CreateItem** sem usar representação.</span><span class="sxs-lookup"><span data-stu-id="f2cca-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f2cca-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="f2cca-139">See also</span></span>


- [<span data-ttu-id="f2cca-140">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f2cca-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f2cca-141">Função ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="f2cca-141">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="f2cca-142">Configurar representação</span><span class="sxs-lookup"><span data-stu-id="f2cca-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="f2cca-143">Identificar a conta para representar</span><span class="sxs-lookup"><span data-stu-id="f2cca-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="f2cca-144">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f2cca-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="f2cca-145">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="f2cca-145">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [<span data-ttu-id="f2cca-146">Propriedade ExchangeService.ImpersonatedUserId</span><span class="sxs-lookup"><span data-stu-id="f2cca-146">ExchangeService.ImpersonatedUserId property</span></span>](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    

