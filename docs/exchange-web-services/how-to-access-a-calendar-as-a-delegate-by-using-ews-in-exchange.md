---
title: Acessar um calendário como um representante, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Saiba como acessar um calendário como um representante, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 24327c28f58e728807fc5581b480d3c01d3b7208
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750684"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a>Acessar um calendário como um representante, usando o EWS no Exchange

Saiba como acessar um calendário como um representante, usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode usar a API gerenciada de EWS ou EWS para conceder a um usuário Delegar acesso à pasta de calendário de um proprietário caixa de correio. O representante pode então criar solicitações de reunião em nome do proprietário da caixa de correio, criar compromissos, responder às solicitações de reunião, recuperar, atualizar e excluir reuniões da pasta de calendário do proprietário da caixa de correio, dependendo de suas permissões.
  
Como um representante, use os métodos e as mesmas operações para acessar a pasta de calendário de um proprietário caixa de correio que você usa para acessar sua própria pasta Calendário. A principal diferença é que você precisa usar [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de calendário ou a subpasta de calendário e, em seguida, depois de identificar a ID de item ou o ID da pasta, você pode usar [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item. 
  
**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para acessar um calendário como um representante**

|**Se você quiser …**|**Use este método de API gerenciada de EWS …**|**Use essa operação EWS …**|
|:-----|:-----|:-----|
|Criar uma reunião ou compromisso como um representante  <br/> |[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de calendário do proprietário da caixa de correio  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Criar vários reuniões ou compromissos como um representante  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de calendário do proprietário da caixa de correio  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Pesquise ou encontrar um compromisso ou reunião como um representante  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de calendário do proprietário da caixa de correio  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Obtenha um compromisso ou reunião como um representante  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Atualizar um compromisso ou reunião como um representante  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir um compromisso ou reunião como um representante  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
> [!NOTE]
> Os exemplos de código neste artigo, primary@contoso.com é o proprietário da caixa de correio. 
  
## <a name="prerequisite-tasks"></a>Tarefas de pré-requisito
<a name="bk_prereq"> </a>

Antes de um usuário pode acessar a pasta de calendário de um proprietário caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para pasta de calendário do proprietário da caixa de correio. 
  
Um representante deve ter uma caixa de correio associada à sua conta para atualizar o calendário de um proprietário de caixa de correio.
  
Se precisar de um representante trabalhar com as solicitações de reunião e respostas apenas, você pode adicionar o representante para a pasta de calendário e usar o valor de enumeração padrão [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API ou o [ DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) valor do elemento EWS do **DelegatesAndSendInformationToMe** para enviar solicitações para o delegado e mensagens informativas para o proprietário da caixa de correio. O representante, em seguida, não precisará ter permissão de acesso à pasta de caixa de entrada do proprietário da caixa de correio. 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Criar uma reunião ou compromisso como um representante usando a API gerenciada de EWS
<a name="bk_createewsma"> </a>

A API gerenciada de EWS permite que você use o objeto de serviço para o usuário delegado para criar itens de calendário para o proprietário da caixa de correio. Este exemplo mostra como usar o método [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes. 
  
Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e o delegado recebeu as permissões apropriadas para a pasta de calendário do proprietário da caixa de correio. 
  
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

Observe que, quando você salva o item, a chamada do método [Salvar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) deve identificar pasta de calendário do proprietário da caixa de correio. Se a pasta de calendário do proprietário da caixa de correio não for especificada, a solicitação de reunião obtém salvos não pasta de calendário do proprietário da caixa de correio e de calendário do representante. Você pode incluir uma pasta de calendário do proprietário da caixa de correio na chamada do método **Salvar** de duas maneiras. Recomendamos que você criar uma nova instância do objeto [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) usando o [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o endereço SMTP do proprietário da caixa de correio. 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

No entanto, você também pode [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para a pasta de calendário em primeiro lugar e, em seguida, usar a identificação da pasta na chamada do método **Salvar** . Lembre-se, no entanto, se esse cria uma chamada de EWS extra. 
  
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

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Criar uma reunião ou compromisso como um representante usando o EWS
<a name="bk_createews"> </a>

EWS permite que você use o objeto de serviço para o usuário delegado para criar itens de calendário para o proprietário da caixa de correio. Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes. 
  
Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **Save** para [criar uma reunião ou compromisso como um representante](#bk_createewsma).
  
O cabeçalho SOAP foi removido do exemplo a seguir para fins de concisão.
  
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

O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se a reunião foi criada com êxito. A resposta também contém a ID do item de reunião recém-criado.
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Procurar uma reunião ou compromisso como um representante usando a API gerenciada de EWS
<a name="bk_searchewsma"> </a>

Para pesquisar uma reunião, você deve usar um dos métodos [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você pode especificar uma pasta de calendário do proprietário da caixa de correio. 
  
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

Depois que a chamada **FindItems** retornará uma resposta com uma ID, você pode obter, atualizar ou excluir essa reunião usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) — e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio. 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Procurar por uma reunião ou compromisso como um representante usando o EWS
<a name="bk_searchews"> </a>

EWS permite que você use o objeto de serviço para o usuário delegado para pesquisar compromissos e reuniões que atendam a um conjunto de critérios de pesquisa. Este exemplo mostra como usar a operação [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar reuniões na pasta de calendário do proprietário da caixa de correio que contêm a palavra "building" no assunto. 
  
Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **FindItem** pesquisar [por uma reunião ou compromisso como um representante](#bk_searchewsma).
  
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

O servidor responde à solicitação **FindItem** com uma mensagem de [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pesquisa foi concluída com êxito. A resposta conterá uma [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) de compromissos ou reuniões que atendidos os critérios de pesquisa. Nesse caso, apenas uma reunião é encontrada. 
  
O valor do elemento [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para melhorar a legibilidade. 
  
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

Agora que você tem o **ItemId** referentes à reunião que atenda aos seus critérios, você pode obter, atualizar ou excluir essa reunião by using the **ItemId** e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) — e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio. 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obter, atualizar ou excluir itens de calendário como um representante, usando a API gerenciada de EWS
<a name="bk_geteswma"> </a>

Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir uma reunião ou compromisso da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante. A única diferença é que o objeto de serviço é para o usuário delegado. A ID do item incluída na chamada do método **vincular** exclusivamente identifica o item no armazenamento da caixa de correio, na pasta de calendário do proprietário da caixa de correio. 
  
**Tabela 2. Métodos de API gerenciada de EWS para trabalhar com os compromissos e reuniões como um representante**

|**Task**|**Método API gerenciada de EWS**|**Exemplo de código**|
|:-----|:-----|:-----|
|Obtenha um compromisso ou reunião  <br/> |[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Obter um item usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Atualização de uma reunião ou compromisso  <br/> |[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido de [atualização](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Atualização de uma reunião usando a API gerenciada de EWS](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|Excluir um compromisso ou reunião  <br/> |[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Excluir](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Excluir uma reunião usando a API gerenciada de EWS](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a>Obter, atualizar ou excluir itens de calendário como um representante usando o EWS
<a name="bk_getews"> </a>

Você pode usar o EWS para obter, atualizar ou excluir uma reunião ou compromisso da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante. A única diferença é que o objeto de serviço é para o usuário delegado. A ID do item incluída na chamada do método [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) exclusivamente identifica o item no armazenamento da caixa de correio, na pasta de calendário do proprietário da caixa de correio. 
  
**Tabela 3. Operações do EWS para trabalhar com os compromissos e reuniões como um representante**

|**Task**|**Operação do EWS**|**Exemplo de código**|
|:-----|:-----|:-----|
|Obtenha um compromisso ou reunião  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obter um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Atualização de uma reunião ou compromisso  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Atualizar uma reunião usando o EWS](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|Excluir um compromisso ou reunião  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a>Confira também

- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)   
- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    

