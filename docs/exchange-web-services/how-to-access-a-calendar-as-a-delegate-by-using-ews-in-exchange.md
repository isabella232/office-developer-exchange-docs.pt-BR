---
title: Acessar um calendário como um representante, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Saiba como acessar um calendário como um representante, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 609e5f0bb22c78174289a2eb10210999c8391a3d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353837"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="7ad34-103">Acessar um calendário como um representante, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ad34-103">Access a calendar as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="7ad34-104">Saiba como acessar um calendário como um representante, usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ad34-104">Learn how to access a calendar as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7ad34-105">Você pode usar a API gerenciada de EWS ou EWS para conceder a um usuário Delegar acesso à pasta de calendário de um proprietário caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Calendar folder.</span></span> <span data-ttu-id="7ad34-106">O representante pode então criar solicitações de reunião em nome do proprietário da caixa de correio, criar compromissos, responder às solicitações de reunião, recuperar, atualizar e excluir reuniões da pasta de calendário do proprietário da caixa de correio, dependendo de suas permissões.</span><span class="sxs-lookup"><span data-stu-id="7ad34-106">The delegate can then create meeting requests on behalf of the mailbox owner, create appointments, respond to meeting requests, and retrieve, update, and delete meetings from the mailbox owner's Calendar folder, depending on their permissions.</span></span>
  
<span data-ttu-id="7ad34-107">Como um representante, use os métodos e as mesmas operações para acessar a pasta de calendário de um proprietário caixa de correio que você usa para acessar sua própria pasta Calendário.</span><span class="sxs-lookup"><span data-stu-id="7ad34-107">As a delegate, you use the same methods and operations to access a mailbox owner's Calendar folder that you use to access your own Calendar folder.</span></span> <span data-ttu-id="7ad34-108">A principal diferença é que você precisa usar [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de calendário ou a subpasta de calendário e, em seguida, depois de identificar a ID de item ou o ID da pasta, você pode usar [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item.</span><span class="sxs-lookup"><span data-stu-id="7ad34-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a calendar item or calendar subfolder, and then after you identify the item ID or folder ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="7ad34-109">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para acessar um calendário como um representante**</span><span class="sxs-lookup"><span data-stu-id="7ad34-109">**Table 1. EWS Managed API methods and EWS operations for accessing a calendar as a delegate**</span></span>

|<span data-ttu-id="7ad34-110">**Se você quiser …**</span><span class="sxs-lookup"><span data-stu-id="7ad34-110">**If you want to…**</span></span>|<span data-ttu-id="7ad34-111">**Use este método de API gerenciada de EWS …**</span><span class="sxs-lookup"><span data-stu-id="7ad34-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="7ad34-112">**Use essa operação EWS …**</span><span class="sxs-lookup"><span data-stu-id="7ad34-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ad34-113">Criar uma reunião ou compromisso como um representante</span><span class="sxs-lookup"><span data-stu-id="7ad34-113">Create a meeting or appointment as a delegate</span></span>  <br/> |<span data-ttu-id="7ad34-114">[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de calendário do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ad34-114">[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="7ad34-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ad34-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="7ad34-116">Criar vários reuniões ou compromissos como um representante</span><span class="sxs-lookup"><span data-stu-id="7ad34-116">Create multiple meetings or appointments as a delegate</span></span>  <br/> |<span data-ttu-id="7ad34-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de calendário do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ad34-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="7ad34-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ad34-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="7ad34-119">Pesquise ou encontrar um compromisso ou reunião como um representante</span><span class="sxs-lookup"><span data-stu-id="7ad34-119">Search for or find an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="7ad34-120">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de calendário do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ad34-120">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="7ad34-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7ad34-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="7ad34-122">Obtenha um compromisso ou reunião como um representante</span><span class="sxs-lookup"><span data-stu-id="7ad34-122">Get an appointment or meeting as a delegate</span></span>  <br/> |[<span data-ttu-id="7ad34-123">Appointment.Bind</span><span class="sxs-lookup"><span data-stu-id="7ad34-123">Appointment.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7ad34-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="7ad34-124">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="7ad34-125">Atualizar um compromisso ou reunião como um representante</span><span class="sxs-lookup"><span data-stu-id="7ad34-125">Update an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="7ad34-126">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7ad34-126">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="7ad34-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7ad34-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="7ad34-128">Excluir um compromisso ou reunião como um representante</span><span class="sxs-lookup"><span data-stu-id="7ad34-128">Delete an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="7ad34-129">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7ad34-129">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="7ad34-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="7ad34-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="7ad34-131">Os exemplos de código neste artigo, primary@contoso.com é o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-131">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="7ad34-132">Tarefas de pré-requisito</span><span class="sxs-lookup"><span data-stu-id="7ad34-132">Prerequisite tasks</span></span>
<span data-ttu-id="7ad34-133"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-133"></span></span>

<span data-ttu-id="7ad34-134">Antes de um usuário pode acessar a pasta de calendário de um proprietário caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para pasta de calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-134">Before a user can access a mailbox owner's Calendar folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="7ad34-135">Um representante deve ter uma caixa de correio associada à sua conta para atualizar o calendário de um proprietário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-135">A delegate must have a mailbox attached to their account to update the calendar of a mailbox owner.</span></span>
  
<span data-ttu-id="7ad34-136">Se precisar de um representante trabalhar com as solicitações de reunião e respostas apenas, você pode adicionar o representante para a pasta de calendário e usar o valor de enumeração padrão [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API ou o [ DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) valor do elemento EWS do **DelegatesAndSendInformationToMe** para enviar solicitações para o delegado e mensagens informativas para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-136">If a delegate needs to work with meeting requests and responses only, you can add the delegate to the Calendar folder, and use the default [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API enumeration value or the [DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS element value of **DelegatesAndSendInformationToMe** to send the requests to the delegate and informational messages to the mailbox owner.</span></span> <span data-ttu-id="7ad34-137">O representante, em seguida, não precisará ter permissão de acesso à pasta de caixa de entrada do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-137">The delegate then does not need to be given access to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="7ad34-138">Criar uma reunião ou compromisso como um representante usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-138">Create a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="7ad34-139"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-139"></span></span>

<span data-ttu-id="7ad34-140">A API gerenciada de EWS permite que você use o objeto de serviço para o usuário delegado para criar itens de calendário para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-140">The EWS Managed API enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="7ad34-141">Este exemplo mostra como usar o método [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes.</span><span class="sxs-lookup"><span data-stu-id="7ad34-141">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="7ad34-142">Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e o delegado recebeu as permissões apropriadas para a pasta de calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Calendar folder.</span></span> 
  
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

<span data-ttu-id="7ad34-143">Observe que, quando você salva o item, a chamada do método [Salvar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) deve identificar pasta de calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="7ad34-144">Se a pasta de calendário do proprietário da caixa de correio não for especificada, a solicitação de reunião obtém salvos não pasta de calendário do proprietário da caixa de correio e de calendário do representante.</span><span class="sxs-lookup"><span data-stu-id="7ad34-144">If the mailbox owner's Calendar folder is not specified, the meeting request gets saved to the delegate's calendar and not the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="7ad34-145">Você pode incluir uma pasta de calendário do proprietário da caixa de correio na chamada do método **Salvar** de duas maneiras.</span><span class="sxs-lookup"><span data-stu-id="7ad34-145">You can include the mailbox owner's Calendar folder in the **Save** method call in two ways.</span></span> <span data-ttu-id="7ad34-146">Recomendamos que você criar uma nova instância do objeto [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) usando o [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

<span data-ttu-id="7ad34-147">No entanto, você também pode [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para a pasta de calendário em primeiro lugar e, em seguida, usar a identificação da pasta na chamada do método **Salvar** .</span><span class="sxs-lookup"><span data-stu-id="7ad34-147">However, you can also [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Calendar folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="7ad34-148">Lembre-se, no entanto, se esse cria uma chamada de EWS extra.</span><span class="sxs-lookup"><span data-stu-id="7ad34-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
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

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="7ad34-149">Criar uma reunião ou compromisso como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-149">Create a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="7ad34-150"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-150"></span></span>

<span data-ttu-id="7ad34-151">EWS permite que você use o objeto de serviço para o usuário delegado para criar itens de calendário para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-151">EWS enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="7ad34-152">Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes.</span><span class="sxs-lookup"><span data-stu-id="7ad34-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="7ad34-153">Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **Save** para [criar uma reunião ou compromisso como um representante](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="7ad34-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a meeting or appointment as a delegate](#bk_createewsma).</span></span>
  
<span data-ttu-id="7ad34-154">O cabeçalho SOAP foi removido do exemplo a seguir para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="7ad34-154">The SOAP header has been removed from the following example for brevity.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="7ad34-155">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se a reunião foi criada com êxito.</span><span class="sxs-lookup"><span data-stu-id="7ad34-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the meeting was created successfully.</span></span> <span data-ttu-id="7ad34-156">A resposta também contém a ID do item de reunião recém-criado.</span><span class="sxs-lookup"><span data-stu-id="7ad34-156">The response also contains the item ID of the newly created meeting.</span></span>
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="7ad34-157">Procurar uma reunião ou compromisso como um representante usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-157">Search for a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="7ad34-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-158"></span></span>

<span data-ttu-id="7ad34-159">Para pesquisar uma reunião, você deve usar um dos métodos [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você pode especificar uma pasta de calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-159">To search for a meeting, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Calendar folder.</span></span> 
  
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

<span data-ttu-id="7ad34-160">Depois que a chamada **FindItems** retornará uma resposta com uma ID, você pode obter, atualizar ou excluir essa reunião usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) — e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that meeting by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="7ad34-161">Procurar por uma reunião ou compromisso como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-161">Search for a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="7ad34-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-162"></span></span>

<span data-ttu-id="7ad34-163">EWS permite que você use o objeto de serviço para o usuário delegado para pesquisar compromissos e reuniões que atendam a um conjunto de critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7ad34-163">EWS enables you to use the service object for the delegate user to search for appointments and meetings that meet a set of search criteria.</span></span> <span data-ttu-id="7ad34-164">Este exemplo mostra como usar a operação [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar reuniões na pasta de calendário do proprietário da caixa de correio que contêm a palavra "building" no assunto.</span><span class="sxs-lookup"><span data-stu-id="7ad34-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Calendar folder that contain the word "building" in the subject.</span></span> 
  
<span data-ttu-id="7ad34-165">Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **FindItem** pesquisar [por uma reunião ou compromisso como um representante](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="7ad34-165">This is also the XML request that the EWS Managed API sends when you use the **FindItem** method to [search for a meeting or appointment as a delegate](#bk_searchewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="7ad34-166">O servidor responde à solicitação **FindItem** com uma mensagem de [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pesquisa foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="7ad34-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="7ad34-167">A resposta conterá uma [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) de compromissos ou reuniões que atendidos os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7ad34-167">The response contains a [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) for any appointments or meetings that met the search criteria.</span></span> <span data-ttu-id="7ad34-168">Nesse caso, apenas uma reunião é encontrada.</span><span class="sxs-lookup"><span data-stu-id="7ad34-168">In this case, only one meeting is found.</span></span> 
  
<span data-ttu-id="7ad34-169">O valor do elemento [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ad34-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="7ad34-170">Agora que você tem o **ItemId** referentes à reunião que atenda aos seus critérios, você pode obter, atualizar ou excluir essa reunião by using the **ItemId** e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) — e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-170">Now that you have the **ItemId** for the meeting that meets your criteria, you can get, update, or delete that meeting by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="7ad34-171">Obter, atualizar ou excluir itens de calendário como um representante, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-171">Get, update, or delete calendar items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="7ad34-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-172"></span></span>

<span data-ttu-id="7ad34-173">Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir uma reunião ou compromisso da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="7ad34-173">You can use the EWS Managed API to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="7ad34-174">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="7ad34-174">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="7ad34-175">A ID do item incluída na chamada do método **vincular** exclusivamente identifica o item no armazenamento da caixa de correio, na pasta de calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="7ad34-176">**Tabela 2. Métodos de API gerenciada de EWS para trabalhar com os compromissos e reuniões como um representante**</span><span class="sxs-lookup"><span data-stu-id="7ad34-176">**Table 2. EWS Managed API methods for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="7ad34-177">**Task**</span><span class="sxs-lookup"><span data-stu-id="7ad34-177">**Task**</span></span>|<span data-ttu-id="7ad34-178">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="7ad34-178">**EWS Managed API method**</span></span>|<span data-ttu-id="7ad34-179">**Código de exemplo**</span><span class="sxs-lookup"><span data-stu-id="7ad34-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ad34-180">Obtenha um compromisso ou reunião</span><span class="sxs-lookup"><span data-stu-id="7ad34-180">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="7ad34-181">Vincular</span><span class="sxs-lookup"><span data-stu-id="7ad34-181">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7ad34-182">Obter um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="7ad34-183">Atualização de uma reunião ou compromisso</span><span class="sxs-lookup"><span data-stu-id="7ad34-183">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="7ad34-184">[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido de [atualização](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7ad34-184">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="7ad34-185">Atualização de uma reunião usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-185">Update a meeting by using the EWS Managed API</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|<span data-ttu-id="7ad34-186">Excluir um compromisso ou reunião</span><span class="sxs-lookup"><span data-stu-id="7ad34-186">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="7ad34-187">[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Excluir](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7ad34-187">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="7ad34-188">Excluir uma reunião usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-188">Delete a meeting by using the EWS Managed API</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="7ad34-189">Obter, atualizar ou excluir itens de calendário como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-189">Get, update, or delete calendar items as a delegate by using EWS</span></span>
<span data-ttu-id="7ad34-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="7ad34-190"></span></span>

<span data-ttu-id="7ad34-191">Você pode usar o EWS para obter, atualizar ou excluir uma reunião ou compromisso da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="7ad34-191">You can use EWS to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="7ad34-192">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="7ad34-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="7ad34-193">A ID do item incluída na chamada do método [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) exclusivamente identifica o item no armazenamento da caixa de correio, na pasta de calendário do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7ad34-193">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="7ad34-194">**Tabela 3. Operações do EWS para trabalhar com os compromissos e reuniões como um representante**</span><span class="sxs-lookup"><span data-stu-id="7ad34-194">**Table 3. EWS operations for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="7ad34-195">**Task**</span><span class="sxs-lookup"><span data-stu-id="7ad34-195">**Task**</span></span>|<span data-ttu-id="7ad34-196">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="7ad34-196">**EWS operation**</span></span>|<span data-ttu-id="7ad34-197">**Código de exemplo**</span><span class="sxs-lookup"><span data-stu-id="7ad34-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ad34-198">Obtenha um compromisso ou reunião</span><span class="sxs-lookup"><span data-stu-id="7ad34-198">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="7ad34-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="7ad34-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="7ad34-200">Obter um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="7ad34-201">Atualização de uma reunião ou compromisso</span><span class="sxs-lookup"><span data-stu-id="7ad34-201">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="7ad34-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7ad34-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="7ad34-203">Atualizar uma reunião usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7ad34-203">Update a meeting by using EWS</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|<span data-ttu-id="7ad34-204">Excluir um compromisso ou reunião</span><span class="sxs-lookup"><span data-stu-id="7ad34-204">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="7ad34-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="7ad34-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ad34-206">Confira também</span><span class="sxs-lookup"><span data-stu-id="7ad34-206">See also</span></span>

- [<span data-ttu-id="7ad34-207">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ad34-207">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="7ad34-208">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ad34-208">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="7ad34-209">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ad34-209">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="7ad34-210">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7ad34-210">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

