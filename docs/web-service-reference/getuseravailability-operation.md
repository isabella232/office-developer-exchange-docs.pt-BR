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
description: Encontre informações sobre o EWS GetUserAvailability operação.
ms.openlocfilehash: 41246fe22bfb7444cd4aa7b1d4651d475dd9231c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823686"
---
# <a name="getuseravailability-operation"></a><span data-ttu-id="14661-103">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="14661-103">GetUserAvailability operation</span></span>

<span data-ttu-id="14661-104">Encontre informações sobre a operação de EWS **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="14661-104">Find information about the **GetUserAvailability** EWS operation.</span></span> 
  
<span data-ttu-id="14661-105">A operação **GetUserAvailability** fornece informações detalhadas sobre a disponibilidade de um conjunto de usuários, salas e recursos em um período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="14661-105">The **GetUserAvailability** operation provides detailed information about the availability of a set of users, rooms, and resources within a specified time period.</span></span> 
  
## <a name="using-the-getuseravailability-operation"></a><span data-ttu-id="14661-106">Usando a operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="14661-106">Using the GetUserAvailability operation</span></span>

<span data-ttu-id="14661-107">A operação **GetUserAvailability** fornece informações de disponibilidade do usuário atual em um nível especificado de detalhes.</span><span class="sxs-lookup"><span data-stu-id="14661-107">The **GetUserAvailability** operation provides current user availability information at a specified level of detail.</span></span> <span data-ttu-id="14661-108">Aplicativos cliente como o Outlook, Outlook Web Access, Outlook Mobile Access e outras pessoas usam endereços SMTP para identificar as informações de usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="14661-108">Client applications such as Outlook, Outlook Web Access, Outlook Mobile Access, and others use SMTP addresses to identify the requested user information.</span></span> 
  
<span data-ttu-id="14661-109">O serviço de disponibilidade expande listas de distribuição para recuperar o status livre/ocupado para cada membro da lista, desde que o número de caixas de correio na lista de distribuição é menor do que 100, que é o número máximo de identidades que o **GetUserAvailability **operação pode solicitar.</span><span class="sxs-lookup"><span data-stu-id="14661-109">The Availability service expands distribution lists to retrieve the free/busy status for each member of the list, as long as the number of mailboxes in the distribution list is less than 100, which is the maximum number of identities that the **GetUserAvailability** operation can request.</span></span> <span data-ttu-id="14661-110">Os status livre/ocupado dos membros da lista de distribuição são mesclados em um único status livre/ocupado para a lista de distribuição de toda.</span><span class="sxs-lookup"><span data-stu-id="14661-110">The free/busy statuses of the members of the distribution list are merged into a single free/busy status for the whole distribution list.</span></span> 
  
<span data-ttu-id="14661-111">As solicitações do aplicativo cliente especificam o período de tempo da consulta disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="14661-111">Client application requests specify the time period of the availability query.</span></span> <span data-ttu-id="14661-112">O padrão o período de tempo para as informações solicitadas é 42 dias.</span><span class="sxs-lookup"><span data-stu-id="14661-112">The default time period for the requested information is 42 days.</span></span> <span data-ttu-id="14661-113">Se o calendário do usuário contiver compromissos ou reuniões que estão dentro e fora do período de tempo definido para a consulta, o compromisso será retornado.</span><span class="sxs-lookup"><span data-stu-id="14661-113">If the user's calendar contains appointments or meetings that are both within and outside the defined time period for the query, the appointment is returned.</span></span> 
  
<span data-ttu-id="14661-114">Os horários de compromissos e reuniões que são retornados estão no mesmo fuso horário como aplicativo cliente que está solicitando a reunião.</span><span class="sxs-lookup"><span data-stu-id="14661-114">The appointment and meeting times that are returned are in the same time zone as the client application that is requesting the meeting.</span></span>
  
<span data-ttu-id="14661-115">O serviço de disponibilidade processa a solicitação para cada cliente.</span><span class="sxs-lookup"><span data-stu-id="14661-115">The Availability service processes the request for each client.</span></span> <span data-ttu-id="14661-116">O serviço expande todos os compromissos recorrentes e retorna o número máximo de detalhes do calendário que o cliente solicitante tem permissão para receber.</span><span class="sxs-lookup"><span data-stu-id="14661-116">The service expands all the recurring appointments and returns the maximum number of calendar details that the requesting client has permission to receive.</span></span>
  
> [!NOTE]
> <span data-ttu-id="14661-117">Se a caixa de correio de destino não está disponível ou não pode ser encontrada, uma exceção **MailRecipientNotFoundException** é lançada.</span><span class="sxs-lookup"><span data-stu-id="14661-117">If the target mailbox is unavailable or cannot be found, a **MailRecipientNotFoundException** exception is thrown.</span></span> <span data-ttu-id="14661-118">O cliente recebe uma mensagem de erro que afirma que o destinatário do email não foi encontrado no serviço de diretório do Active Directory ou serviços de domínio Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="14661-118">The client receives an error message that states that the mail recipient is not found in the Active Directory directory service or Active Directory Domain Services (AD DS).</span></span> 
  
### <a name="getuseravailability-operation-soap-headers"></a><span data-ttu-id="14661-119">Cabeçalhos SOAP GetUserAvailability operação</span><span class="sxs-lookup"><span data-stu-id="14661-119">GetUserAvailability operation SOAP headers</span></span>

<span data-ttu-id="14661-120">A operação **GetUserAvailability** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="14661-120">The **GetUserAvailability** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="14661-121">**Header**</span><span class="sxs-lookup"><span data-stu-id="14661-121">**Header**</span></span>|<span data-ttu-id="14661-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="14661-122">**Element**</span></span>|<span data-ttu-id="14661-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14661-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="14661-124">**Representação**</span><span class="sxs-lookup"><span data-stu-id="14661-124">**Impersonation**</span></span> <br/> |[<span data-ttu-id="14661-125">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="14661-125">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="14661-126">Identifica o usuário para o qual o cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="14661-126">Identifies the user whom the client is impersonating.</span></span> <span data-ttu-id="14661-127">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="14661-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="14661-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="14661-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="14661-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="14661-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="14661-130">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="14661-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="14661-131">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="14661-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="14661-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="14661-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="14661-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="14661-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="14661-134">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="14661-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="14661-135">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="14661-135">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="14661-136">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="14661-136">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="14661-137">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="14661-137">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="14661-138">Especifica um cabeçalho SOAP que identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="14661-138">Specifies a SOAP header that identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="14661-139">Todos os horários que são retornados do servidor serão convertidos para o fuso horário especificado.</span><span class="sxs-lookup"><span data-stu-id="14661-139">All times that are returned from the server will be converted to the specified time zone.</span></span> <span data-ttu-id="14661-140">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="14661-140">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a><span data-ttu-id="14661-141">Exemplo de solicitação de GetUserAvailability: obter informações de disponibilidade</span><span class="sxs-lookup"><span data-stu-id="14661-141">GetUserAvailability request example: Get availability information</span></span>

<span data-ttu-id="14661-142">O exemplo a seguir de uma solicitação de operação **GetUserAvailability** mostra como obter as informações de disponibilidade detalhadas para dois usuários no fuso horário hora do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="14661-142">The following example of a **GetUserAvailability** operation request shows how to get detailed availability information for two users in the Pacific Time time zone.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="14661-143">Para obter mais informações sobre como recuperar sugeridos reuniões usando o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) , consulte o esquema no diretório virtual EWS.</span><span class="sxs-lookup"><span data-stu-id="14661-143">For more information about retrieving suggested meetings by using the [SuggestionsViewOptions](suggestionsviewoptions.md) element, see the schema in the EWS virtual directory.</span></span> 
  
<span data-ttu-id="14661-144">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="14661-144">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="14661-145">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="14661-145">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
    
- [<span data-ttu-id="14661-146">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="14661-146">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="14661-147">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="14661-147">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="14661-148">StandardTime</span><span class="sxs-lookup"><span data-stu-id="14661-148">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="14661-149">Bias</span><span class="sxs-lookup"><span data-stu-id="14661-149">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="14661-150">Time</span><span class="sxs-lookup"><span data-stu-id="14661-150">Time</span></span>](time.md)
    
- [<span data-ttu-id="14661-151">DayOrder</span><span class="sxs-lookup"><span data-stu-id="14661-151">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="14661-152">Month</span><span class="sxs-lookup"><span data-stu-id="14661-152">Month</span></span>](month.md)
    
- [<span data-ttu-id="14661-153">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="14661-153">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="14661-154">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="14661-154">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="14661-155">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="14661-155">MailboxDataArray</span></span>](mailboxdataarray.md)
    
- [<span data-ttu-id="14661-156">MailboxData</span><span class="sxs-lookup"><span data-stu-id="14661-156">MailboxData</span></span>](mailboxdata.md)
    
- [<span data-ttu-id="14661-157">Email (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="14661-157">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
    
- [<span data-ttu-id="14661-158">Endereço (string)</span><span class="sxs-lookup"><span data-stu-id="14661-158">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="14661-159">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="14661-159">AttendeeType</span></span>](attendeetype.md)
    
- [<span data-ttu-id="14661-160">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="14661-160">ExcludeConflicts</span></span>](excludeconflicts.md)
    
- [<span data-ttu-id="14661-161">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="14661-161">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
    
- [<span data-ttu-id="14661-162">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="14661-162">TimeWindow</span></span>](timewindow.md)
    
- [<span data-ttu-id="14661-163">StartTime</span><span class="sxs-lookup"><span data-stu-id="14661-163">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="14661-164">EndTime</span><span class="sxs-lookup"><span data-stu-id="14661-164">EndTime</span></span>](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a><span data-ttu-id="14661-165">Resposta de operação GetUserAvailability bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="14661-165">Successful GetUserAvailability operation response</span></span>

<span data-ttu-id="14661-166">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de operação **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="14661-166">The following example shows a successful response to the **GetUserAvailability** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="14661-167">Os identificadores de eventos de calendário foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14661-167">The calendar event identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="14661-168">As informações de disponibilidade para cada usuário é exibida em um elemento [FreeBusyResponse](freebusyresponse.md) exclusivo.</span><span class="sxs-lookup"><span data-stu-id="14661-168">The availability information for each user appears in a unique [FreeBusyResponse](freebusyresponse.md) element.</span></span> <span data-ttu-id="14661-169">A ordem dos usuários na solicitação de operação **GetUserAvailability** determina a ordem dos dados de disponibilidade para cada usuário na resposta.</span><span class="sxs-lookup"><span data-stu-id="14661-169">The order of users in the **GetUserAvailability** operation request determines the order of availability data for each user in the response.</span></span> 
  
<span data-ttu-id="14661-170">Um erro será retornado ao cliente se o número de compromissos no período de tempo definido na consulta for maior que o número máximo especificado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="14661-170">An error will be returned to the client if the number of appointments in the time period that is defined in the query is greater than the administrator-specified maximum number.</span></span> <span data-ttu-id="14661-171">O número máximo de padrão de compromissos é 10.000 instâncias única e expandida itens de recorrência.</span><span class="sxs-lookup"><span data-stu-id="14661-171">The default maximum number of appointments is 10,000 single instances and expanded recurrence items.</span></span> <span data-ttu-id="14661-172">Essa propriedade pode ser configurada apenas por um administrador.</span><span class="sxs-lookup"><span data-stu-id="14661-172">This property can be configured only by an administrator.</span></span>
  
<span data-ttu-id="14661-173">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="14661-173">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="14661-174">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="14661-174">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="14661-175">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="14661-175">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
    
- [<span data-ttu-id="14661-176">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="14661-176">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
    
- [<span data-ttu-id="14661-177">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="14661-177">FreeBusyResponse</span></span>](freebusyresponse.md)
    
- [<span data-ttu-id="14661-178">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14661-178">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="14661-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="14661-179">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="14661-180">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="14661-180">FreeBusyView</span></span>](freebusyview.md)
    
- [<span data-ttu-id="14661-181">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="14661-181">FreeBusyViewType</span></span>](freebusyviewtype.md)
    
- [<span data-ttu-id="14661-182">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="14661-182">MergedFreeBusy</span></span>](mergedfreebusy.md)
    
- [<span data-ttu-id="14661-183">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="14661-183">CalendarEventArray</span></span>](calendareventarray.md)
    
- [<span data-ttu-id="14661-184">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="14661-184">CalendarEvent</span></span>](calendarevent.md)
    
- [<span data-ttu-id="14661-185">StartTime</span><span class="sxs-lookup"><span data-stu-id="14661-185">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="14661-186">EndTime</span><span class="sxs-lookup"><span data-stu-id="14661-186">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="14661-187">BusyType</span><span class="sxs-lookup"><span data-stu-id="14661-187">BusyType</span></span>](busytype.md)
    
- [<span data-ttu-id="14661-188">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="14661-188">CalendarEventDetails</span></span>](calendareventdetails.md)
    
- [<span data-ttu-id="14661-189">ID DO</span><span class="sxs-lookup"><span data-stu-id="14661-189">ID</span></span>](id.md)
    
- [<span data-ttu-id="14661-190">Assunto (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="14661-190">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
    
- [<span data-ttu-id="14661-191">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="14661-191">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
    
- [<span data-ttu-id="14661-192">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="14661-192">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
    
- [<span data-ttu-id="14661-193">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="14661-193">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
    
- [<span data-ttu-id="14661-194">IsException</span><span class="sxs-lookup"><span data-stu-id="14661-194">IsException</span></span>](isexception.md)
    
- [<span data-ttu-id="14661-195">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="14661-195">IsReminderSet</span></span>](isreminderset.md)
    
- [<span data-ttu-id="14661-196">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="14661-196">IsPrivate</span></span>](isprivate.md)
    
- [<span data-ttu-id="14661-197">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="14661-197">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
    
- [<span data-ttu-id="14661-198">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="14661-198">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="14661-199">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="14661-199">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="14661-200">StandardTime</span><span class="sxs-lookup"><span data-stu-id="14661-200">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="14661-201">Bias</span><span class="sxs-lookup"><span data-stu-id="14661-201">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="14661-202">Time</span><span class="sxs-lookup"><span data-stu-id="14661-202">Time</span></span>](time.md)
    
- [<span data-ttu-id="14661-203">DayOrder</span><span class="sxs-lookup"><span data-stu-id="14661-203">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="14661-204">Month</span><span class="sxs-lookup"><span data-stu-id="14661-204">Month</span></span>](month.md)
    
- [<span data-ttu-id="14661-205">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="14661-205">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="14661-206">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="14661-206">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="14661-207">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="14661-207">WorkingPeriodArray</span></span>](workingperiodarray.md)
    
- [<span data-ttu-id="14661-208">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="14661-208">WorkingPeriod</span></span>](workingperiod.md)
    
- [<span data-ttu-id="14661-209">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="14661-209">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
    
- [<span data-ttu-id="14661-210">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="14661-210">StartTimeInMinutes</span></span>](starttimeinminutes.md)
    
- [<span data-ttu-id="14661-211">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="14661-211">EndTimeInMinutes</span></span>](endtimeinminutes.md)
    
## <a name="see-also"></a><span data-ttu-id="14661-212">Confira também</span><span class="sxs-lookup"><span data-stu-id="14661-212">See also</span></span>

- [<span data-ttu-id="14661-213">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="14661-213">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="14661-214">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="14661-214">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

