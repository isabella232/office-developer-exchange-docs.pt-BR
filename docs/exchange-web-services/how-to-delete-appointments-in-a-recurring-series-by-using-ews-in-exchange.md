---
title: Excluir compromissos em uma série recorrente usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Saiba como excluir compromissos em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 5646a30d218ed4d795044aefe5efea1399d19a79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528122"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Excluir compromissos em uma série recorrente usando o EWS no Exchange

Saiba como excluir compromissos em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.
  
Você pode usar a API gerenciada do EWS ou o EWS para excluir uma série de compromissos ou reuniões ou apenas uma instância na série. O processo que você usa para excluir uma série inteira é essencialmente o mesmo que o processo que você usa para excluir apenas uma única ocorrência. Você usa os mesmos métodos da API gerenciada do EWS ou as operações do EWS que você usa para [excluir um único compromisso ou reunião de instância](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md). A diferença está na ID do item incluída no método ou na operação. Vamos começar examinando como os dois cenários são os mesmos. 
  
Para excluir uma série recorrente ou uma única ocorrência em uma série recorrente, você precisa localizar a ocorrência ou a série que deseja excluir e, em seguida, chamar o método ou a operação apropriado para removê-lo. Embora seja possível simplesmente excluir qualquer tipo de compromisso, recomendamos que você mantenha todos os participantes ou o organizador atualizado e cancele as reuniões que o usuário organizou e recuse reuniões que o usuário não organizou.
  
Então, como os cenários são diferentes? É tudo sobre o objeto [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) usado para invocar o método (para a API gerenciada do EWS) ou a ID do item incluída na solicitação de operação (para EWS). Para excluir uma série inteira, você precisa do objeto **compromisso** ou ID do item para o mestre recorrente. Para excluir uma única ocorrência, você precisará do objeto **compromisso** ou da ID do item da ocorrência. 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>Excluir um compromisso recorrente usando a API gerenciada do EWS

Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**. O parâmetro _recurringItem_ é um objeto de **compromisso** para o mestre recorrente ou uma única ocorrência. O parâmetro _deleteEntireSeries_ indica se é para excluir a série inteira à qual o _recurringItem_ faz parte. 
  
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

Para usar este exemplo, você precisa [associar a uma ocorrência ou ao mestre recorrente](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)e passar o objeto de **compromisso** resultante para o método. Tenha em mente que, se você acessar compromissos usando uma classe [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , os itens resultantes serão todas as ocorrências únicas. Por outro lado, se você usar a classe [doview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , os itens resultantes serão todos os mestres recorrentes. 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>Excluir um compromisso recorrente usando o EWS

Excluir uma série recorrente usando o EWS é o mesmo que [excluir uma reunião de instância única](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md). Na verdade, as solicitações SOAP têm o mesmo formato. Novamente, a chave é a ID do item usada na solicitação. Se a ID do item corresponder ao mestre recorrente, a série inteira será excluída. Se a ID do item corresponder a uma única ocorrência, apenas essa ocorrência será excluída.
  
> [!NOTE]
> Nos exemplos de código a seguir, os atributos **ItemId**, **ChangeKey**e **recurringMasterId** são reduzidos para legibilidade. 
  
Este exemplo usa a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) com um elemento [CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) para cancelar uma reunião para a qual o usuário é o organizador. O valor do elemento [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indica o item a ser cancelado e pode ser a ID de item de um mestre recorrente ou uma única ocorrência. 
  
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

Este exemplo usa a **operação CreateItem** com um elemento [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) para recusar uma reunião para a qual o usuário não é o organizador. Como no exemplo anterior, o valor do elemento **ReferenceItemId** indica o item a ser recusado e pode ser a ID do item de um mestre recorrente ou uma única ocorrência. 
  
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

Este exemplo usa a [Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) para excluir uma única ocorrência de um compromisso sem participantes. A ocorrência a ser excluída é especificada pelo elemento [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , que é construído a partir da ID de item do mestre recorrente e do índice da ocorrência. 
  
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

Observe que você pode obter o mesmo resultado substituindo o elemento **OccurrenceItemId** por um elemento [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) que contém a ID do item da ocorrência, conforme mostrado. 
  
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
    

