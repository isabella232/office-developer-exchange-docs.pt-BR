---
title: Calendários e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Saiba mais sobre pastas de calendário, calendários e itens, compromissos e reuniões no Exchange.
ms.openlocfilehash: bb9702118ff1db66862a5788c2d8f58dd55c4d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750644"
---
# <a name="calendars-and-ews-in-exchange"></a>Calendários e EWS no Exchange

Saiba mais sobre pastas de calendário, calendários e itens, compromissos e reuniões no Exchange.
  
Você provavelmente está familiarizado com muitos dos recursos de calendário em clientes de email como o Outlook, que permitem controlar compromissos, agendar reuniões, verifique a disponibilidade de pessoas, convidar participantes e alterar ou cancelar reuniões.
  
Recursos relacionados ao calendário no Exchange são um pouco diferentes do que você vê um cliente como o Outlook. Em vez de exiba informações, EWS no Exchange permite que você faça coisas como criar, armazenar, enviar ou alterar as informações. Para usar o EWS para trabalhar com calendários, você precisará estar familiarizado com os conceitos, como o armazenamento de informações, tempo, recorrência e fluxo de mensagens. Mais especificamente, você precisará estar familiarizado com os seguintes itens:
  
- Pastas de calendário, itens de calendário e exibições de calendário
    
- Solicitações de reunião, respostas, agendamento, participantes, recursos, salas e disponibilidade
    
- Durações de tempo, fusos horários e as horas de início e término de reuniões e compromissos
    
- Série recorrente, os padrões de recorrência, exceções e compromissos de única instância e reuniões
    
Felizmente, EWS e a API gerenciada de EWS fornecem um rico conjunto de operações e métodos que permitem que você realize uma ampla variedade de tarefas relacionadas ao calendário. Por exemplo, usando a API gerenciada de EWS, você pode criar uma reunião e enviar convites para os participantes com apenas algumas linhas de código, conforme mostrado no exemplo a seguir.
  
```cs
            Appointment meeting = new Appointment(service);
            // Set the properties on the meeting object to create the meeting.
            meeting.Subject = "Team building exercise";
            meeting.Body = "Let's learn to really work as a team and then have lunch!";
            meeting.Start = DateTime.Now.AddDays(2);
            meeting.End = meeting.Start.AddHours(2);
            meeting.Location = "Conference Room 12";
            meeting.RequiredAttendees.Add("Mack.Chaves@contoso.com");
            meeting.RequiredAttendees.Add("Sadie.Daniels@contoso.com");
            meeting.OptionalAttendees.Add("Magdalena.Kemp@contoso.com");
            meeting.ReminderMinutesBeforeStart = 60;
            // Send the meeting request
            meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);

```

## <a name="calendar-folders-and-calendar-items"></a>Pastas de calendário e itens de calendário
<a name="bk_CalendarFolder"> </a>

Pastas de calendário contêm itens de calendário. Pastas de calendário têm uma [classe de pasta](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) de **IPF. Compromisso**e pode incluir apenas os itens definidos pela propriedade [ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API, que é associada a um objeto de [Classe de compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou o elemento do EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) . 
  
Itens em uma pasta de calendário são um pouco diferentes de itens em outras pastas em uma caixa de correio, pois ocorrências em uma série recorrente e exceções a uma série recorrente não são reais itens na caixa de correio, mas em vez disso, são armazenadas internamente como anexos para um recorrente mestre. Portanto, para recuperar todos os compromissos em um intervalo de datas determinado, você precisará usar um modo de exibição de calendário. Para saber mais sobre como recuperar compromissos e modos de exibição de calendário, consulte [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="meetings-and-appointments"></a>Reuniões e compromissos
<a name="bk_meetings"> </a>

A diferença essencial entre reuniões e compromissos é que reuniões possuem participantes, e não de compromissos. Internamente, o Exchange usa o mesmo objeto para reuniões e compromissos. Use a API gerenciada de EWS [classe de compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou o elemento do EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) para trabalhar com compromissos e reuniões. 
  
Compromissos e reuniões podem ser instâncias única ou parte de uma [série recorrente](recurrence-patterns-and-ews.md), mas como compromissos não incluem os participantes, salas ou recursos, eles não exigem uma mensagem a ser enviada.
  
Como reuniões incluem o envio e responder às solicitações e atualizações, eles envolvem acessando mais do que apenas os itens em uma pasta de calendário. Eles também têm um fluxo de trabalho associado. Reuniões devem ser agendados quando os participantes estão disponíveis e também podem envolver reservar uma sala de reunião ou recursos como um projetor ou outros equipamentos.
  
O fluxo de trabalho de reunião geralmente envolve as seguintes etapas:
  
1. Uma reunião é criada e preenchida com informações como início e hora de término, local e corpo da mensagem.
    
2. Uma lista de participantes em potencial, recursos e salas é criada.
    
3. O status de disponibilidade dos participantes é verificado. 
    
4. Uma solicitação de reunião é enviada aos participantes.
    
5. Participantes respondam à solicitação de reunião com seu intenção participar ou não. Os participantes também podem propor um novo horário para a reunião.
    
6. Reuniões podem ser cancelados ou atualizados, que normalmente acionam novas mensagens sejam enviadas aos participantes.
    
## <a name="calendars-and-time"></a>Calendários e hora
<a name="bk_Time"> </a>

Funcionalidade de tempo é parte do calendário. Compromissos e reuniões tem início e término, durações e outras propriedades relacionadas ao tempo, como a hora em que uma mensagem é criada, enviada e recebida. Reuniões e compromissos existentes podem ser recuperadas de uma pasta de calendário com base em uma hora de início e término. Série recorrente tem inícios e terminará. E reuniões ocorrerem em uma zona de tempo determinada, que é cada vez mais importante em uma economia global.
  
Horas são armazenadas internamente em um servidor do Exchange no tempo Universal Coordenado (UTC). Exchange converte-los para o fuso horário local com base nas configurações de cliente. Propriedades de [DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) limitam-se à zona de hora local do computador. 
  
## <a name="recurring-series"></a>Série recorrente
<a name="bk_recurrence"> </a>

Uma série recorrente de compromissos ou reuniões é composta de um mestre recorrente, um conjunto de itens de ocorrência e, opcionalmente, um conjunto de itens de exceção. Informações de recorrência são armazenadas no item mestre recorrente. O elemento EWS [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) é associado a ocorrências e exceções em uma série ou você pode usar o método [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API para obter o recorrente mestre. Usando uma instância de uma série, você pode encontrar todos os elementos e informações associadas a série. 
  
Observe que as propriedades de recorrência existirem em todos os itens de calendário, mas eles são preenchidos somente em itens recorrentes de mestres. Além de um índice de todas as ocorrências de uma série, o mestre recorrente tem uma referência ao ocorrências excluídas e modificadas e o padrão de recorrência de uma série (por exemplo, diariamente, semanalmente, mensalmente ou anualmente).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Criar eventos de dia inteiro usando o EWS no Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Obtenha os compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [Obter listas de sala, usando o EWS no Exchange](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [Obter informações de disponibilidade usando o EWS no Exchange](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [Propor um novo horário de reunião usando o EWS no Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [Processar itens de calendário em lotes no Exchange](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [Padrões de recorrência e EWS](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    

