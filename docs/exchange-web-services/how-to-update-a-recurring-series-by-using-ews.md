---
title: Atualizar uma série recorrente usando o EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e61bee9-4840-4773-a0a7-47b11e1fdf59
description: Saiba como modificar compromissos em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: eb40dd60f28a6acf4395d3149744ce7321c34999
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455846"
---
# <a name="update-a-recurring-series-by-using-ews"></a><span data-ttu-id="43a38-103">Atualizar uma série recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="43a38-103">Update a recurring series by using EWS</span></span>

<span data-ttu-id="43a38-104">Saiba como modificar compromissos em uma série recorrente usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="43a38-104">Learn how to modify appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="43a38-105">Você pode usar a API gerenciada do EWS ou o EWS para atualizar uma série recorrente [atualizando a série inteira](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)ou atualizando uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="43a38-105">You can use the EWS Managed API or EWS to update a recurring series by either [updating the entire series](how-to-update-a-recurring-series-by-using-ews-in-exchange.md), or by updating a single occurrence.</span></span> <span data-ttu-id="43a38-106">Neste artigo, discutiremos como atualizar uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="43a38-106">In this article we'll discuss how to update a single occurrence.</span></span>
  
<span data-ttu-id="43a38-107">A modificação de um único compromisso em uma série é muito semelhante à [modificação de um único compromisso de instância](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="43a38-107">Modifying a single appointment in a series is very similar to [modifying a single instance appointment](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="43a38-108">Você usa os mesmos métodos e operações, mas usa a ID de item da ocorrência que você deseja alterar.</span><span class="sxs-lookup"><span data-stu-id="43a38-108">You use the same methods and operations, but you use the item ID of the occurrence you want to change.</span></span>
  
<span data-ttu-id="43a38-109">Quando você altera uma única ocorrência em uma série, essa ocorrência é adicionada a uma matriz de compromissos modificados associados ao mestre recorrente para a série.</span><span class="sxs-lookup"><span data-stu-id="43a38-109">When you change a single occurrence in a series, that occurrence is added to an array of modified appointments associated with the recurring master for the series.</span></span> <span data-ttu-id="43a38-110">Você pode usar a propriedade de API gerenciada do EWS [ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) ou o elemento [ModifiedOccurrences](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) EWS para acessar todos os compromissos em uma série que foram modificados.</span><span class="sxs-lookup"><span data-stu-id="43a38-110">You can use the [Appointment.ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) EWS Managed API property or the [ModifiedOccurrences](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) EWS element to access all the appointments in a series that have been modified.</span></span> 
  
## <a name="modify-a-single-occurrence-in-a-series-by-using-the-ews-managed-api"></a><span data-ttu-id="43a38-111">Modificar uma única ocorrência em uma série usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="43a38-111">Modify a single occurrence in a series by using the EWS Managed API</span></span>

<span data-ttu-id="43a38-112">Para modificar uma única instância em uma série, você:</span><span class="sxs-lookup"><span data-stu-id="43a38-112">To modify a single instance in a series, you:</span></span>
  
1. <span data-ttu-id="43a38-113">Vincule à ocorrência que você deseja modificar usando o método de [compromisso. BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) com o valor de índice do item ou o método de [compromisso. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) com a ID da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="43a38-113">Bind to the occurrence you want to modify by using either the [Appointment.BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method with the item's index value, or the [Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) method with the occurrence's ID.</span></span> <span data-ttu-id="43a38-114">Você obtém essa ID a partir da propriedade [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de um objeto [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) que corresponde à ocorrência ou a partir da propriedade [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.occurrenceinfo.itemid%28v=exchg.80%29.aspx) do objeto [OccurrenceInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.occurrenceinfo%28v=exchg.80%29.aspx) que corresponde à ocorrência.</span><span class="sxs-lookup"><span data-stu-id="43a38-114">You obtain this ID from either the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) property of an [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object that corresponds to the occurrence, or from the [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.occurrenceinfo.itemid%28v=exchg.80%29.aspx) property of the [OccurrenceInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.occurrenceinfo%28v=exchg.80%29.aspx) object that corresponds to the occurrence.</span></span> 
    
2. <span data-ttu-id="43a38-115">Atualize as propriedades no objeto de compromisso da ocorrência.</span><span class="sxs-lookup"><span data-stu-id="43a38-115">Update the properties on the occurrence's Appointment object.</span></span>
    
3. <span data-ttu-id="43a38-116">Salve as alterações no objeto de compromisso da ocorrência usando o método de [compromisso. salvar](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="43a38-116">Save the changes to the occurrence's appointment object by using the [Appointment.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="43a38-117">O exemplo a seguir atualiza um compromisso em uma série recorrente e verifica se o compromisso modificado foi atualizado no mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="43a38-117">The following example updates an appointment in a recurring series and verifies that the modified appointment is updated on the recurring master.</span></span> <span data-ttu-id="43a38-118">Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**.</span><span class="sxs-lookup"><span data-stu-id="43a38-118">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="43a38-119">O `recurrenceMasterId` parâmetro é um identificador associado ao mestre recorrente para que a ocorrência seja modificada.</span><span class="sxs-lookup"><span data-stu-id="43a38-119">The  `recurrenceMasterId` parameter is an identifier associated with the recurring master for the occurrence to modify.</span></span> 
  
```cs
public static ItemId ModifyARecurringSeries(ExchangeService service, ItemId recurrenceMasterId)
{
    Appointment calendarItem = Appointment.Bind(service, recurrenceMasterId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    if (calendarItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        // Get the recurring master from an occurrence in a recurring series with the properties you need.
        recurrMaster = Appointment.Bind(service,
                                        recurrenceMasterId,
                                        new PropertySet(AppointmentSchema.AppointmentType,
                                                        AppointmentSchema.Subject,
                                                        AppointmentSchema.FirstOccurrence,
                                                        AppointmentSchema.LastOccurrence,
                                                        AppointmentSchema.ModifiedOccurrences,
                                                        AppointmentSchema.DeletedOccurrences));
    }
    else
    {
        Console.WriteLine("Item id was not for a recurring master.");
        return recurrenceMasterId;
    }
    // Bind to the second occurrence in the series with the properties to modify.
    Appointment occurrenceToModify = Appointment.BindToOccurrence(service,
                                                                    recurrMaster.Id,
                                                                    2,
                                                                    new PropertySet(AppointmentSchema.Location,
                                                                                    AppointmentSchema.Start,
                                                                                    AppointmentSchema.End,
                                                                                    AppointmentSchema.RequiredAttendees,
                                                                                    AppointmentSchema.Subject));
    // Update the properties you want to change.
    occurrenceToModify.Location = "Helipad of Contoso Bldg 1";
    occurrenceToModify.Start = occurrenceToModify.Start.AddDays(1);
    occurrenceToModify.End = occurrenceToModify.End.AddDays(1);
    occurrenceToModify.RequiredAttendees.Add("Contoso CEO", "sadie@contoso");
    occurrenceToModify.RequiredAttendees.Add("Contoso Head of Research", "ronnie@contoso.com");
    occurrenceToModify.RequiredAttendees.Add("Contoso Head of Security", "alfred@contoso.com");
    occurrenceToModify.Subject = occurrenceToModify.Subject.ToString() + ":Mandatory";
    // Update the occurrence in your calendar folder and send meeting update requests to attendees.
    // This method call results in an UpdateItem request to EWS.
    occurrenceToModify.Update(ConflictResolutionMode.AlwaysOverwrite, SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy);
    // View updated and deleted occurrences on the recurring master prior to retrieving updated information.
    Console.WriteLine("Modified Occurrences prior to updating recurring master: {0}",
                    (recurrMaster.ModifiedOccurrences == null ? "None" : recurrMaster.ModifiedOccurrences.Count.ToString()));
    // Update the recurring master to view the modified and deleted occurrences.
    recurrMaster = Appointment.Bind(service, recurrenceMasterId, new PropertySet(AppointmentSchema.ModifiedOccurrences,
                                                                        AppointmentSchema.DeletedOccurrences));
    // View updated and deleted occurrences on the recurring master after retrieving updated information.
    Console.WriteLine("Modified Occurrences after updating recurring master:\t {0}",
                    (recurrMaster.ModifiedOccurrences == null ? "None" : recurrMaster.ModifiedOccurrences.Count.ToString()));
    return recurrMaster.Id;            
}

```

## <a name="modify-a-single-occurrence-in-a-series-by-using-ews"></a><span data-ttu-id="43a38-120">Modificar uma única ocorrência em uma série usando o EWS</span><span class="sxs-lookup"><span data-stu-id="43a38-120">Modify a single occurrence in a series by using EWS</span></span>

<span data-ttu-id="43a38-121">Modificar uma única instância em uma série é essencialmente o mesmo que modificar um único compromisso de instância.</span><span class="sxs-lookup"><span data-stu-id="43a38-121">Modifying a single instance in a series is essentially the same as modifying a single instance appointment.</span></span> <span data-ttu-id="43a38-122">Você pode especificar a ocorrência a ser alterada usando um [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ou um elemento [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="43a38-122">You can specify the occurrence to change by using either an [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) or an [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="43a38-123">O exemplo a seguir mostra a solicitação de XML quando você usa a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) para atualizar uma ocorrência em uma série recorrente de compromissos.</span><span class="sxs-lookup"><span data-stu-id="43a38-123">The following example shows the request XML when you use the [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to update an occurrence in a recurring series of appointments.</span></span> <span data-ttu-id="43a38-124">O **ItemId** e o **ChangeKey** são reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="43a38-124">The **ItemId** and **ChangeKey** are shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>Helipad of Contoso Bldg 1</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-03-27T19:33:00.000-07:00</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-03-27T20:33:00.000-07:00</t:End>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack@contoso.com</t:Name>
                      <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie@contoso.com</t:Name>
                      <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Magdalena@contoso.com</t:Name>
                      <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso CEO</t:Name>
                      <t:EmailAddress>sadie@contoso</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso Head of Research</t:Name>
                      <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Contoso Head of Security</t:Name>
                      <t:EmailAddress>alfred@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Weekly Update Meeting:Mandatory</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="43a38-125">O servidor responde à solicitação **UpdateItem** com uma mensagem [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a ocorrência foi atualizada com êxito e o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do compromisso atualizado.</span><span class="sxs-lookup"><span data-stu-id="43a38-125">The server responds to the **UpdateItem** request with an [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the occurrence was updated successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the updated appointment.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="43a38-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="43a38-126">See also</span></span>


- [<span data-ttu-id="43a38-127">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43a38-127">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="43a38-128">Atualizar compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43a38-128">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="43a38-129">Padrões de recorrência e EWS</span><span class="sxs-lookup"><span data-stu-id="43a38-129">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="43a38-130">Acessar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43a38-130">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="43a38-131">Criar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43a38-131">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="43a38-132">Excluir compromissos em uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43a38-132">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="43a38-133">Atualizar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43a38-133">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

