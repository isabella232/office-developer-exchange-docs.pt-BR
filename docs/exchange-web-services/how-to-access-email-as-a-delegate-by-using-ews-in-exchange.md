---
title: Acessar email como um representante usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Saiba como acessar o email como um representante usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 0c26f69042c568fe7d877778c7d8f1e689e5b372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528283"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a>Acessar email como um representante usando o EWS no Exchange

Saiba como acessar o email como um representante usando a API gerenciada do EWS ou o EWS no Exchange.
  
Você pode usar a API gerenciada do EWS ou o EWS para conceder acesso de representante de usuário à pasta caixa de entrada do proprietário da caixa de correio. O representante pode então criar solicitações de reunião em nome do proprietário da caixa de correio, Pesquisar emails e recuperar, atualizar e excluir emails da pasta caixa de entrada do proprietário da caixa de correio, dependendo de suas permissões.
  
Como representante, você usa os mesmos métodos e operações para acessar a pasta caixa de entrada do proprietário da caixa de correio que você usa para acessar uma pasta caixa de entrada sem acesso de representante. A principal diferença é que você precisa usar o [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de email e depois depois de identificar a ID do item, você pode usar o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item. 
  
**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para acessar o email como um representante**

|**Se você quiser...**|**Use este método de API gerenciada do EWS...**|**Use esta operação do EWS...**|
|:-----|:-----|:-----|
|Criar e enviar um email como um representante  <br/> |[EmailMessage. Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta Rascunhos do proprietário da caixa de correio  <br/> [EmailMessage. SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta Itens enviados do proprietário da caixa de correio  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> [SendItem](https://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Criar várias mensagens de email como um representante  <br/> |[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta caixa de entrada do proprietário da caixa de correio  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Procurar ou localizar um email como representante  <br/> |[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta caixa de entrada do proprietário da caixa de correio  <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Obter um email como representante  <br/> |[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Atualizar um email como representante  <br/> |[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido por [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir um email como representante  <br/> |[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido por [EmailMessage. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Tenha em mente os seguintes pontos ao trabalhar com emails como representante:
  
- Se um representante só precisar trabalhar com solicitações de reunião e respostas, o representante não precisará acessar a pasta caixa de entrada. Para obter mais informações, consulte [tarefas de pré-requisito para acessar calendários como um representante](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).
    
- Quando um destinatário recebe uma mensagem que foi enviada em nome de um proprietário de caixa de correio, o remetente aparece como " *Representante* em nome do *proprietário da caixa de correio* ". 
    
> [!NOTE]
> Nos exemplos de código deste artigo, primary@contoso.com é o proprietário da caixa de correio. 
  
## <a name="prerequisite-tasks"></a>Tarefas de pré-requisito
<a name="bk_prereq"> </a>

Antes que um usuário possa acessar a pasta caixa de entrada do proprietário da caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para a pasta caixa de entrada do proprietário da caixa de correio. 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Criar e enviar um email como um representante usando a API gerenciada do EWS
<a name="bk_createewsma"> </a>

A API gerenciada do EWS permite que você use o objeto de serviço para que o usuário delegado crie e envie emails em nome do proprietário da caixa de correio. Este exemplo mostra como usar o método [Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) para salvar a mensagem na pasta Rascunhos do proprietário da caixa de correio e, em seguida, o método [SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) para enviar o email e salvar a mensagem na pasta Itens enviados do proprietário da caixa de correio. 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e que o representante recebeu as [permissões apropriadas para a pasta caixa de entrada, rascunhos e itens enviados do proprietário da caixa de correio](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).
  
```cs
public static void DelegateAccessCreateEmail(ExchangeService service)
{
    // Create an email message and provide it with connection 
    // configuration information by using an ExchangeService 
    // object named service.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Company Soccer Team";
    message.Body = "Are you interested in joining?";
    message.ToRecipients.Add("sadie@contoso.com");
    // Save the email to the mailbox owner's Drafts folder.
    // This method call results in a CreateItem call to EWS.
    // The FolderId parameter contains the context for the 
    // mailbox owner's Inbox folder. Any additional actions 
    // taken on this message will be performed in the mailbox 
    // owner's mailbox. 
    message.Save(new FolderId(WellKnownFolderName.Drafts, new Mailbox("primary@contoso.com")));
    // Send the email and save the message in the mailbox owner's 
    // Sent Items folder.
    // This method call results in a SendItem call to EWS.
    message.SendAndSaveCopy(new FolderId(WellKnownFolderName.SentItems, new Mailbox("primary@contoso.com")));
    Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" 
    + message.ToRecipients[0] + "' and saved in the Sent Items folder of the mailbox owner.");
}
```

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a>Criar e enviar um email como um representante usando o EWS
<a name="bk_createews"> </a>

O EWS permite que você use o objeto de serviço do usuário delegado para criar e enviar emails em nome do proprietário da caixa de correio. Este exemplo mostra como usar a operação [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar um email e a operação [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) para enviar o horário e salvá-lo na pasta Itens enviados do proprietário da caixa de correio. 
  
Essa é também a primeira solicitação XML que a API gerenciada do EWS envia quando você usa o método **Save** para [criar e enviar um email](#bk_createewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o email foi criado e salvo com êxito. A resposta também contém a ID do item de email recém-criado.
  
O valor de **ItemId** foi reduzido para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="iNRaAAA="
                        ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

Em seguida, use a operação **SendItem** para enviar a mensagem em nome do proprietário da caixa de correio e salvá-la na pasta Itens enviados do proprietário da caixa de correio. 
  
O valor de **ItemId** foi reduzido para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="iNRaAAA="
                  ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **SendItem** com uma mensagem [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o email foi enviado e salvo com êxito na pasta Itens enviados do proprietário da caixa de correio.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Procurar um email como um representante usando a API gerenciada do EWS
<a name="bk_searchewsma"> </a>

Para pesquisar um email, você deve usar um dos métodos [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você possa especificar a pasta caixa de entrada do proprietário da caixa de correio. 
  
```cs
static void DelegateAccessSearchEmailWithFilter(ExchangeService service)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    // Define the search filter.
    SearchFilter.ContainsSubstring filter = new SearchFilter.ContainsSubstring(ItemSchema.Subject, 
        "soccer", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching Inbox items. 
        // The parameters of FindItems must denote the mailbox owner,
        // mailbox, and Inbox folder.
        // This call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(new 
            FolderId(WellKnownFolderName.Inbox, "primary@contoso.com"), 
            filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

Depois que a chamada **FindItems** retorna uma resposta com uma ID, você pode obter, atualizar ou excluir esse email usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) – e não é necessário especificar o endereço SMTP do proprietário da caixa de correio. 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a>Procurar um email como um representante usando o EWS
<a name="bk_searchews"> </a>

O EWS permite que você use o objeto de serviço para que o usuário delegado pesquise emails que atendam a um conjunto de critérios de pesquisa. Este exemplo mostra como usar a operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar mensagens na pasta de caixa de entrada do proprietário que contenham a palavra "futebol" no assunto. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você [pesquisa um email](#bk_searchewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
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
          <t:Constant Value="soccer" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **FindItem** com uma mensagem [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pesquisa foi concluída com êxito. A resposta contém um elemento [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) para todos os emails que atenderem aos critérios de pesquisa. Nesse caso, somente um email é encontrado. 
  
O valor do elemento [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
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
              <t:Message>
                <t:ItemId Id="iNwoAAA="
                          ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQuu" />
                <t:Subject>Soccer team</t:Subject>
                <t:DateTimeReceived>2014-03-10T06:16:55Z</t:DateTimeReceived>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Agora que você tem o **ItemId** para o email que atende aos seus critérios, é possível obter, atualizar ou excluir esse email usando **ItemId** e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) -e não é necessário especificar o endereço SMTP do proprietário da caixa de correio. 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obter, atualizar ou excluir itens de email como um representante usando a API gerenciada do EWS
<a name="bk_geteswma"> </a>

Você pode usar a API gerenciada do EWS para obter, atualizar ou excluir um email da mesma maneira que você realiza essas ações quando não está usando o acesso de representante. A única diferença é que o objeto **ExchangeService** é para o usuário delegado. A ID do item incluída na chamada do método **BIND** identifica exclusivamente o item no repositório de caixa de correio, na pasta caixa de entrada do proprietário da caixa de correio. 
  
**Tabela 2. Métodos da API gerenciada do EWS que trabalham com email como um representante**

|**Tarefa**|**Método de API gerenciada do EWS**|**Exemplo de código**|
|:-----|:-----|:-----|
|Obter um email  <br/> |[Associá](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[Obter um item usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Atualizar um email  <br/> |[Vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido por [atualização](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[Atualizar um item usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Excluir um email  <br/> |[Vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido por [delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[Excluir um item usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a>Obter, atualizar ou excluir itens de email como um representante usando o EWS
<a name="bk_getews"> </a>

Você pode usar a API gerenciada do EWS para obter, atualizar ou excluir um email da mesma maneira que você realiza essas ações quando não está usando o acesso de representante. A única diferença é que o objeto de serviço é para o usuário delegado. A ID do item incluída na solicitação **GetItem** identifica exclusivamente o item no repositório de caixa de correio, na pasta caixa de entrada do proprietário da caixa de correio. 
  
**Tabela 3. Operações do EWS para trabalhar com o email como um representante**

|**Tarefa**|**Operação do EWS**|**Exemplo de código**|
|:-----|:-----|:-----|
|Obter um email  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obter um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Atualizar um email  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Atualizar um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Excluir um email  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[Excluir um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>Confira também

- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)    
- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    

