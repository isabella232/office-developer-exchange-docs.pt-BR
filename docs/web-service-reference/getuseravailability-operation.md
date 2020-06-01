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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458219"
---
# <a name="getuseravailability-operation"></a>Operação GetUserAvailability

Encontre informações sobre a operação do EWS do **GetUserAvailability** . 
  
A operação **GetUserAvailability** fornece informações detalhadas sobre a disponibilidade de um conjunto de usuários, salas e recursos dentro de um período de tempo especificado. 
  
## <a name="using-the-getuseravailability-operation"></a>Usando a operação GetUserAvailability

A operação **GetUserAvailability** fornece as informações de disponibilidade do usuário atual em um nível especificado de detalhes. Aplicativos cliente como Outlook, Outlook Web Access, Outlook Mobile Access e outros usam endereços SMTP para identificar as informações de usuário solicitadas. 
  
O serviço de disponibilidade expande as listas de distribuição para recuperar o status de disponibilidade de cada membro da lista, desde que o número de caixas de correio na lista de distribuição seja menor que 100, que é o número máximo de identidades que a operação **GetUserAvailability** pode solicitar. Os status de disponibilidade dos membros da lista de distribuição são mesclados em um único status de disponibilidade para toda a lista de distribuição. 
  
Solicitações de aplicativo cliente especificam o período de tempo da consulta de disponibilidade. O período de tempo padrão para as informações solicitadas é de 42 dias. Se o calendário do usuário contiver compromissos ou reuniões que estejam dentro e fora do período de tempo definido para a consulta, o compromisso será retornado. 
  
O compromisso e os horários de reunião retornados estão no mesmo fuso horário que o aplicativo cliente que está solicitando a reunião.
  
O serviço de disponibilidade processa a solicitação para cada cliente. O serviço expande todos os compromissos recorrentes e retorna o número máximo de detalhes do calendário que o cliente solicitante tem permissão para receber.
  
> [!NOTE]
> Se a caixa de correio de destino estiver indisponível ou não puder ser encontrada, uma exceção **MailRecipientNotFoundException** será lançada. O cliente recebe uma mensagem de erro que indica que o destinatário do email não é encontrado no serviço de diretório do Active Directory ou no AD DS (serviços de domínio Active Directory). 
  
### <a name="getuseravailability-operation-soap-headers"></a>Cabeçalhos SOAP de operação GetUserAvailability

A operação **GetUserAvailability** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Header**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Especifica um cabeçalho SOAP que identifica o fuso horário a ser usado para todas as respostas do servidor. Todas as horas retornadas do servidor serão convertidas no fuso horário especificado. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a>Exemplo de solicitação GetUserAvailability: obter informações de disponibilidade

O exemplo a seguir de uma solicitação de operação **GetUserAvailability** mostra como obter informações detalhadas de disponibilidade de dois usuários no fuso horário do Pacífico. 
  
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

Para obter mais informações sobre como recuperar reuniões sugeridas usando o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) , consulte o esquema no diretório virtual do EWS. 
  
O corpo SOAP de solicitação contém os seguintes elementos:
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
    
- [Fuso horário (disponibilidade)](timezone-availability.md)
    
- [Bias (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Time](time.md)
    
- [DayOrder](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (fuso horário)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [MailboxDataArray](mailboxdataarray.md)
    
- [MailboxData](mailboxdata.md)
    
- [Email (EmailAddresstype)](email-emailaddresstype.md)
    
- [Endereço (cadeia de caracteres)](address-string.md)
    
- [Articipantetype](attendeetype.md)
    
- [ExcludeConflicts](excludeconflicts.md)
    
- [FreeBusyViewOptions](freebusyviewoptions.md)
    
- [TimeWindow](timewindow.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a>Resposta de operação GetUserAvailability bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de operação **GetUserAvailability** . 
  
> [!NOTE]
> Os identificadores de eventos de calendário foram reduzidos para preservar a legibilidade. 
  
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

As informações de disponibilidade para cada usuário são exibidas em um elemento [FreeBusyResponse](freebusyresponse.md) exclusivo. A ordem dos usuários na solicitação de operação **GetUserAvailability** determina a ordem dos dados de disponibilidade para cada usuário na resposta. 
  
Um erro será retornado ao cliente se o número de compromissos no período de tempo definido na consulta for maior do que o número máximo especificado pelo administrador. O número máximo padrão de compromissos é de 10.000 instâncias únicas e itens de recorrência expandidos. Essa propriedade pode ser configurada somente por um administrador.
  
Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
    
- [FreeBusyResponseArray](freebusyresponsearray.md)
    
- [FreeBusyResponse](freebusyresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [FreeBusyView](freebusyview.md)
    
- [FreeBusyViewType](freebusyviewtype.md)
    
- [MergedFreeBusy](mergedfreebusy.md)
    
- [CalendarEventArray](calendareventarray.md)
    
- [CalendarEvent](calendarevent.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [BusyType](busytype.md)
    
- [CalendarEventDetails](calendareventdetails.md)
    
- [ID](id.md)
    
- [Assunto (CalendarEventDetails)](subject-calendareventdetails.md)
    
- [Local (CalendarEventDetails)](location-calendareventdetails.md)
    
- [Iscumprimento (CalendarEventDetails)](ismeeting-calendareventdetails.md)
    
- [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)
    
- [IsException](isexception.md)
    
- [ReminderSet](isreminderset.md)
    
- [IsPrivate](isprivate.md)
    
- [WorkingHours](workinghours-ex15websvcsotherref.md)
    
- [Fuso horário (disponibilidade)](timezone-availability.md)
    
- [Bias (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Time](time.md)
    
- [DayOrder](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (fuso horário)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [WorkingPeriodArray](workingperiodarray.md)
    
- [WorkingPeriod](workingperiod.md)
    
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
    
- [StartTimeInMinutes](starttimeinminutes.md)
    
- [EndTimeInMinutes](endtimeinminutes.md)
    
## <a name="see-also"></a>Também consulte

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Obtendo disponibilidade do usuário](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

