---
title: Criar compromissos em um fuso horário específico usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Saiba como criar compromissos em fusos horários específicos usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 9b1160a9d62ab092d1b60265eba1ad953be0032b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456854"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a><span data-ttu-id="bb756-103">Criar compromissos em um fuso horário específico usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bb756-103">Create appointments in a specific time zone by using EWS in Exchange</span></span>

<span data-ttu-id="bb756-104">Saiba como criar compromissos em fusos horários específicos usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb756-104">Learn how to create appointments in specific time zones by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="bb756-105">Quando um compromisso ou reunião é criado em um calendário do Exchange, o fuso horário usado para especificar as horas de início e término é salvo como o fuso horário de criação do compromisso.</span><span class="sxs-lookup"><span data-stu-id="bb756-105">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment.</span></span> <span data-ttu-id="bb756-106">Esse fuso horário também é usado para [interpretar valores de data e hora que não têm um fuso horário explícito especificado](time-zones-and-ews-in-exchange.md), portanto, é importante entender suas opções para especificar o fuso horário.</span><span class="sxs-lookup"><span data-stu-id="bb756-106">That time zone is also used to [interpret date and time values that do not have an explicit time zone specified](time-zones-and-ews-in-exchange.md), so it is important to understand your options to specify the time zone.</span></span>
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a><span data-ttu-id="bb756-107">Criar compromissos em fusos horários diferentes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="bb756-107">Creating appointments in different time zones by using the EWS Managed API</span></span>

<span data-ttu-id="bb756-108">Ao criar compromissos ou reuniões usando a API gerenciada do EWS, você tem três opções para especificar o fuso horário:</span><span class="sxs-lookup"><span data-stu-id="bb756-108">When creating appointments or meetings using the EWS Managed API, you have three options for specifying the time zone:</span></span>
  
- <span data-ttu-id="bb756-109">Para usar o fuso horário do computador em que a API gerenciada do EWS está sendo executada, não especifique um fuso horário ao criar o objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bb756-109">To use the time zone of the computer where your EWS Managed API is executing, do not specify a time zone when creating the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object.</span></span> 
    
- <span data-ttu-id="bb756-110">Para usar um fuso horário específico para todas as propriedades de data/hora, incluindo propriedades ao criar um novo compromisso ou reunião, especifique um fuso horário no construtor para o objeto **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="bb756-110">To use a specific time zone for all date/time properties, including properties when creating a new appointment or meeting, specify a time zone in the constructor for the **ExchangeService** object.</span></span> 
    
- <span data-ttu-id="bb756-111">Para usar um fuso horário diferente daquele especificado na propriedade [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) , use as propriedades [compromisso. StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) e [compromisso. endtimezone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bb756-111">To use a different time zone than the one specified in the [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property, use the [Appointment.StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) and [Appointment.EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) properties.</span></span> 
    
    > [!NOTE]
    > <span data-ttu-id="bb756-112">A propriedade **endtimezone** só está disponível quando a propriedade [ExchangeService. RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) é definida como **Exchange2010** ou posterior.</span><span class="sxs-lookup"><span data-stu-id="bb756-112">The **EndTimeZone** property is only available when the [ExchangeService.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) property is set to **Exchange2010** or later.</span></span> <span data-ttu-id="bb756-113">Se ele não estiver disponível, a configuração do **StartTimeZone** se aplicará às horas de início e de término do compromisso.</span><span class="sxs-lookup"><span data-stu-id="bb756-113">If it is not available, setting the **StartTimeZone** applies to both the start and end times of the appointment.</span></span> 
  
<span data-ttu-id="bb756-114">No exemplo a seguir, a API gerenciada do EWS é usada para criar três compromissos.</span><span class="sxs-lookup"><span data-stu-id="bb756-114">In the following example, the EWS Managed API is used to create three appointments.</span></span> <span data-ttu-id="bb756-115">Cada compromisso é definido para iniciar em 1:00 PM dois dias de agora, em um fuso horário não especificado, e terminar uma hora depois.</span><span class="sxs-lookup"><span data-stu-id="bb756-115">Each appointment is set to start at 1:00 PM two days from now, in an unspecified time zone, and end one hour later.</span></span> <span data-ttu-id="bb756-116">O primeiro compromisso é criado no fuso horário do computador cliente usando o comportamento padrão de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="bb756-116">The first appointment is created in the client computer's time zone by using default EWS Managed API behavior.</span></span> <span data-ttu-id="bb756-117">O segundo é criado no fuso horário central usando as propriedades de **compromisso. StartTimeZone** e **compromisso. endtimezone** .</span><span class="sxs-lookup"><span data-stu-id="bb756-117">The second is created in the Central time zone by using the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="bb756-118">O terceiro é criado no fuso horário das montanhas usando a propriedade **ExchangeService. TimeZone** .</span><span class="sxs-lookup"><span data-stu-id="bb756-118">The third is created in the Mountain time zone by using the **ExchangeService.TimeZone** property.</span></span> 
  
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

<span data-ttu-id="bb756-119">Quando este exemplo é executado em um computador cliente configurado no fuso horário do leste, e os três compromissos que ele cria são exibidos de um cliente configurado no fuso horário do leste, eles aparecem às 1:00 P.M., 2:00 PM e 3:00 PM, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="bb756-119">When this example is executed on a client computer configured in the Eastern time zone, and the three appointments it creates are viewed from a client configured in the Eastern time zone, they appear at 1:00 PM, 2:00 PM, and 3:00 PM, respectively.</span></span>
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a><span data-ttu-id="bb756-120">Criar compromissos em fusos horários diferentes usando o EWS</span><span class="sxs-lookup"><span data-stu-id="bb756-120">Creating appointments in different time zones by using EWS</span></span>

<span data-ttu-id="bb756-121">Ao criar compromissos ou reuniões usando o EWS, você tem três opções para especificar o fuso horário:</span><span class="sxs-lookup"><span data-stu-id="bb756-121">When creating appointments or meetings using EWS, you have three options for specifying the time zone:</span></span>
  
- <span data-ttu-id="bb756-122">Para usar o tempo universal coordenado (UTC), não inclua um elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , elemento [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (somente Exchange 2007) ou os elementos [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) e [endtimezone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 e posterior) na solicitação de [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bb756-122">To use Coordinated Universal Time (UTC), do not include a [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) element (Exchange 2007 only), or [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements (Exchange 2010 and later) in the [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
- <span data-ttu-id="bb756-123">Para usar um fuso horário específico para todas as propriedades de data/hora, incluindo propriedades ao criar um novo compromisso ou reunião, especifique um fuso horário no elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) na solicitação de [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bb756-123">To use a specific time zone for all date/time properties, including properties when creating a new appointment or meeting, specify a time zone in the [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element in the [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
- <span data-ttu-id="bb756-124">Para usar um fuso horário diferente daquele especificado no elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , inclua um elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , elemento [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (somente Exchange 2007) ou [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) e [endtimezone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) Elements (Exchange 2010 e posterior) na solicitação de [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bb756-124">To use a different time zone than the one specified in the [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, include a [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) element (Exchange 2007 only), or [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements (Exchange 2010 and later) in the [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
<span data-ttu-id="bb756-125">O exemplo a seguir, a solicitação de [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) cria um compromisso usando UTC.</span><span class="sxs-lookup"><span data-stu-id="bb756-125">The following example [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request creates an appointment using UTC.</span></span> <span data-ttu-id="bb756-126">Observe que o elemento **TimeZoneContext** , o elemento **StartTimeZone** e o elemento **endtimezone** estão ausentes.</span><span class="sxs-lookup"><span data-stu-id="bb756-126">Notice that the **TimeZoneContext** element, the **StartTimeZone** element, and the **EndTimeZone** element are absent.</span></span> <span data-ttu-id="bb756-127">Os valores do elemento **inicial** e **final** são expressos em UTC.</span><span class="sxs-lookup"><span data-stu-id="bb756-127">The **Start** and **End** element values are expressed in UTC.</span></span> 
  
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

<span data-ttu-id="bb756-128">O exemplo a seguir, a solicitação de [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) usa os elementos **StartTimeZone** e **endtimezone** para especificar o fuso horário central para o compromisso.</span><span class="sxs-lookup"><span data-stu-id="bb756-128">The following example [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request uses the **StartTimeZone** and **EndTimeZone** elements to specify the Central time zone for the appointment.</span></span> <span data-ttu-id="bb756-129">Observe que o elemento **TimeZoneContext** está ausente.</span><span class="sxs-lookup"><span data-stu-id="bb756-129">Notice that the **TimeZoneContext** element is absent.</span></span> <span data-ttu-id="bb756-130">No entanto, se estiver presente, os valores dos elementos **StartTimeZone** e **endtimezone** substituirão seu valor.</span><span class="sxs-lookup"><span data-stu-id="bb756-130">However, if it were present, the values of the **StartTimeZone** and **EndTimeZone** elements would override its value.</span></span> <span data-ttu-id="bb756-131">Novamente, os valores do elemento **inicial** e **final** são expressos em UTC.</span><span class="sxs-lookup"><span data-stu-id="bb756-131">Again, the **Start** and **End** element values are expressed in UTC.</span></span> 
  
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

<span data-ttu-id="bb756-132">O exemplo a seguir, solicitação de [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) define o elemento **TimeZoneContext** para o fuso horário das montanhas.</span><span class="sxs-lookup"><span data-stu-id="bb756-132">The following example [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request sets the **TimeZoneContext** element to the Mountain time zone.</span></span> <span data-ttu-id="bb756-133">Observe que os elementos **StartTimeZone** e **endtimezone** estão ausentes.</span><span class="sxs-lookup"><span data-stu-id="bb756-133">Notice that the **StartTimeZone** and **EndTimeZone** elements are absent.</span></span> <span data-ttu-id="bb756-134">Novamente, os valores do elemento **inicial** e **final** são expressos em UTC.</span><span class="sxs-lookup"><span data-stu-id="bb756-134">Again, the **Start** and **End** element values are expressed in UTC.</span></span> 
  
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

<span data-ttu-id="bb756-135">Quando os três compromissos criados pelas solicitações anteriores de exemplos do EWS são exibidos de um cliente configurado no fuso horário da costa leste, eles aparecem em 1:00 P.M., 2:00 PM e 3:00 PM, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="bb756-135">When the three appointments created by the previous EWS example requests are viewed from a client configured in the Eastern time zone, they appear at 1:00 PM, 2:00 PM, and 3:00 PM, respectively.</span></span>
  
## 

<span data-ttu-id="bb756-136">Agora que você sabe como criar compromissos em fusos horários específicos, convém [atualizar os fusos horários em compromissos existentes](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) para um diferente.</span><span class="sxs-lookup"><span data-stu-id="bb756-136">Now that you know how to create appointments in specific time zones, you might want to [update the time zones on existing appointments](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) to a different one.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bb756-137">Também consulte</span><span class="sxs-lookup"><span data-stu-id="bb756-137">See also</span></span>


- [<span data-ttu-id="bb756-138">Fusos horários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bb756-138">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    
- [<span data-ttu-id="bb756-139">Atualizar o fuso horário de um compromisso usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bb756-139">Update the time zone for an appointment by using EWS in Exchange</span></span>](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="bb756-140">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bb756-140">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

