---
title: Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Saiba como criar, obter, atualizar e excluir itens usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: a40cd7ae682c1fb0a8d2f9cfcb10d99d4ab08052
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353963"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a>Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange

Saiba como criar, obter, atualizar e excluir itens usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode usar a API gerenciada de EWS ou o EWS para trabalhar com itens em uma caixa de correio. Você pode usar itens genéricos — objetos de API gerenciada de EWS [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) ou tipos EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) — para executar algumas operações (Obtendo um item ou excluir um item usando o identificador do item); No entanto, na maioria das vezes, que você precisará usar um [item de digitado fortemente](folders-and-items-in-ews-in-exchange.md#bk_item) para realizar um get ou operação de atualização, pois você precisará ter acesso às propriedades que são específicas para o item fortemente tipado. 

Por exemplo, você não pode usar um item genérico para recuperar um item que contém um início e data de término - você precisa de um objeto de API gerenciada de EWS [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou um tipo EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) para fazer isso. E se você estiver usando a API gerenciada de EWS, você sempre precisará criar itens fortemente tipadas, porque a classe genérica do **Item** não tem um construtor. Se você estiver trabalhando com um item que não é digitado fortemente, você sempre pode usar a classe do **Item** base para funcionar com o item. 
  
**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para trabalhar com itens**

|**Para...**|**Método API gerenciada de EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Criar um item genérico  <br/> |Nenhum. Você só pode criar tipos de item específico usando a API gerenciada de EWS; não é possível criar itens genéricos.  <br/> |[CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Obtenha um item  <br/> |[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|Atualização de um item  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir um item  <br/> |[Item](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Neste artigo, você saberá quando você pode usar a classe base genérica e quando você precisa usar um item fortemente tipado para concluir a tarefa. Os exemplos de código mostra como usar a classe base e o que fazer quando você não pode usar a classe base ou ele não atender às suas necessidades.
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a>Criar um item usando a API gerenciada de EWS
<a name="bk_createewsma"> </a>

A API gerenciada de EWS não tem um construtor publicamente disponível para a classe de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , portanto, você deve usar o construtor para o tipo de item específico que você deseja criar para criar um item. Por exemplo, use o [Construtor de classe EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) para criar uma nova mensagem de email e o [Construtor de classe de contato](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) para criar um novo contato. Da mesma forma, o servidor retorna nunca genéricos objetos de **Item** nas respostas; todos os itens genéricos são retornados como objetos **EmailMessage** . 
  
Quando você sabe o tipo de item para criar, você pode concluir a tarefa em apenas algumas etapas. As etapas são semelhantes para todos os tipos de item:
  
1. Inicialize uma nova instância de uma das classes de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) com o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) como um parâmetro. 
    
2. Definir as propriedades do item. Os esquemas são diferentes para cada tipo de item, portanto propriedades diferentes estão disponíveis para itens diferentes.
    
3. Salvar o item, ou salvar e enviar o item.
    
Por exemplo, você pode criar um objeto [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , definir o [assunto](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [corpo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)e propriedades [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) e depois enviá-la usando o método [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

Para saber como criar uma reunião ou um item de compromisso usando a API gerenciada de EWS, consulte [criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="create-an-item-by-using-ews"></a>Criar um item usando o EWS
<a name="bk_createews"> </a>

Você pode criar um item genérico ou um item de fortemente tipado usando o EWS. As etapas são semelhantes para todos os tipos de item:
  
1. Use a operação [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para criar um item no armazenamento do Exchange. 
    
2. Use o elemento de [itens](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) para conter um ou mais itens para criar. 
    
3. Definir as propriedades do item.
    
Por exemplo, você pode criar uma mensagem de email e enviá-la usando o código no exemplo a seguir. Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, que indica se o email foi criado com êxito e o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do recentemente mensagem criada. 
  
Para saber como criar um item de compromisso ou uma reunião usando o EWS, consulte [criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a>Obter um item usando a API gerenciada de EWS
<a name="bk_getewsma"> </a>

Para usar a API gerenciada de EWS para obter um item se você souber a [Item.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para recuperar, basta chamar um dos métodos [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) no item e o item será recuperado. Como prática recomendada, recomendamos que você limite as propriedades retornadas somente àqueles que são necessários. Este exemplo retorna a propriedade de **Id** de item e a propriedade **Subject** . 
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. A variável local *itemId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para atualizar. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

Se você estiver procurando por um item que atenda a critérios específicos, faça o seguinte:
  
1. Ligar para a pasta que contém os itens a ser obtido.
    
2. Criar uma instância de um [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) ou um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) para filtrar os itens a ser retornado. 
    
3. Criar uma instância de um objeto [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou de [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) para especificar o número de itens para retornar. 
    
4. Chame o método [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) . 
    
Por exemplo, se você quiser recuperar mensagens de email não lido na caixa de entrada, use o código no exemplo a seguir. Este exemplo usa um **SearchFilterCollection** para limitar os resultados do método **FindItems** a mensagens não lidas e limita a **ItemView** para limitar os resultados para um item. Este código determinado funciona somente em objetos [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) porque o valor de [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) é parte do **SearchFilter**. 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

Como alternativa, você pode usar um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para limitar os resultados da pesquisa, conforme mostrado no exemplo de código a seguir. Este exemplo usa o método [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para recuperar até cinco compromissos que ocorrem nos próximos 30 dias. Este código Obviamente só funciona nos itens de calendário. 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

Observe que as informações do servidor retorna a resposta do método **vincular** é diferente do que as informações que o servidor retorna uma resposta de método **FindItem** ou **FindAppointment** . O método **vincular** pode retornar todas as propriedades esquematizadas, enquanto os métodos **FindItem** e **FindAppointment** não retornará todas as propriedades esquematizadas. Tão se precisar de acesso completo ao item, você terá que usar o método **vincular** . Se você não tiver o item a **Id** do item você gostaria de recuperar, use os métodos **FindItem** ou **FindAppointment** para recuperar o Id e, em seguida, use o método **ligar** para recuperar as propriedades que você precisa. 
  
Para saber como obter uma reunião ou um item de compromisso usando a API gerenciada de EWS, consulte [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="get-an-item-by-using-ews"></a>Obter um item usando o EWS
<a name="bk_getews"> </a>

Se você souber o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do item para recuperar, você pode obter o item usando a operação [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
O exemplo a seguir mostra a solicitação XML para obter o [assunto](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) de um item com um específicos **ItemId**. Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método [ligar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) em um **ItemId**. Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta XML que o servidor retorna após processa a operação **GetItem** . A resposta indica que o item foi recuperado com êxito. Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

Se você não souber o **ItemId** do item que deseja recuperar, você pode usar a operação [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar o item. Para usar a operação **FindItem** , você deve primeiro identificar a pasta que você está procurando. Você pode identificar a pasta usando seu **DistinguinguishedFolderName** ou usando o [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx). Você pode usar o [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) ou [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operações para obter **FolderId** você precisa. Em seguida, use a operação de **FindItem** para pesquisar dessa pasta para obter os resultados que correspondem ao filtro de pesquisa. Diferentemente da API gerenciada de EWS, EWS não fornece uma operação de localização separado para compromissos. A operação **FindItem** recupera itens de todos os tipos. 
  
O exemplo a seguir mostra a solicitação de operação de XML **FindItem** que será enviada para o servidor para encontrar os compromissos na pasta de calendário que ocorrem nos próximos 30 dias. Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade. 
  
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
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **FindItem** com uma mensagem de [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui o valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a operação foi concluída com êxito. Se quaisquer itens de calendário de acordo com os critérios de filtragem, eles são incluídos na resposta.
  
Observe que as informações do servidor retorna a resposta de operação **GetItem** é diferente do que as informações que o servidor retorna em uma **FindItem** ou a resposta de operação **FindAppointment** . A operação **GetItem** pode retornar todas as propriedades esquematizadas, enquanto as operações **FindItem** e **FindAppointment** não retornará todas as propriedades esquematizadas. Isso se você precisar de acesso completo ao item, você terá que usar a operação **GetItem** . Se você não tiver o **ItemId** do item você gostaria de recuperar, use as operações **FindItem** ou **FindAppointment** para recuperar o **ItemId**e, em seguida, use a operação de **GetItem** para recuperar os elementos que você precisa. 
  
Para saber como obter um item de compromisso ou uma reunião usando o EWS, consulte [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a>Atualização de um item usando a API gerenciada de EWS
<a name="bk_updateewsma"> </a>

As etapas para atualizar um item usando a API gerenciada de EWS são semelhantes para todos os tipos de item. No entanto, as propriedades do item são diferentes para cada tipo de item e o método [Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) tem vários métodos sobrecarregados à sua escolha. Para atualizar um item: 
  
1. Use o método [ligar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para obter a versão mais recente do item, a menos que você já tem. Para atualizar propriedades específicas para um item fortemente tipado, você terá que associar a esse tipo de item. Para atualizar as propriedades disponíveis no tipo de item genérico, é possível vincular o objeto de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . 
    
2. Atualize as propriedades no item.
    
3. Chame o método **Update** . 
    
Por exemplo, você pode atualizar o assunto de um email usando o tipo de item genérico, conforme mostrado no código no exemplo a seguir.
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. A variável local *itemId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para atualizar. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

Para saber como atualizar de uma reunião ou um item de compromisso usando a API gerenciada de EWS, consulte [atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-ews"></a>Atualizar um item usando o EWS
<a name="bk_updateews"> </a>

Para atualizar um item usando o EWS, faça o seguinte:
  
1. Use a operação de [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) obter a versão mais recente do item, a menos que você já possui. 
    
2. Use a operação [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) para especificar os campos para atualizar e destinar novos valores aos campos. 
    
O exemplo a seguir mostra a solicitação de operação de XML **UpdateItem** que será enviada para o servidor para atualizar o valor de [assunto](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) da mensagem de email. Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **UpdateItem** com uma mensagem de [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui o valor [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, que indica se a atualização de item foi bem-sucedida.
  
Para saber como atualizar de uma reunião ou um item de compromisso usando o EWS, consulte [atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a>Excluir um item usando a API gerenciada de EWS
<a name="bk_deleteewsma"> </a>

Você pode excluir itens ao movê-las para a pasta Itens excluídos ou para o dumpster. Se você souber o [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para excluir, chame o método [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) no item. 
  
Se você precisar localizar o item antes de excluí-lo, faça o seguinte:
  
1. Chame o método [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para localizar o item a ser excluído. 
    
1. Instanciar um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) e limitar o às propriedades para retornar ou usar um [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) para encontrar itens específicos. 
    
2. Criar uma instância de um [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) ou [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) para especificar o número de itens para retornar. 
    
2. Chame o método [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) . 
    
Por exemplo, o código a seguir mostra como mover uma mensagem de email para a pasta Itens excluídos.
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. A variável local *itemId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para atualizar. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

Para obter mais detalhes sobre a exclusão de itens, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md). Para saber como excluir um item de compromisso ou uma reunião usando a API gerenciada de EWS, consulte [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-ews"></a>Excluir um item usando o EWS
<a name="bk_deleteews"> </a>

Você pode excluir um item usando a operação [DeleteItem](../web-service-reference/deleteitem-operation.md) . 
  
O exemplo a seguir mostra a solicitação XML que será enviada para o servidor para mover a mensagem de email para a pasta Itens excluídos. Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **DeleteItem** com uma mensagem de [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui o valor [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, que indica que a exclusão de item foi bem-sucedida.
  
Para obter mais detalhes sobre a exclusão de itens, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md). Para saber como excluir um item de compromisso ou uma reunião usando o EWS, consulte [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="move-or-copy-items-to-another-mailbox"></a>Mover ou copiar itens para outra caixa de correio
<a name="bk_movecopybtnmailboxes"> </a>

Você pode mover ou copiar itens entre caixas de correio usando as operações [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) e [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) . Para saber mais, consulte [Exportar e importar itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também

- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    

