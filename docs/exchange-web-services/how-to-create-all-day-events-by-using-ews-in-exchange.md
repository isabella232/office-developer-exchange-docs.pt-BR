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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750699"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="b1920-103">Criar eventos de dia inteiro usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b1920-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="b1920-104">Saiba como criar eventos de dia inteiro usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1920-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b1920-105">Eventos de dia inteiro fornecem uma maneira para representar algo que acontece para um dia inteiro ou vários dias — por exemplo, um feriado ou dias de férias.</span><span class="sxs-lookup"><span data-stu-id="b1920-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="b1920-106">Criar eventos de dia inteiro com a API gerenciada de EWS ou o EWS é muito fácil.</span><span class="sxs-lookup"><span data-stu-id="b1920-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="b1920-107">É como [a criação de compromissos](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mas com algumas pequenas alterações.</span><span class="sxs-lookup"><span data-stu-id="b1920-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="b1920-108">Definindo os horários de início e término</span><span class="sxs-lookup"><span data-stu-id="b1920-108">Setting start and end times</span></span>

<span data-ttu-id="b1920-109">Por definição, os eventos de dia inteiro iniciar à meia-noite em um determinado dia e end 24 horas (ou um múltiplo de 24 horas) posteriormente.</span><span class="sxs-lookup"><span data-stu-id="b1920-109">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later.</span></span> <span data-ttu-id="b1920-110">No entanto, a API gerenciada de EWS e EWS permitem especificar horários que não seja a meia-noite ao criar eventos de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="b1920-110">However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events.</span></span> <span data-ttu-id="b1920-111">Isso pode levar à comportamento acidentais se não ter ciência de como esses horários obtém convertidos no servidor.</span><span class="sxs-lookup"><span data-stu-id="b1920-111">This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="b1920-112">Quando uma solicitação for recebida para criar um novo evento de dia inteiro com o início de não-meia-noite (na [zona de tempo da solicitação ou compromisso](time-zones-and-ews-in-exchange.md)) e/ou de término, esses horários obtém ajustados para meia-noite no fuso horário apropriado conforme as regras a seguintes:</span><span class="sxs-lookup"><span data-stu-id="b1920-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="b1920-113">Horas de início de não-meia-noite são ajustadas para a meia-noite antes da hora especificada.</span><span class="sxs-lookup"><span data-stu-id="b1920-113">Non-midnight start times are adjusted to the midnight prior to the time specified.</span></span> <span data-ttu-id="b1920-114">Por exemplo, 1:00 PM em 6 de junho obtém ajustada para 12:00 AM em 6 de junho.</span><span class="sxs-lookup"><span data-stu-id="b1920-114">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="b1920-115">Encerramento de não-meia-noite é ajustados para a meia-noite após o tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="b1920-115">Non-midnight end times are adjusted to the midnight after the time specified.</span></span> <span data-ttu-id="b1920-116">Por exemplo, 1:00 PM em 6 de junho obtém ajustada para 12:00 AM em 7 de junho.</span><span class="sxs-lookup"><span data-stu-id="b1920-116">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="b1920-117">Portanto, o evento de dia inteiro que você criar é sempre inclui a hora de início e término que você especifica, mas talvez mais tempo de declaração no usuário do calendário devido à mudança para a meia-noite.</span><span class="sxs-lookup"><span data-stu-id="b1920-117">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight.</span></span> <span data-ttu-id="b1920-118">Porque o servidor irá ajustar a hora de início e término para meia-noite, recomendamos que você especifique seu horário de início e término à meia-noite para evitar quaisquer alterações indesejadas para os horários.</span><span class="sxs-lookup"><span data-stu-id="b1920-118">Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="b1920-119">Também é importante considerar os fusos horários ao criar eventos de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="b1920-119">It's also important to consider time zones when creating all-day events.</span></span> <span data-ttu-id="b1920-120">Como o Exchange server impõe um meia-noite início e hora no fuso horário do compromisso ou solicitação de término, exibindo desse evento de dia inteiro em um cliente configurado para um fuso horário diferente pode gerar resultados inesperados.</span><span class="sxs-lookup"><span data-stu-id="b1920-120">Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results.</span></span> <span data-ttu-id="b1920-121">Dependendo do cliente, ele pode ser exibido como um evento de dia inteiro com dias adicionais que você não pretende incluir ou ela pode não aparecer como um evento de dia inteiro todo.</span><span class="sxs-lookup"><span data-stu-id="b1920-121">Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether.</span></span> <span data-ttu-id="b1920-122">Por isso, é recomendável que você use fuso de horário preferencial do usuário sempre que possível, quando você criar eventos de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="b1920-122">Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="b1920-123">Criar um evento de dia inteiro usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="b1920-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="b1920-124">O exemplo a seguir mostra como usar a API gerenciada de EWS para criar um evento de dia inteiro, começando na data especificada pelo parâmetro _startDate_ e que dura para o número de dias especificado pelo parâmetro _numDays_ .</span><span class="sxs-lookup"><span data-stu-id="b1920-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="b1920-125">Observe que o compromisso será criado no fuso horário especificado pela propriedade [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b1920-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="b1920-126">Este exemplo pressupõe que o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) passado no parâmetro _serviço_ foi inicializado com os valores válidos para as propriedades de [credenciais](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b1920-126">This example assumes that the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="b1920-127">Criar um evento de dia inteiro usando o EWS</span><span class="sxs-lookup"><span data-stu-id="b1920-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="b1920-128">O exemplo a seguir mostra uma solicitação EWS [operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar um evento de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="b1920-128">The following example shows an EWS [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="b1920-129">O compromisso é criado no fuso horário do Leste, conforme indicado pelo elemento [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b1920-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="b1920-130">Observe que a parte de tempo dos valores dos elementos [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) estão ambas 04:00Z, que converte a meia-noite no fuso horário do Leste durante o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="b1920-130">Notice that the time portion of the values of the [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="b1920-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="b1920-131">See also</span></span>


- [<span data-ttu-id="b1920-132">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b1920-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="b1920-133">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b1920-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="b1920-134">Fusos horários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b1920-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    

