---
title: Acessar um calendário como um representante usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Saiba como acessar um calendário como um representante usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 20ec294ddc4ccf014f0b2148c786c8c3ef8a6069
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528290"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="74127-103">Acessar um calendário como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74127-103">Access a calendar as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="74127-104">Saiba como acessar um calendário como um representante usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="74127-104">Learn how to access a calendar as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="74127-105">Você pode usar a API gerenciada do EWS ou o EWS para conceder acesso de representante de usuário à pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Calendar folder.</span></span> <span data-ttu-id="74127-106">O representante pode então criar solicitações de reunião em nome do proprietário da caixa de correio, criar compromissos, responder a solicitações de reunião e recuperar, atualizar e excluir reuniões da pasta de calendário do proprietário da caixa de correio, dependendo de suas permissões.</span><span class="sxs-lookup"><span data-stu-id="74127-106">The delegate can then create meeting requests on behalf of the mailbox owner, create appointments, respond to meeting requests, and retrieve, update, and delete meetings from the mailbox owner's Calendar folder, depending on their permissions.</span></span>
  
<span data-ttu-id="74127-107">Como representante, você usa os mesmos métodos e operações para acessar a pasta de calendário do proprietário da caixa de correio que você usa para acessar sua própria pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="74127-107">As a delegate, you use the same methods and operations to access a mailbox owner's Calendar folder that you use to access your own Calendar folder.</span></span> <span data-ttu-id="74127-108">A principal diferença é que você precisa usar o [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de calendário ou subpasta de calendário e depois de identificar a ID de item ou a ID de pasta, você pode usar o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item.</span><span class="sxs-lookup"><span data-stu-id="74127-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a calendar item or calendar subfolder, and then after you identify the item ID or folder ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="74127-109">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para acessar um calendário como um representante**</span><span class="sxs-lookup"><span data-stu-id="74127-109">**Table 1. EWS Managed API methods and EWS operations for accessing a calendar as a delegate**</span></span>

|<span data-ttu-id="74127-110">**Se você quiser...**</span><span class="sxs-lookup"><span data-stu-id="74127-110">**If you want to…**</span></span>|<span data-ttu-id="74127-111">**Use este método de API gerenciada do EWS...**</span><span class="sxs-lookup"><span data-stu-id="74127-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="74127-112">**Use esta operação do EWS...**</span><span class="sxs-lookup"><span data-stu-id="74127-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="74127-113">Criar uma reunião ou um compromisso como um representante</span><span class="sxs-lookup"><span data-stu-id="74127-113">Create a meeting or appointment as a delegate</span></span>  <br/> |<span data-ttu-id="74127-114">[Compromisso. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta calendário do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="74127-114">[Appointment.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="74127-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="74127-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="74127-116">Criar várias reuniões ou compromissos como um representante</span><span class="sxs-lookup"><span data-stu-id="74127-116">Create multiple meetings or appointments as a delegate</span></span>  <br/> |<span data-ttu-id="74127-117">[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta calendário do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="74127-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="74127-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="74127-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="74127-119">Procurar ou localizar um compromisso ou reunião como representante</span><span class="sxs-lookup"><span data-stu-id="74127-119">Search for or find an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="74127-120">[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta calendário do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="74127-120">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="74127-121">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="74127-121">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="74127-122">Obter um compromisso ou reunião como representante</span><span class="sxs-lookup"><span data-stu-id="74127-122">Get an appointment or meeting as a delegate</span></span>  <br/> |[<span data-ttu-id="74127-123">Compromisso. bind</span><span class="sxs-lookup"><span data-stu-id="74127-123">Appointment.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="74127-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="74127-124">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="74127-125">Atualizar um compromisso ou reunião como um representante</span><span class="sxs-lookup"><span data-stu-id="74127-125">Update an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="74127-126">[Compromisso. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido por [compromisso. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="74127-126">[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="74127-127">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="74127-127">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="74127-128">Excluir um compromisso ou reunião como um representante</span><span class="sxs-lookup"><span data-stu-id="74127-128">Delete an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="74127-129">[Compromisso. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido por [compromisso. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="74127-129">[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="74127-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="74127-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="74127-131">Nos exemplos de código deste artigo, primary@contoso.com é o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-131">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="74127-132">Tarefas de pré-requisito</span><span class="sxs-lookup"><span data-stu-id="74127-132">Prerequisite tasks</span></span>
<span data-ttu-id="74127-133"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-133"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="74127-134">Antes que um usuário possa acessar a pasta calendário de um proprietário da caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para a pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-134">Before a user can access a mailbox owner's Calendar folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="74127-135">Um representante deve ter uma caixa de correio anexada à conta para atualizar o calendário de um proprietário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-135">A delegate must have a mailbox attached to their account to update the calendar of a mailbox owner.</span></span>
  
<span data-ttu-id="74127-136">Se um representante precisar trabalhar apenas com solicitações de reunião e respostas, você poderá adicionar o representante à pasta de calendário e usar o valor de enumeração de API gerenciada [MeetingRequestsDeliveryScope. DelegatesAndSendInformationToMe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS padrão ou o valor de elemento [DeliverMeetingRequests](https://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS de **DelegatesAndSendInformationToMe** para enviar as solicitações às mensagens de representante e informativas ao proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-136">If a delegate needs to work with meeting requests and responses only, you can add the delegate to the Calendar folder, and use the default [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API enumeration value or the [DeliverMeetingRequests](https://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS element value of **DelegatesAndSendInformationToMe** to send the requests to the delegate and informational messages to the mailbox owner.</span></span> <span data-ttu-id="74127-137">O representante não precisa ter acesso à pasta caixa de entrada do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-137">The delegate then does not need to be given access to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="74127-138">Criar uma reunião ou um compromisso como um representante usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="74127-138">Create a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="74127-139"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-139"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="74127-140">A API gerenciada do EWS permite que você use o objeto de serviço para que o usuário delegado crie itens de calendário para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-140">The EWS Managed API enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="74127-141">Este exemplo mostra como usar o método [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes.</span><span class="sxs-lookup"><span data-stu-id="74127-141">This example shows how to use the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="74127-142">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e que o representante recebeu as permissões apropriadas para a pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-142">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Calendar folder.</span></span> 
  
```cs
private static void DelegateAccessCreateMeeting(ExchangeService service)
{
    Appointment meeting = new Appointment(service);
    // Set the properties on the meeting object to create the meeting.
    meeting.Subject = "Team building exercise";
    meeting.Body = "Let's learn to really work as a team and then have lunch!";
    meeting.Start = DateTime.Now.AddDays(2);
    meeting.End = meeting.Start.AddHours(4);
    meeting.Location = "Conference Room 12";
    meeting.RequiredAttendees.Add("sadie@contoso.com");
    meeting.ReminderMinutesBeforeStart = 60;
    // Save the meeting to the Calendar folder for 
    // the mailbox owner and send the meeting request.
    // This method call results in a CreateItem call to EWS.
    meeting.Save(new FolderId(WellKnownFolderName.Calendar, 
        "primary@contoso.com"), 
        SendInvitationsMode.SendToAllAndSaveCopy);
    // Verify that the meeting was created.
    Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
    Console.WriteLine("\nMeeting created: " + item.Subject + "\n");
}
```

<span data-ttu-id="74127-143">Observe que, quando você salva o item, a chamada do método [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) deve identificar a pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-143">Note that when you save the item, the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="74127-144">Se a pasta de calendário do proprietário da caixa de correio não for especificada, a solicitação de reunião será salva no calendário do representante e não na pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-144">If the mailbox owner's Calendar folder is not specified, the meeting request gets saved to the delegate's calendar and not the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="74127-145">Você pode incluir a pasta calendário do proprietário da caixa de correio na chamada do método **Save** de duas maneiras.</span><span class="sxs-lookup"><span data-stu-id="74127-145">You can include the mailbox owner's Calendar folder in the **Save** method call in two ways.</span></span> <span data-ttu-id="74127-146">Recomendamos que você instancie uma nova instância do objeto [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) usando o [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-146">We recommend that you instantiate a new instance of the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

<span data-ttu-id="74127-147">No entanto, você também pode [associar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) -se à pasta calendário primeiro e, em seguida, usar a ID da pasta na chamada do método **Save** .</span><span class="sxs-lookup"><span data-stu-id="74127-147">However, you can also [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Calendar folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="74127-148">No entanto, lembre-se de que isso cria uma chamada EWS extra.</span><span class="sxs-lookup"><span data-stu-id="74127-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address
    // and bind to their Calendar folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryCalendar = Folder.Bind(service, 
        new FolderId(WellKnownFolderName.Calendar, primary)); 
…
    // Save the meeting to the Calendar folder for the mailbox owner and send the meeting request.
    meeting.Save(primaryCalendar.Id, 
        SendInvitationsMode.SendToAllAndSaveCopy);
```

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="74127-149">Criar uma reunião ou um compromisso como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="74127-149">Create a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="74127-150"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-150"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="74127-151">O EWS permite que você use o objeto de serviço para que o usuário delegado crie itens de calendário para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-151">EWS enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="74127-152">Este exemplo mostra como usar a operação [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes.</span><span class="sxs-lookup"><span data-stu-id="74127-152">This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="74127-153">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **Save** para [criar uma reunião ou um compromisso como um representante](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="74127-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a meeting or appointment as a delegate](#bk_createewsma).</span></span>
  
<span data-ttu-id="74127-154">O cabeçalho SOAP foi removido do exemplo a seguir por brevidade.</span><span class="sxs-lookup"><span data-stu-id="74127-154">The SOAP header has been removed from the following example for brevity.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
…
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a 
              team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-09T23:26:33.756-05:00</t:Start>
          <t:End>2014-03-10T03:26:33.756-05:00</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="74127-155">O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a reunião foi criada com êxito.</span><span class="sxs-lookup"><span data-stu-id="74127-155">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the meeting was created successfully.</span></span> <span data-ttu-id="74127-156">A resposta também contém a ID do item da reunião recém-criada.</span><span class="sxs-lookup"><span data-stu-id="74127-156">The response also contains the item ID of the newly created meeting.</span></span>
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="74127-157">Pesquisar uma reunião ou um compromisso como um representante usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="74127-157">Search for a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="74127-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-158"><a name="bk_searchewsma"> </a></span></span>

<span data-ttu-id="74127-159">Para pesquisar uma reunião, você deve usar um dos métodos [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você possa especificar a pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-159">To search for a meeting, you must use one of the [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Calendar folder.</span></span> 
  
```cs
static void DelegateAccessSearchWithFilter
    (ExchangeService service, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Define the sort order.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching calendar items. 
        // The FindItems parameters must denote the mailbox owner,
        // mailbox, and Calendar folder.
        // This method call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(
        new FolderId(WellKnownFolderName.Calendar, 
            "primary@contoso.com"), 
            filter, 
            view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while 
            enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="74127-160">Depois que a chamada **FindItems** retorna uma resposta com uma ID, você pode obter, atualizar ou excluir essa reunião usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) — e não é necessário especificar o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that meeting by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="74127-161">Pesquisar uma reunião ou um compromisso como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="74127-161">Search for a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="74127-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-162"><a name="bk_searchews"> </a></span></span>

<span data-ttu-id="74127-163">O EWS permite que você use o objeto de serviço para que o usuário delegado pesquise compromissos e reuniões que atendam a um conjunto de critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="74127-163">EWS enables you to use the service object for the delegate user to search for appointments and meetings that meet a set of search criteria.</span></span> <span data-ttu-id="74127-164">Este exemplo mostra como usar a operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para encontrar reuniões na pasta calendário do proprietário da caixa de correio que contêm a palavra "Building" no assunto.</span><span class="sxs-lookup"><span data-stu-id="74127-164">This example shows how to use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Calendar folder that contain the word "building" in the subject.</span></span> 
  
<span data-ttu-id="74127-165">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **FindItem** para [Pesquisar uma reunião ou um compromisso como um representante](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="74127-165">This is also the XML request that the EWS Managed API sends when you use the **FindItem** method to [search for a meeting or appointment as a delegate](#bk_searchewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="building" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="74127-166">O servidor responde à solicitação **FindItem** com uma mensagem [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pesquisa foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="74127-166">The server responds to the **FindItem** request with a [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="74127-167">A resposta contém um [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) para quaisquer compromissos ou reuniões que atendam aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="74127-167">The response contains a [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) for any appointments or meetings that met the search criteria.</span></span> <span data-ttu-id="74127-168">Nesse caso, somente uma reunião é encontrada.</span><span class="sxs-lookup"><span data-stu-id="74127-168">In this case, only one meeting is found.</span></span> 
  
<span data-ttu-id="74127-169">O valor do elemento [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74127-169">The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="IJpUAAA="
                          ChangeKey="DwAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAAAIKhS" />
                <t:Subject>Team building exercise</t:Subject>
                <t:DateTimeReceived>2014-03-04T21:27:22Z</t:DateTimeReceived>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="74127-170">Agora que você tem o **ItemId** para a reunião que atende aos seus critérios, é possível obter, atualizar ou excluir essa reunião usando o **ItemId** e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) — e não é necessário especificar o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-170">Now that you have the **ItemId** for the meeting that meets your criteria, you can get, update, or delete that meeting by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="74127-171">Obter, atualizar ou excluir itens de calendário como um representante usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="74127-171">Get, update, or delete calendar items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="74127-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-172"><a name="bk_geteswma"> </a></span></span>

<span data-ttu-id="74127-173">Você pode usar a API gerenciada do EWS para obter, atualizar ou excluir uma reunião ou um compromisso da mesma maneira que você executa essas ações quando você não está usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="74127-173">You can use the EWS Managed API to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="74127-174">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="74127-174">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="74127-175">A ID do item incluída na chamada do método **BIND** identifica exclusivamente o item no repositório de caixa de correio, na pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="74127-176">**Tabela 2. Métodos de API gerenciada do EWS para trabalhar com compromissos e reuniões como um representante**</span><span class="sxs-lookup"><span data-stu-id="74127-176">**Table 2. EWS Managed API methods for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="74127-177">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="74127-177">**Task**</span></span>|<span data-ttu-id="74127-178">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="74127-178">**EWS Managed API method**</span></span>|<span data-ttu-id="74127-179">**Exemplo de código**</span><span class="sxs-lookup"><span data-stu-id="74127-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="74127-180">Obter um compromisso ou uma reunião</span><span class="sxs-lookup"><span data-stu-id="74127-180">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="74127-181">Associá</span><span class="sxs-lookup"><span data-stu-id="74127-181">Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="74127-182">Obter um item usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="74127-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="74127-183">Atualizar um compromisso ou uma reunião</span><span class="sxs-lookup"><span data-stu-id="74127-183">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="74127-184">[Vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido por [atualização](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="74127-184">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="74127-185">Atualizar uma reunião usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="74127-185">Update a meeting by using the EWS Managed API</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|<span data-ttu-id="74127-186">Excluir um compromisso ou reunião</span><span class="sxs-lookup"><span data-stu-id="74127-186">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="74127-187">[Vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido por [delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="74127-187">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="74127-188">Excluir uma reunião usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="74127-188">Delete a meeting by using the EWS Managed API</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="74127-189">Obter, atualizar ou excluir itens de calendário como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="74127-189">Get, update, or delete calendar items as a delegate by using EWS</span></span>
<span data-ttu-id="74127-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="74127-190"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="74127-191">Você pode usar o EWS para obter, atualizar ou excluir uma reunião ou um compromisso da mesma maneira que executará essas ações quando não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="74127-191">You can use EWS to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="74127-192">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="74127-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="74127-193">A ID do item incluída na chamada do método [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) identifica exclusivamente o item no repositório de caixa de correio, na pasta calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="74127-193">The item ID included in the [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="74127-194">**Tabela 3. Operações do EWS para trabalhar com compromissos e reuniões como um representante**</span><span class="sxs-lookup"><span data-stu-id="74127-194">**Table 3. EWS operations for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="74127-195">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="74127-195">**Task**</span></span>|<span data-ttu-id="74127-196">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="74127-196">**EWS operation**</span></span>|<span data-ttu-id="74127-197">**Exemplo de código**</span><span class="sxs-lookup"><span data-stu-id="74127-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="74127-198">Obter um compromisso ou uma reunião</span><span class="sxs-lookup"><span data-stu-id="74127-198">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="74127-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="74127-199">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="74127-200">Obter um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="74127-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="74127-201">Atualizar um compromisso ou uma reunião</span><span class="sxs-lookup"><span data-stu-id="74127-201">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="74127-202">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="74127-202">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="74127-203">Atualizar uma reunião usando o EWS</span><span class="sxs-lookup"><span data-stu-id="74127-203">Update a meeting by using EWS</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|<span data-ttu-id="74127-204">Excluir um compromisso ou reunião</span><span class="sxs-lookup"><span data-stu-id="74127-204">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="74127-205">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="74127-205">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74127-206">Confira também</span><span class="sxs-lookup"><span data-stu-id="74127-206">See also</span></span>

- [<span data-ttu-id="74127-207">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74127-207">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="74127-208">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74127-208">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="74127-209">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74127-209">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="74127-210">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74127-210">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

