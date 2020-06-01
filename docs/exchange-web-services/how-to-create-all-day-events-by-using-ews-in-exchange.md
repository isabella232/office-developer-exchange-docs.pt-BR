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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456861"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="7b75d-103">Criar eventos de dia inteiro usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7b75d-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="7b75d-104">Saiba como criar eventos de dia inteiro usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b75d-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7b75d-105">Os eventos de dia inteiro fornecem uma maneira de representar algo que acontece para um dia inteiro ou vários dias — por exemplo, um feriado ou dias de férias.</span><span class="sxs-lookup"><span data-stu-id="7b75d-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="7b75d-106">Criar eventos de dia inteiro com a API gerenciada do EWS ou o EWS é um instantâneo.</span><span class="sxs-lookup"><span data-stu-id="7b75d-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="7b75d-107">É como [criar compromissos](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mas com algumas pequenas alterações.</span><span class="sxs-lookup"><span data-stu-id="7b75d-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="7b75d-108">Definir horários de início e término</span><span class="sxs-lookup"><span data-stu-id="7b75d-108">Setting start and end times</span></span>

<span data-ttu-id="7b75d-109">Por definição, os eventos de dia inteiro começam à meia-noite em um dia específico e terminam 24 horas (ou um múltiplo de 24 horas) mais tarde.</span><span class="sxs-lookup"><span data-stu-id="7b75d-109">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later.</span></span> <span data-ttu-id="7b75d-110">No entanto, a API gerenciada do EWS e o EWS permitem que você especifique horários diferentes da meia-noite ao criar eventos de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="7b75d-110">However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events.</span></span> <span data-ttu-id="7b75d-111">Isso pode levar a um comportamento inesperado se você não estiver ciente de como essas horas são traduzidas no servidor.</span><span class="sxs-lookup"><span data-stu-id="7b75d-111">This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="7b75d-112">Quando uma solicitação é recebida para criar um novo evento de dia inteiro com não-meia-noite (no [fuso horário das horas de](time-zones-and-ews-in-exchange.md)início e/ou de término do compromisso), essas horas são ajustadas à meia-noite no fuso horário apropriado, de acordo com as seguintes regras:</span><span class="sxs-lookup"><span data-stu-id="7b75d-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="7b75d-113">Horários de início sem meia-noite são ajustados à meia-noite antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="7b75d-113">Non-midnight start times are adjusted to the midnight prior to the time specified.</span></span> <span data-ttu-id="7b75d-114">Por exemplo, 1:00 PM em 6 de junho é ajustado para 12:00 AM 6 de junho.</span><span class="sxs-lookup"><span data-stu-id="7b75d-114">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="7b75d-115">Horários de término sem meia-noite são ajustados à meia-noite após o tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="7b75d-115">Non-midnight end times are adjusted to the midnight after the time specified.</span></span> <span data-ttu-id="7b75d-116">Por exemplo, 1:00 PM em 6 de junho é ajustado para 12:00 A.M. em 7 de junho.</span><span class="sxs-lookup"><span data-stu-id="7b75d-116">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="7b75d-117">Portanto, o evento de dia inteiro que você cria é sempre inclusivo da hora de início e de término que você especificar, mas pode solicitar tempo adicional no calendário do usuário devido à meia-noite.</span><span class="sxs-lookup"><span data-stu-id="7b75d-117">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight.</span></span> <span data-ttu-id="7b75d-118">Como o servidor ajustará o tempo de início e de término à meia-noite, recomendamos que você especifique o horário de início e de término à meia-noite para evitar qualquer alteração não intencional nos horários.</span><span class="sxs-lookup"><span data-stu-id="7b75d-118">Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="7b75d-119">Também é importante considerar os fusos horários ao criar eventos de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="7b75d-119">It's also important to consider time zones when creating all-day events.</span></span> <span data-ttu-id="7b75d-120">Como o Exchange Server impõe uma hora de início e de término da meia-noite no fuso horário da solicitação ou compromisso, a exibição desse evento de dia inteiro em um cliente configurado para um fuso horário diferente pode gerar resultados inesperados.</span><span class="sxs-lookup"><span data-stu-id="7b75d-120">Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results.</span></span> <span data-ttu-id="7b75d-121">Dependendo do cliente, ele pode aparecer como um evento de dia inteiro com dias extras que você não pretende incluir ou pode não aparecer como um evento de dia inteiro completamente.</span><span class="sxs-lookup"><span data-stu-id="7b75d-121">Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether.</span></span> <span data-ttu-id="7b75d-122">Por causa disso, recomendamos que você use o fuso horário preferencial do usuário sempre que possível ao criar eventos de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="7b75d-122">Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="7b75d-123">Criar um evento de dia inteiro usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="7b75d-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="7b75d-124">O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um evento de dia inteiro, começando na data especificada pelo parâmetro _StartDate_ e duradoura pelo número de dias especificado pelo parâmetro _numDays_ .</span><span class="sxs-lookup"><span data-stu-id="7b75d-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="7b75d-125">Observe que o compromisso será criado no fuso horário especificado pela propriedade [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7b75d-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="7b75d-126">Este exemplo pressupõe que o objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) passado no parâmetro _Service_ tenha sido inicializado com valores válidos para as propriedades [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7b75d-126">This example assumes that the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="7b75d-127">Criar um evento de dia inteiro usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7b75d-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="7b75d-128">O exemplo a seguir mostra uma solicitação de operação do EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar um evento de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="7b75d-128">The following example shows an EWS [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="7b75d-129">O compromisso é criado no fuso horário da costa leste, conforme indicado pelo elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7b75d-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="7b75d-130">Observe que a parte de hora dos valores dos elementos [inicial](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [final](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) são 04:00Z, que converte para meia-noite no fuso horário da costa leste durante o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="7b75d-130">Notice that the time portion of the values of the [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="7b75d-131">Também consulte</span><span class="sxs-lookup"><span data-stu-id="7b75d-131">See also</span></span>


- [<span data-ttu-id="7b75d-132">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7b75d-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="7b75d-133">Criar compromissos e reuniões usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7b75d-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="7b75d-134">Fusos horários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7b75d-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    

