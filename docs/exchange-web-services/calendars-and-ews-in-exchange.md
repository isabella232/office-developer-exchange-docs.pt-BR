---
title: Calendários e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Saiba mais sobre calendários, pastas e itens de calendário, compromissos e reuniões no Exchange.
localization_priority: Priority
ms.openlocfilehash: 3312ebb4deeb6645ccd7048564d61c3db5ea4b94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456196"
---
# <a name="calendars-and-ews-in-exchange"></a>Calendários e EWS no Exchange

Saiba mais sobre calendários, pastas e itens de calendário, compromissos e reuniões no Exchange.
  
Você provavelmente está familiarizado com muitos dos recursos de calendário em clientes de email, como o Outlook, que permitem rastrear compromissos, agendar reuniões, verificar a disponibilidade de pessoas, convidar participantes e alterar ou cancelar reuniões.
  
Recursos relacionados ao calendário no Exchange são um pouco diferentes daqueles que você vê em um cliente como o Outlook. Em vez de exibir informações, o EWS no Exchange permite que você faça coisas como criar, armazenar, enviar ou alterar informações. Para usar o EWS para trabalhar com calendários, você precisará estar familiarizado com os conceitos como armazenamento de informações, tempo, recorrência e fluxo de mensagens. Mais especificamente, você precisará estar familiarizado com o seguinte:
  
- Pastas de calendário, itens de calendário e exibições de calendário
    
- Solicitações de reunião, respostas, agendamento, participantes, recursos, salas e disponibilidade
    
- Durações de tempo, fusos horários e horários de início e de término de reuniões e compromissos
    
- Série recorrente, padrões de recorrência, exceções e compromissos e reuniões de instância única
    
Felizmente, o EWS e a API gerenciada do EWS oferecem um conjunto avançado de operações e métodos que permitem que você execute uma ampla variedade de tarefas relacionadas ao calendário. Por exemplo, usando a API gerenciada do EWS, você pode criar uma reunião e enviar convites para os participantes com apenas algumas linhas de código, conforme mostrado no exemplo a seguir.
  
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

As pastas de calendário contêm itens de calendário. As pastas de calendário têm uma [classe de pasta](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) de **IPF. Compromisso**e pode incluir somente os itens definidos pela propriedade da API gerenciada do EWS, que é [associada a um](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) objeto de classe de [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou o elemento [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) do EWS. 
  
Os itens em uma pasta de calendário são um pouco diferentes dos itens em outras pastas em uma caixa de correio, pois as ocorrências em uma série recorrente e exceções a uma série recorrente não são itens reais na caixa de correio, mas sim armazenados internamente como anexos em um mestre recorrente. Portanto, para recuperar todos os compromissos em um determinado intervalo de datas, você precisa usar um modo de exibição de calendário. Para saber mais sobre como recuperar compromissos e modos de exibição de calendário, confira [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="meetings-and-appointments"></a>Reuniões e compromissos
<a name="bk_meetings"> </a>

A diferença essencial entre reuniões e compromissos é que as reuniões têm participantes e compromissos não. Internamente, o Exchange usa o mesmo objeto para reuniões e compromissos. Você usa a [classe de compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) da API gerenciada do EWS ou o elemento [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) do EWS para trabalhar com reuniões e compromissos. 
  
Compromissos e reuniões podem ser instâncias únicas ou parte de uma [série recorrente](recurrence-patterns-and-ews.md), mas como os compromissos não incluem participantes, salas ou recursos, eles não exigem que uma mensagem seja enviada.
  
Como as reuniões incluem enviar e responder a solicitações e atualizações, elas envolvem mais do que simplesmente acessar itens em uma pasta de calendário. Eles também têm um fluxo de trabalho associado. As reuniões devem ser agendadas quando os participantes estão disponíveis e também podem envolver a reserva de uma sala de reunião ou recursos como um projetor ou outro equipamento.
  
O fluxo de trabalho de reunião geralmente envolve as seguintes etapas:
  
1. Uma reunião é criada e preenchida com informações como hora de início e de término, local e corpo da mensagem.
    
2. Uma lista de participantes, recursos e salas potenciais é criada.
    
3. O status de disponibilidade dos participantes é verificado. 
    
4. Uma solicitação de reunião é enviada aos participantes.
    
5. Os participantes respondem à reunião com sua intenção de participar ou não. Os participantes também podem propor um novo horário para a reunião.
    
6. As reuniões podem ser canceladas ou atualizadas, que geralmente disparam novas mensagens a serem enviadas aos participantes.
    
## <a name="calendars-and-time"></a>Calendários e tempo
<a name="bk_Time"> </a>

A funcionalidade relacionada ao tempo é parte integrante do calendário. Compromissos e reuniões têm horários de início e de término, durações e outras propriedades relacionadas a tempo, como a hora em que uma mensagem é criada, enviada e recebida. Compromissos e reuniões existentes podem ser recuperados de uma pasta de calendário com base em uma hora de início e de término. A série recorrente tem início e término. As reuniões ocorrem em um determinado fuso horário, o que é cada vez mais importante em uma economia global.
  
Os horários são armazenados internamente em um servidor do Exchange em tempo universal coordenado (UTC). O Exchange converte-os no fuso horário local com base nas configurações do cliente. As propriedades [DateTime](https://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) têm o escopo para o fuso horário local do computador. 
  
## <a name="recurring-series"></a>Série recorrente
<a name="bk_recurrence"> </a>

Uma série recorrente de compromissos ou reuniões é composta por um mestre recorrente, um conjunto de itens de ocorrência e, opcionalmente, um conjunto de itens de exceção. As informações de recorrência são armazenadas no item mestre recorrente. O elemento [RecurringMasterItemId](https://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS é associado a ocorrências e exceções em uma série ou você pode usar o método de [compromisso. BINDTORECURRINGMASTER](https://msdn.microsoft.com/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API para obter o mestre recorrente. Usando uma instância de uma série, você pode encontrar todos os elementos e informações associados à série. 
  
Observe que as propriedades de recorrência existem em todos os itens de calendário, mas são preenchidas apenas em itens mestres recorrentes. Além de um índice de todas as ocorrências de uma série, o mestre recorrente tem uma referência para ocorrências modificadas e excluídas e o padrão de recorrência de uma série (por exemplo, diariamente, semanalmente, mensal ou anualmente).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Criar eventos de dia inteiro usando o EWS no Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [Obter listas de salas usando o EWS no Exchange](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [Obter informações de disponibilidade usando o EWS no Exchange](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [Propor um novo horário de reunião usando o EWS no Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [Processar itens de calendário em lotes no Exchange](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [Padrões de recorrência e EWS](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

