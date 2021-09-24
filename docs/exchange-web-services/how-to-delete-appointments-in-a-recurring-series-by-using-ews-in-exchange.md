---
title: Excluir compromissos em uma série recorrente usando o EWS em Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Saiba como excluir compromissos em uma série recorrente usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 8a68b6655c98f290d569a14dc0ac518c5d875cbe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513189"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Excluir compromissos em uma série recorrente usando o EWS em Exchange

Saiba como excluir compromissos em uma série recorrente usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Você pode usar a API Gerenciada do EWS ou o EWS para excluir uma série de compromissos ou reuniões ou apenas uma instância na série. O processo usado para excluir uma série inteira é essencialmente o mesmo que o processo usado para excluir apenas uma única ocorrência. Você usa os mesmos métodos de API Gerenciada do EWS ou operações EWS que você usa para excluir um compromisso ou reunião de instância [única.](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) A diferença está na ID do item incluída no método ou operação. Vamos começar analisando como ambos os cenários são os mesmos. 
  
Para excluir uma série recorrente ou uma única ocorrência em uma série recorrente, você precisa encontrar a ocorrência ou a série que deseja excluir e, em seguida, chamar o método ou a operação apropriado para removê-la. Embora você possa simplesmente excluir qualquer tipo de compromisso, recomendamos manter todos os participantes ou o organizador atualizados e cancelar reuniões que o usuário organizou e recusar reuniões que o usuário não organizou.
  
Como os cenários são diferentes? Trata-se do objeto [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) usado para invocar o método (para a API Gerenciada do EWS) ou a ID do item incluída na solicitação de operação (para EWS). Para excluir uma série inteira, você precisa da ID do objeto **Appointment** ou do item do mestre recorrente. Para excluir uma única ocorrência, você precisa da ID do objeto **Appointment** ou do item para a ocorrência. 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>Excluir um compromisso recorrente usando a API Gerenciada do EWS

Este exemplo pressupõe que você tenha autenticado em um servidor Exchange e tenha adquirido um [objeto ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **service**. O  _parâmetro recurringItem_ é um **objeto Appointment** para o mestre recorrente ou uma única ocorrência. O  _parâmetro deleteEntireSeries_ indica se é preciso excluir toda a série da que o  _RecurringItem_ faz parte. 
  
```cs
public static bool DeleteRecurringItem(ExchangeService service, Appointment recurringItem, bool deleteEntireSeries)
{
    Appointment appointmentToDelete = null;
    // If the item is a single appointment, fail.
    if (recurringItem.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        if (!deleteEntireSeries)
        {
            // The item is the recurring master, so deleting it will delete
            // the entire series. The caller indicated that the entire series
            // should not be deleted, so fail.
            Console.WriteLine("ERROR: The item to delete is the recurring master of the series. Deleting it will delete the entire series.");
            return false;
        }
        else
        {
            appointmentToDelete = recurringItem;
        }
    }
    else
    {
        if (deleteEntireSeries)
        {
            // The item passed is not the recurring master, but the caller
            // wants to delete the entire series. Bind to the recurring
            // master to delete it.
            try
            {
                appointmentToDelete = Appointment.BindToRecurringMaster(service, recurringItem.Id);
            }
            catch (Exception ex)
            {
                Console.WriteLine("ERROR: {0}", ex.Message);
                return false;
            }
        }
        else
        {
            // The item passed is not the recurring master, but the caller
            // only wants to delete the occurrence, so just
            // delete the passed item.
            appointmentToDelete = recurringItem;
        }
    }
    if (appointmentToDelete != null)
    {
        // Remove the item, depending on the scenario. 
        if (appointmentToDelete.IsMeeting)
        {
            CalendarActionResults results;
            // If it's a meeting and the user is the organizer, cancel it.
            // Determine this by testing the AppointmentState bitmask for 
            // the presence of the second bit. This bit indicates that the appointment
            // was received, which means that someone sent it to the user. Therefore,
            // they're not the organizer.
            int isReceived = 2;
            if ((appointmentToDelete.AppointmentState &amp; isReceived) == 0)
            {
                results = appointmentToDelete.CancelMeeting("Cancelling this meeting.");
                return true;
            }
            // If it's a meeting and the user is not the organizer, decline it.
            else
            {
                results = appointmentToDelete.Decline(true);
                return true;
            }
        }
        else
        {
            // The item isn't a meeting, so just delete it.
            appointmentToDelete.Delete(DeleteMode.MoveToDeletedItems);
            return true;
        }
    }
    return false;
}
```

Para usar este exemplo, você precisa se vincular [a](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)uma ocorrência ou ao mestre recorrente e passar o objeto **Appointment** resultante para o método. Lembre-se de que, se você acessar compromissos usando uma classe [CalendarView,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) os itens resultantes serão todas ocorrências simples. Por outro lado, se você usar a [classe ItemView,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) os itens resultantes serão todos mestres recorrentes. 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>Excluir um compromisso recorrente usando o EWS

Excluir uma série recorrente usando eWS é o mesmo que excluir [uma reunião de instância única.](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md) Na verdade, as solicitações SOAP levam o mesmo formato. Novamente, a chave é a ID do item usada na solicitação. Se a ID do item corresponder ao mestre recorrente, toda a série será excluída. Se a ID do item corresponder a uma única ocorrência, somente essa ocorrência será excluída.
  
> [!NOTE]
> Nos exemplos de código a seguir, os **atributos ItemId,** **ChangeKey** e **RecurringMasterId** são reduzidos para a capacidade de leitura. 
  
Este exemplo usa a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) com um [elemento CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) para cancelar uma reunião para a qual o usuário é o organizador. O valor do [elemento ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indica o item a ser cancelado e pode ser a ID do item de um mestre recorrente ou uma única ocorrência. 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:NewBodyContent BodyType="HTML">Cancelling this meeting.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Este exemplo usa a **operação CreateItem** com um [elemento DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) para recusar uma reunião para a qual o usuário não é o organizador. Como no exemplo anterior, o valor do **elemento ReferenceItemId** indica o item a recusar e pode ser a ID do item de um mestre recorrente ou uma única ocorrência. 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:DeclineItem>
          <t:ReferenceItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
        </t:DeclineItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Este exemplo usa a [operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) para excluir uma única ocorrência de um compromisso sem participantes. A ocorrência a ser excluído é especificada pelo [elemento OccurrenceItemId,](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) que é construído a partir da ID do item do mestre recorrente e do índice da ocorrência. 
  
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
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

Observe que você pode obter o mesmo resultado substituindo o **elemento OccurrenceItemId** por um [elemento ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) que contém a ID do item da ocorrência, conforme mostrado. 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>Confira também


- [Padrões de recorrência e EWS](recurrence-patterns-and-ews.md)
    
- [Acessar uma série recorrente usando o EWS no Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Criar uma série recorrente usando o EWS no Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Atualizar uma série recorrente usando o EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Atualizar uma série recorrente usando o EWS no Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

