---
title: Operação GetUserAvailability
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailability
api_type:
- schema
ms.assetid: 8da17226-5d3a-4525-9ffa-d83730f47bb1
description: Encontre informações sobre a operação do EWS do GetUserAvailability.
ms.openlocfilehash: b6d03c7da65e3f30f093b7e41448abcca2330a84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458219"
---
# <a name="getuseravailability-operation"></a><span data-ttu-id="37f99-103">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="37f99-103">GetUserAvailability operation</span></span>

<span data-ttu-id="37f99-104">Encontre informações sobre a operação do EWS do **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="37f99-104">Find information about the **GetUserAvailability** EWS operation.</span></span> 
  
<span data-ttu-id="37f99-105">A operação **GetUserAvailability** fornece informações detalhadas sobre a disponibilidade de um conjunto de usuários, salas e recursos dentro de um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="37f99-105">The **GetUserAvailability** operation provides detailed information about the availability of a set of users, rooms, and resources within a specified time period.</span></span> 
  
## <a name="using-the-getuseravailability-operation"></a><span data-ttu-id="37f99-106">Usando a operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="37f99-106">Using the GetUserAvailability operation</span></span>

<span data-ttu-id="37f99-107">A operação **GetUserAvailability** fornece as informações de disponibilidade do usuário atual em um nível especificado de detalhes.</span><span class="sxs-lookup"><span data-stu-id="37f99-107">The **GetUserAvailability** operation provides current user availability information at a specified level of detail.</span></span> <span data-ttu-id="37f99-108">Aplicativos cliente como Outlook, Outlook Web Access, Outlook Mobile Access e outros usam endereços SMTP para identificar as informações de usuário solicitadas.</span><span class="sxs-lookup"><span data-stu-id="37f99-108">Client applications such as Outlook, Outlook Web Access, Outlook Mobile Access, and others use SMTP addresses to identify the requested user information.</span></span> 
  
<span data-ttu-id="37f99-109">O serviço de disponibilidade expande as listas de distribuição para recuperar o status de disponibilidade de cada membro da lista, desde que o número de caixas de correio na lista de distribuição seja menor que 100, que é o número máximo de identidades que a operação **GetUserAvailability** pode solicitar.</span><span class="sxs-lookup"><span data-stu-id="37f99-109">The Availability service expands distribution lists to retrieve the free/busy status for each member of the list, as long as the number of mailboxes in the distribution list is less than 100, which is the maximum number of identities that the **GetUserAvailability** operation can request.</span></span> <span data-ttu-id="37f99-110">Os status de disponibilidade dos membros da lista de distribuição são mesclados em um único status de disponibilidade para toda a lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="37f99-110">The free/busy statuses of the members of the distribution list are merged into a single free/busy status for the whole distribution list.</span></span> 
  
<span data-ttu-id="37f99-111">Solicitações de aplicativo cliente especificam o período de tempo da consulta de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="37f99-111">Client application requests specify the time period of the availability query.</span></span> <span data-ttu-id="37f99-112">O período de tempo padrão para as informações solicitadas é de 42 dias.</span><span class="sxs-lookup"><span data-stu-id="37f99-112">The default time period for the requested information is 42 days.</span></span> <span data-ttu-id="37f99-113">Se o calendário do usuário contiver compromissos ou reuniões que estejam dentro e fora do período de tempo definido para a consulta, o compromisso será retornado.</span><span class="sxs-lookup"><span data-stu-id="37f99-113">If the user's calendar contains appointments or meetings that are both within and outside the defined time period for the query, the appointment is returned.</span></span> 
  
<span data-ttu-id="37f99-114">O compromisso e os horários de reunião retornados estão no mesmo fuso horário que o aplicativo cliente que está solicitando a reunião.</span><span class="sxs-lookup"><span data-stu-id="37f99-114">The appointment and meeting times that are returned are in the same time zone as the client application that is requesting the meeting.</span></span>
  
<span data-ttu-id="37f99-115">O serviço de disponibilidade processa a solicitação para cada cliente.</span><span class="sxs-lookup"><span data-stu-id="37f99-115">The Availability service processes the request for each client.</span></span> <span data-ttu-id="37f99-116">O serviço expande todos os compromissos recorrentes e retorna o número máximo de detalhes do calendário que o cliente solicitante tem permissão para receber.</span><span class="sxs-lookup"><span data-stu-id="37f99-116">The service expands all the recurring appointments and returns the maximum number of calendar details that the requesting client has permission to receive.</span></span>
  
> [!NOTE]
> <span data-ttu-id="37f99-117">Se a caixa de correio de destino estiver indisponível ou não puder ser encontrada, uma exceção **MailRecipientNotFoundException** será lançada.</span><span class="sxs-lookup"><span data-stu-id="37f99-117">If the target mailbox is unavailable or cannot be found, a **MailRecipientNotFoundException** exception is thrown.</span></span> <span data-ttu-id="37f99-118">O cliente recebe uma mensagem de erro que indica que o destinatário do email não é encontrado no serviço de diretório do Active Directory ou no AD DS (serviços de domínio Active Directory).</span><span class="sxs-lookup"><span data-stu-id="37f99-118">The client receives an error message that states that the mail recipient is not found in the Active Directory directory service or Active Directory Domain Services (AD DS).</span></span> 
  
### <a name="getuseravailability-operation-soap-headers"></a><span data-ttu-id="37f99-119">Cabeçalhos SOAP de operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="37f99-119">GetUserAvailability operation SOAP headers</span></span>

<span data-ttu-id="37f99-120">A operação **GetUserAvailability** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="37f99-120">The **GetUserAvailability** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="37f99-121">**Header**</span><span class="sxs-lookup"><span data-stu-id="37f99-121">**Header**</span></span>|<span data-ttu-id="37f99-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37f99-122">**Element**</span></span>|<span data-ttu-id="37f99-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37f99-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="37f99-124">**Representação**</span><span class="sxs-lookup"><span data-stu-id="37f99-124">**Impersonation**</span></span> <br/> |[<span data-ttu-id="37f99-125">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="37f99-125">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="37f99-126">Identifica o usuário que o cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="37f99-126">Identifies the user whom the client is impersonating.</span></span> <span data-ttu-id="37f99-127">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="37f99-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="37f99-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="37f99-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="37f99-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="37f99-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="37f99-130">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="37f99-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="37f99-131">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="37f99-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="37f99-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="37f99-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="37f99-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="37f99-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="37f99-134">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="37f99-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="37f99-135">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="37f99-135">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="37f99-136">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="37f99-136">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="37f99-137">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="37f99-137">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="37f99-138">Especifica um cabeçalho SOAP que identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="37f99-138">Specifies a SOAP header that identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="37f99-139">Todas as horas retornadas do servidor serão convertidas no fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="37f99-139">All times that are returned from the server will be converted to the specified time zone.</span></span> <span data-ttu-id="37f99-140">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="37f99-140">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a><span data-ttu-id="37f99-141">Exemplo de solicitação GetUserAvailability: obter informações de disponibilidade</span><span class="sxs-lookup"><span data-stu-id="37f99-141">GetUserAvailability request example: Get availability information</span></span>

<span data-ttu-id="37f99-142">O exemplo a seguir de uma solicitação de operação **GetUserAvailability** mostra como obter informações detalhadas de disponibilidade de dois usuários no fuso horário do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="37f99-142">The following example of a **GetUserAvailability** operation request shows how to get detailed availability information for two users in the Pacific Time time zone.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </t:TimeZone>
      <MailboxDataArray>
        <t:MailboxData>
          <t:Email>
            <t:Address>user1@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
        <t:MailboxData>
          <t:Email>
            <t:Address>user2@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
      </MailboxDataArray>
      <t:FreeBusyViewOptions>
        <t:TimeWindow>
          <t:StartTime>2006-10-16T00:00:00</t:StartTime>
          <t:EndTime>2006-10-16T23:59:59</t:EndTime>
        </t:TimeWindow>
        <t:MergedFreeBusyIntervalInMinutes>60</t:MergedFreeBusyIntervalInMinutes>
        <t:RequestedView>DetailedMerged</t:RequestedView>
      </t:FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="37f99-143">Para obter mais informações sobre como recuperar reuniões sugeridas usando o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) , consulte o esquema no diretório virtual do EWS.</span><span class="sxs-lookup"><span data-stu-id="37f99-143">For more information about retrieving suggested meetings by using the [SuggestionsViewOptions](suggestionsviewoptions.md) element, see the schema in the EWS virtual directory.</span></span> 
  
<span data-ttu-id="37f99-144">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="37f99-144">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="37f99-145">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="37f99-145">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
    
- [<span data-ttu-id="37f99-146">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="37f99-146">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="37f99-147">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="37f99-147">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="37f99-148">StandardTime</span><span class="sxs-lookup"><span data-stu-id="37f99-148">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="37f99-149">Bias</span><span class="sxs-lookup"><span data-stu-id="37f99-149">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="37f99-150">Time</span><span class="sxs-lookup"><span data-stu-id="37f99-150">Time</span></span>](time.md)
    
- [<span data-ttu-id="37f99-151">DayOrder</span><span class="sxs-lookup"><span data-stu-id="37f99-151">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="37f99-152">Month</span><span class="sxs-lookup"><span data-stu-id="37f99-152">Month</span></span>](month.md)
    
- [<span data-ttu-id="37f99-153">DayOfWeek (fuso horário)</span><span class="sxs-lookup"><span data-stu-id="37f99-153">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="37f99-154">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="37f99-154">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="37f99-155">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="37f99-155">MailboxDataArray</span></span>](mailboxdataarray.md)
    
- [<span data-ttu-id="37f99-156">MailboxData</span><span class="sxs-lookup"><span data-stu-id="37f99-156">MailboxData</span></span>](mailboxdata.md)
    
- [<span data-ttu-id="37f99-157">Email (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="37f99-157">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
    
- [<span data-ttu-id="37f99-158">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="37f99-158">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="37f99-159">Articipantetype</span><span class="sxs-lookup"><span data-stu-id="37f99-159">AttendeeType</span></span>](attendeetype.md)
    
- [<span data-ttu-id="37f99-160">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="37f99-160">ExcludeConflicts</span></span>](excludeconflicts.md)
    
- [<span data-ttu-id="37f99-161">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="37f99-161">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
    
- [<span data-ttu-id="37f99-162">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="37f99-162">TimeWindow</span></span>](timewindow.md)
    
- [<span data-ttu-id="37f99-163">StartTime</span><span class="sxs-lookup"><span data-stu-id="37f99-163">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="37f99-164">EndTime</span><span class="sxs-lookup"><span data-stu-id="37f99-164">EndTime</span></span>](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a><span data-ttu-id="37f99-165">Resposta de operação GetUserAvailability bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="37f99-165">Successful GetUserAvailability operation response</span></span>

<span data-ttu-id="37f99-166">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de operação **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="37f99-166">The following example shows a successful response to the **GetUserAvailability** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="37f99-167">Os identificadores de eventos de calendário foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37f99-167">The calendar event identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="https://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T06:00:00-07:00</StartTime>
                <EndTime>2006-10-16T06:30:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0</ID>
                  <Subject>Meet with Contoso Account Executives</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T07:00:00-07:00</StartTime>
                <EndTime>2006-10-16T08:00:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>E14B6414B0B</ID>
                  <Subject>Pick up my groceries</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T09:40:00-07:00</StartTime>
                <EndTime>2006-10-16T10:10:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0B1</ID>
                  <Subject>Meet with doctor</Subject>
                  <Location>Kirkland</Location>
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>5</DayOrder>
                  <Month>10</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>4</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>480</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="https://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>5</DayOrder>
                  <Month>10</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>4</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>480</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
      </FreeBusyResponseArray>
    </GetUserAvailabilityResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="37f99-168">As informações de disponibilidade para cada usuário são exibidas em um elemento [FreeBusyResponse](freebusyresponse.md) exclusivo.</span><span class="sxs-lookup"><span data-stu-id="37f99-168">The availability information for each user appears in a unique [FreeBusyResponse](freebusyresponse.md) element.</span></span> <span data-ttu-id="37f99-169">A ordem dos usuários na solicitação de operação **GetUserAvailability** determina a ordem dos dados de disponibilidade para cada usuário na resposta.</span><span class="sxs-lookup"><span data-stu-id="37f99-169">The order of users in the **GetUserAvailability** operation request determines the order of availability data for each user in the response.</span></span> 
  
<span data-ttu-id="37f99-170">Um erro será retornado ao cliente se o número de compromissos no período de tempo definido na consulta for maior do que o número máximo especificado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="37f99-170">An error will be returned to the client if the number of appointments in the time period that is defined in the query is greater than the administrator-specified maximum number.</span></span> <span data-ttu-id="37f99-171">O número máximo padrão de compromissos é de 10.000 instâncias únicas e itens de recorrência expandidos.</span><span class="sxs-lookup"><span data-stu-id="37f99-171">The default maximum number of appointments is 10,000 single instances and expanded recurrence items.</span></span> <span data-ttu-id="37f99-172">Essa propriedade pode ser configurada somente por um administrador.</span><span class="sxs-lookup"><span data-stu-id="37f99-172">This property can be configured only by an administrator.</span></span>
  
<span data-ttu-id="37f99-173">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="37f99-173">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="37f99-174">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="37f99-174">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="37f99-175">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="37f99-175">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
    
- [<span data-ttu-id="37f99-176">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="37f99-176">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
    
- [<span data-ttu-id="37f99-177">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="37f99-177">FreeBusyResponse</span></span>](freebusyresponse.md)
    
- [<span data-ttu-id="37f99-178">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="37f99-178">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="37f99-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="37f99-179">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="37f99-180">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="37f99-180">FreeBusyView</span></span>](freebusyview.md)
    
- [<span data-ttu-id="37f99-181">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="37f99-181">FreeBusyViewType</span></span>](freebusyviewtype.md)
    
- [<span data-ttu-id="37f99-182">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="37f99-182">MergedFreeBusy</span></span>](mergedfreebusy.md)
    
- [<span data-ttu-id="37f99-183">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="37f99-183">CalendarEventArray</span></span>](calendareventarray.md)
    
- [<span data-ttu-id="37f99-184">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="37f99-184">CalendarEvent</span></span>](calendarevent.md)
    
- [<span data-ttu-id="37f99-185">StartTime</span><span class="sxs-lookup"><span data-stu-id="37f99-185">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="37f99-186">EndTime</span><span class="sxs-lookup"><span data-stu-id="37f99-186">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="37f99-187">BusyType</span><span class="sxs-lookup"><span data-stu-id="37f99-187">BusyType</span></span>](busytype.md)
    
- [<span data-ttu-id="37f99-188">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="37f99-188">CalendarEventDetails</span></span>](calendareventdetails.md)
    
- [<span data-ttu-id="37f99-189">ID</span><span class="sxs-lookup"><span data-stu-id="37f99-189">ID</span></span>](id.md)
    
- [<span data-ttu-id="37f99-190">Assunto (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="37f99-190">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
    
- [<span data-ttu-id="37f99-191">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="37f99-191">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
    
- [<span data-ttu-id="37f99-192">Iscumprimento (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="37f99-192">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
    
- [<span data-ttu-id="37f99-193">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="37f99-193">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
    
- [<span data-ttu-id="37f99-194">IsException</span><span class="sxs-lookup"><span data-stu-id="37f99-194">IsException</span></span>](isexception.md)
    
- [<span data-ttu-id="37f99-195">ReminderSet</span><span class="sxs-lookup"><span data-stu-id="37f99-195">IsReminderSet</span></span>](isreminderset.md)
    
- [<span data-ttu-id="37f99-196">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="37f99-196">IsPrivate</span></span>](isprivate.md)
    
- [<span data-ttu-id="37f99-197">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="37f99-197">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
    
- [<span data-ttu-id="37f99-198">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="37f99-198">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="37f99-199">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="37f99-199">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="37f99-200">StandardTime</span><span class="sxs-lookup"><span data-stu-id="37f99-200">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="37f99-201">Bias</span><span class="sxs-lookup"><span data-stu-id="37f99-201">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="37f99-202">Time</span><span class="sxs-lookup"><span data-stu-id="37f99-202">Time</span></span>](time.md)
    
- [<span data-ttu-id="37f99-203">DayOrder</span><span class="sxs-lookup"><span data-stu-id="37f99-203">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="37f99-204">Month</span><span class="sxs-lookup"><span data-stu-id="37f99-204">Month</span></span>](month.md)
    
- [<span data-ttu-id="37f99-205">DayOfWeek (fuso horário)</span><span class="sxs-lookup"><span data-stu-id="37f99-205">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="37f99-206">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="37f99-206">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="37f99-207">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="37f99-207">WorkingPeriodArray</span></span>](workingperiodarray.md)
    
- [<span data-ttu-id="37f99-208">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="37f99-208">WorkingPeriod</span></span>](workingperiod.md)
    
- [<span data-ttu-id="37f99-209">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="37f99-209">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
    
- [<span data-ttu-id="37f99-210">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="37f99-210">StartTimeInMinutes</span></span>](starttimeinminutes.md)
    
- [<span data-ttu-id="37f99-211">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="37f99-211">EndTimeInMinutes</span></span>](endtimeinminutes.md)
    
## <a name="see-also"></a><span data-ttu-id="37f99-212">Confira também</span><span class="sxs-lookup"><span data-stu-id="37f99-212">See also</span></span>

- [<span data-ttu-id="37f99-213">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="37f99-213">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="37f99-214">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="37f99-214">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

