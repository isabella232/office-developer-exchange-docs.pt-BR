---
title: Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Saiba como criar, obter, atualizar e excluir itens usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: e86affbe8efe0dfc312f5ed5fadec2547f1352ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527583"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a>Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange

Saiba como criar, obter, atualizar e excluir itens usando a API gerenciada do EWS ou o EWS no Exchange.
  
Você pode usar a API gerenciada do EWS ou o EWS para trabalhar com itens em uma caixa de correio. Você pode usar itens genéricos – objetos de [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) da API gerenciada por EWS ou tipos de [Item](https://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) do EWS para executar algumas operações (obter um item ou excluir um item usando o identificador do item); no entanto, a maior parte do tempo você terá que usar um [Item fortemente tipado](folders-and-items-in-ews-in-exchange.md#bk_item) para executar uma operação get ou Update, pois você precisará ter acesso às propriedades que são específicas para o item fortemente tipado. 

Por exemplo, você não pode usar um item genérico para recuperar um item que contenha uma data de início e de término-você precisa de um objeto de [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) da API gerenciada do EWS ou um tipo de [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) do EWS para fazer isso. E se você estiver usando a API gerenciada do EWS, você sempre precisará criar itens fortemente tipados, pois a classe de **Item** genérico não tem um construtor. Se você estiver trabalhando com um item que não tenha rigidez de tipos, você sempre poderá usar a classe de **Item** base para trabalhar com o item. 
  
**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com itens**

|**Para...**|**Método de API gerenciada do EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Criar um item genérico  <br/> |Nenhum Você só pode criar tipos de item específicos usando a API gerenciada do EWS; Você não pode criar itens genéricos.  <br/> |[CreateItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Obter um item  <br/> |[Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|Atualizar um item  <br/> |[Item. Update](https://msdn.microsoft.com/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir um item  <br/> |[Item. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Neste artigo, você aprenderá quando você pode usar a classe base genérica e quando precisa usar um item com rigidez de tipos para concluir a tarefa. Os exemplos de código mostrarão como usar a classe base e o que fazer quando você não pode usar a classe base ou não atende às suas necessidades.
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a>Criar um item usando a API gerenciada do EWS
<a name="bk_createewsma"> </a>

A API gerenciada do EWS não tem um construtor disponível publicamente para a classe [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , portanto, você deve usar o construtor para o tipo de item específico que você deseja criar para criar um item. Por exemplo, use o [Construtor de classe EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) para criar uma nova mensagem de email e o [Construtor de classe de contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) para criar um novo contato. Da mesma forma, o servidor nunca retorna objetos de **Item** genérico em respostas; todos os itens genéricos são retornados como objetos **EmailMessage** . 
  
Quando você sabe o tipo de item a ser criado, você pode concluir a tarefa em apenas algumas etapas. As etapas são semelhantes para todos os tipos de item:
  
1. Inicializar uma nova instância de uma das classes de [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) com o objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) como um parâmetro. 
    
2. Definir propriedades no item. Os esquemas são diferentes para cada tipo de item e, portanto, propriedades diferentes estão disponíveis para diferentes itens.
    
3. Salve o item ou salve e envie o item.
    
Por exemplo, você pode criar um objeto [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , definir as [Propriedades Subject](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)e [ToRecipients](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) e enviá-lo usando o método [EmailMessage. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
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

Para saber como criar um item de reunião ou compromisso usando a API gerenciada do EWS, confira [criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="create-an-item-by-using-ews"></a>Criar um item usando o EWS
<a name="bk_createews"> </a>

Você pode criar um item genérico ou um item fortemente tipado usando o EWS. As etapas são semelhantes para todos os tipos de item:
  
1. Use a operação [CreateItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para criar um item no repositório do Exchange. 
    
2. Use o elemento [Items](https://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) para conter um ou mais itens a serem criados. 
    
3. Definir propriedades no item.
    
Por exemplo, você pode criar uma mensagem de email e enviá-la usando o código no exemplo a seguir. Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método [SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
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

O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que o email foi criado com êxito e o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem recém-criada. 
  
Para saber como criar um item de reunião ou compromisso usando o EWS, confira [criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a>Obter um item usando a API gerenciada do EWS
<a name="bk_getewsma"> </a>

Para usar a API gerenciada do EWS para obter um item se você souber o [Item.ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item a ser recuperado, basta chamar um dos métodos [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) no item e o item será recuperado. Como prática recomendada, recomendamos que você limite as propriedades retornadas somente para as que forem necessárias. Este exemplo retorna a propriedade item **ID** e a propriedade **Subject** . 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. A variável local *ItemId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item a ser atualizado. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

Se você estiver procurando um item que atenda a critérios específicos, faça o seguinte:
  
1. Vincule à pasta que contém os itens a serem obtidos.
    
2. Crie uma instância de [SearchFilter. SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) ou um [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) para filtrar os itens a serem retornados. 
    
3. Crie uma instância de um objeto item [View](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) ou [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) para especificar o número de itens a serem retornados. 
    
4. Chame o método [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [ExchangeService. FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) . 
    
Por exemplo, se você quiser recuperar mensagens de email não lidas na caixa de entrada, use o código no exemplo a seguir. Este exemplo usa um **SearchFilterCollection** para limitar os resultados do método **FindItems** a mensagens não lidas e limita o **modo de exibição** para limitar os resultados a um item. Este código específico só funciona nos objetos [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) porque o valor de [EmailMessageSchema. IsRead](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) é parte do **SearchFilter**. 
  
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

Como alternativa, você pode usar um [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para limitar os resultados da pesquisa, conforme mostrado no exemplo de código a seguir. Este exemplo usa o método [FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para recuperar até cinco compromissos que ocorrem nos próximos 30 dias. Este código de curso só funciona em itens de calendário. 
  
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

Observe que as informações que o servidor retorna na resposta do método **BIND** são diferentes das informações que o servidor retorna para uma resposta de método **FindItem** ou **FindAppointment** . O método **BIND** pode retornar todas as propriedades esquematizado, enquanto os métodos **FindItem** e **FindAppointment** não retornam todas as propriedades esquematizado. Portanto, se você precisar de acesso completo ao item, será necessário usar o método **BIND** . Se você não tiver a **ID** do item que deseja recuperar, use os métodos **FindItem** ou **FindAppointment** para recuperar a ID e, em seguida, use o método **BIND** para recuperar as propriedades que você precisa. 
  
Para saber como obter um item de reunião ou compromisso usando a API gerenciada do EWS, confira [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="get-an-item-by-using-ews"></a>Obter um item usando o EWS
<a name="bk_getews"> </a>

Se você souber o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do item a ser recuperado, poderá obter o item usando a operação [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
O exemplo a seguir mostra a solicitação XML para obter o [assunto](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) de um item com um **ItemId**específico. Essa é também a solicitação XML que a API gerenciada do EWS envia ao chamar o método [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) em um **ItemId**. Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O exemplo a seguir mostra a resposta XML que o servidor retorna depois de processar a operação **GetItem** . A resposta indica que o item foi recuperado com êxito. Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Se você não souber o **ItemId** do item que deseja recuperar, poderá usar a operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar o item. Para usar a operação **FindItem** , você deve primeiro identificar a pasta que está pesquisando. Você pode identificar a pasta usando seu **DistinguinguishedFolderName** ou usando o [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx). Você pode usar as operações [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) ou [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) para obter o **FolderId** necessário. Em seguida, use a operação **FindItem** para pesquisar na pasta resultados que correspondam ao filtro de pesquisa. Diferentemente da API gerenciada por EWS, o EWS não fornece uma operação de localização separada para compromissos. A operação **FindItem** recupera itens de todos os tipos. 
  
O exemplo a seguir mostra a solicitação de operação **FINDITEM** XML que é enviada ao servidor para localizar compromissos na pasta calendário que ocorrem nos próximos 30 dias. Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
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

O servidor responde à solicitação **FindItem** com uma mensagem [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a operação foi concluída com êxito. Se algum item de calendário atender aos critérios de filtragem, ele será incluído na resposta.
  
Observe que as informações que o servidor retorna na resposta da operação **GetItem** são diferentes das informações que o servidor retorna em uma resposta de operação **FindItem** ou **FindAppointment** . A operação **GetItem** pode retornar todas as propriedades esquematizado, enquanto as operações **FindItem** e **FindAppointment** não retornam todas as propriedades de esquematizado. Portanto, se você precisar de acesso completo ao item, será necessário usar a operação **GetItem** . Se você não tiver o **ItemId** do item que deseja recuperar, use as operações **FindItem** ou **FindAppointment** para recuperar o **ItemId**e, em seguida, use a operação **GetItem** para recuperar os elementos necessários. 
  
Para saber como obter um item de reunião ou compromisso usando o EWS, confira [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a>Atualizar um item usando a API gerenciada do EWS
<a name="bk_updateewsma"> </a>

As etapas para atualizar um item usando a API gerenciada do EWS são semelhantes para todos os tipos de item; no entanto, as propriedades do item são diferentes para cada tipo de item, e o método [Update](https://msdn.microsoft.com/library/office/dd635915%28v=exchg.80%29.aspx) tem vários métodos sobrecarregados para escolher. Para atualizar um item: 
  
1. Use o método [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para obter a versão mais recente do item, a menos que você já tenha isso. Para atualizar as propriedades específicas de um item com rigidez de tipos, você terá que associar a esse tipo de item. Para atualizar as propriedades disponíveis no tipo de item genérico, você pode associar ao objeto [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . 
    
2. Atualize as propriedades do item.
    
3. Chame o método **Update** . 
    
Por exemplo, você pode atualizar o assunto de um email usando o tipo de item genérico, conforme mostrado no código no exemplo a seguir.
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. A variável local *ItemId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item a ser atualizado. 
  
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

Para saber como atualizar um item de reunião ou compromisso usando a API gerenciada do EWS, confira [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-ews"></a>Atualizar um item usando o EWS
<a name="bk_updateews"> </a>

Para atualizar um item usando o EWS, faça o seguinte:
  
1. Use a operação [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) para obter a versão mais recente do item, a menos que você já tenha isso. 
    
2. Use a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) para especificar os campos a serem atualizados e atribuir novos valores a esses campos. 
    
O exemplo a seguir mostra a solicitação de operação de **UPDATEITEM** XML que é enviada ao servidor para atualizar o valor de [assunto](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) da mensagem de email. Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **UpdateItem** com uma mensagem [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que a atualização do item foi bem-sucedida.
  
Para saber como atualizar um item de reunião ou compromisso usando o EWS, confira [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a>Excluir um item usando a API gerenciada do EWS
<a name="bk_deleteewsma"> </a>

Você pode excluir itens movendo-os para a pasta itens excluídos ou para o dumpster. Se você souber o [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item a ser excluído, basta chamar o método [delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) no item. 
  
Se você precisar localizar o item antes de excluí-lo, faça o seguinte:
  
1. Chame o método [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para localizar o item a ser excluído. 
    
1. Instanciar um [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) e limitá-lo às propriedades a serem retornadas ou usar um [SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) para localizar itens específicos. 
    
2. Instancie um item [View](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) ou [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) para especificar o número de itens a serem retornados. 
    
2. Chame o método [delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) . 
    
Por exemplo, o código a seguir mostra como mover uma mensagem de email para a pasta itens excluídos.
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. A variável local *ItemId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item a ser atualizado. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

Para obter mais detalhes sobre como excluir itens, consulte [excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md). Para saber como excluir um item de reunião ou compromisso usando a API gerenciada do EWS, consulte [excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-ews"></a>Excluir um item usando o EWS
<a name="bk_deleteews"> </a>

Você pode excluir um item usando a operação [DeleteItem](../web-service-reference/deleteitem-operation.md) . 
  
O exemplo a seguir mostra a solicitação XML que é enviada ao servidor para mover a mensagem de email para a pasta itens excluídos. Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **DeleteItem** com uma mensagem [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que a exclusão do item foi bem-sucedida.
  
Para obter mais detalhes sobre como excluir itens, consulte [excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md). Para saber como excluir um item de reunião ou compromisso usando o EWS, confira [excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="move-or-copy-items-to-another-mailbox"></a>Mover ou copiar itens para outra caixa de correio
<a name="bk_movecopybtnmailboxes"> </a>

Você pode mover ou copiar itens entre caixas de correio usando as operações [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) e [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) . Para saber mais, confira [exportando e importando itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também

- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    

