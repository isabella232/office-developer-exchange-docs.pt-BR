---
title: Contatos de acesso como um representante, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Saiba como acessar contatos como um representante, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: a7f695dcbe0693809817de84284294dff872aa9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750681"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a>Contatos de acesso como um representante, usando o EWS no Exchange

Saiba como acessar contatos como um representante, usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode usar a API gerenciada de EWS ou EWS dar um usuário acesso à pasta de contatos de um proprietário caixa de correio. O representante, em seguida, pode criar contatos em nome do proprietário da caixa de correio e recuperar, atualizar e excluir os contatos da pasta de contatos do proprietário da caixa de correio, dependendo de suas permissões.
  
Como um representante, use os métodos e as mesmas operações para acessar a pasta de contatos de um proprietário caixa de correio que você usa para acessar sua própria pasta de contatos. A principal diferença é que você precisa usar [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de contato e, em seguida, depois de identificar a ID do item, você pode usar [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item. 
  
**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para acessar um contato como um representante**

|**Se você quiser …**|**Use este método de API gerenciada de EWS …**|**Use essa operação EWS …**|
|:-----|:-----|:-----|
|Criar um contato como um representante  <br/> |[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Criar vários contatos como um representante  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Resolver um contato como um representante  <br/> |[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio  <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Pesquise ou localizar um contato como um representante  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio  <br/> |
|Obtenha um contato como um representante  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Atualizar um contato como um representante  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) seguido [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir um contato como um representante  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) seguido [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
> [!NOTE]
> Os exemplos de código neste artigo, primary@contoso.com é o proprietário da caixa de correio. 

<a name="bk_prereq"> </a>

## <a name="prerequisite-tasks"></a>Tarefas de pré-requisito

Antes de um usuário pode acessar a pasta de contatos do proprietário da caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) à pasta de contatos do proprietário da caixa de correio. 

<a name="bk_createewsma"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Criar um contato como um representante, usando a API gerenciada de EWS

A API gerenciada de EWS permite que você use o objeto de serviço para o usuário delegado para criar contatos para o proprietário da caixa de correio. Este exemplo mostra como usar o método [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes. 
  
Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e o delegado recebeu as permissões apropriadas para a pasta de contatos do proprietário da caixa de correio. 
  
```cs
 public static void DelegateAccessCreateContact(ExchangeService service)
{
    // Create the contact.
    Contact contact = new Contact(service);
    // Specify the name and how the contact should be filed.
    contact.GivenName = "Brian";
    contact.MiddleName = "David";
    contact.Surname = "Johnson";
    contact.FileAsMapping = FileAsMapping.SurnameCommaGivenName;
    // Specify the company name.
    contact.CompanyName = "Contoso";
    // Specify the business, home, and car phone numbers.
    contact.PhoneNumbers[PhoneNumberKey.BusinessPhone] = "425-555-0110";
    contact.PhoneNumbers[PhoneNumberKey.HomePhone] = "425-555-0120";
    contact.PhoneNumbers[PhoneNumberKey.CarPhone] = "425-555-0130";
    // Specify two email addresses.
    contact.EmailAddresses[EmailAddressKey.EmailAddress1] = 
        new EmailAddress("brian_1@contoso.com");
    contact.EmailAddresses[EmailAddressKey.EmailAddress2] = 
        new EmailAddress("brian_2@contoso.com");
    // Save the contact in the mailbox owner's Contacts folder.
    // This method call results in a CreateItem call to EWS. 
    // The contact identifier contains the context for the mailbox owner's 
    // Contact folder. Any additional actions take on this contact will 
    // be performed in the mailbox owner's mailbox. 
    contact.Save(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    // Verify that the contact was created.
    // This method call results in a GetItem call to EWS
    // to load the display name property on the contact. 
    contact.Load(new PropertySet (ContactSchema.DisplayName));
    Console.WriteLine("\nContact created: " + contact.DisplayName + "\n");
}
```

Observe que, quando você salva o item, a chamada do método [Salvar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) deve identificar pasta de contatos do proprietário da caixa de correio. Se a pasta de contatos do proprietário da caixa de correio não for especificada, a solicitação de reunião obtém salvos não pasta de contatos do proprietário da caixa de correio e de pasta de contatos do representante. Você pode incluir uma pasta de contatos do proprietário da caixa de correio na chamada do método **Salvar** na forma dois. Recomendamos que você criar uma nova instância do objeto [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) usando o [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o endereço SMTP do proprietário da caixa de correio. 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

No entanto, você também pode [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para a pasta Contatos em primeiro lugar e, em seguida, usar a identificação da pasta na chamada do método **Salvar** . Lembre-se, no entanto, se esse cria uma chamada de EWS extra. 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<a name="bk_createews"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a>Criar um contato como um representante usando o EWS

EWS permite que você use o objeto de serviço para o usuário delegado para criar itens de contato do proprietário da caixa de correio. Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar um contato. 
  
Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **Save** para [criar um contato](#bk_createewsma).
  
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
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Contact>
          <t:FileAsMapping>LastCommaFirst</t:FileAsMapping>
          <t:GivenName>Brian</t:GivenName>
          <t:MiddleName>David</t:MiddleName>
          <t:CompanyName>Contoso</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">brian_1@contoso.com</t:Entry>
            <t:Entry Key="EmailAddress2">brian_2@contoso.com</t:Entry>
          </t:EmailAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">425-555-0110</t:Entry>
            <t:Entry Key="HomePhone">425-555-0120</t:Entry>
            <t:Entry Key="CarPhone">425-555-0130</t:Entry>
          </t:PhoneNumbers>
          <t:Surname>Johnson</t:Surname>
        </t:Contact>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se o contato foi criado com êxito. A resposta também contém a ID de item do contato recém-criado.

<a name="bk_resolveewsma"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Resolver um contato como um representante, usando a API gerenciada de EWS

Para localizar um contato, com base em um nome ambíguo possivelmente ou termo, você deve usar um dos métodos [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você pode especificar uma pasta de contatos do proprietário da caixa de correio. 
  
```cs
private static void DelegateAccessResolveContacts(ExchangeService service)
{
    // Create a list to store folders to search.
    List<FolderId> folders = new List<FolderId>();
   
    // Add the mailbox owner's folder to the list.
    folders.Add(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    
    // Resolve the ambiguous name "Johnson".
    // This method call results in a ResolveNames call to EWS.
    NameResolutionCollection resolvedNames = service.ResolveName(
        "johnson", folders, ResolveNameSearchLocation.ContactsOnly, true);
    // Output the list of candidate email addresses and contact names.
    foreach (NameResolution nameRes in resolvedNames)
    {
        Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
        Console.WriteLine("Contact ID: " + nameRes.Mailbox.Id);
    }
}
```

Depois que a chamada do método **ResolveNames** retornará uma resposta com uma ID, você pode [obter, atualizar ou excluir o contato](#bk_getewsma) usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio. 

<a name="bk_resolveews"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a>Resolver um contato como um representante usando o EWS

EWS permite que você use o objeto de serviço para o usuário delegado para resolver nomes de parciais na pasta de contatos do proprietário da caixa de correio. Este exemplo mostra como usar a operação [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) para localizar reuniões na pasta de contatos do proprietário da caixa de correio que contêm a palavra "johnson". 
  
Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **ResolveName** resolver [um contato](#bk_resolveewsma).
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ResolveNames ReturnFullContactData="true"
                    SearchScope="Contacts">
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
      <m:UnresolvedEntry>johnson</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **ResolveNames** com uma mensagem de [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a operação concluída com êxito e encontrados apenas um resultado ou **ErrorNameResolutionMultipleResults** se vários resultados encontrados - que é o que é mostrado no exemplo de código de terceiro com base no contato [criar um contato como um representante usando a API gerenciada de EWS](#bk_createewsma). A resposta também contém o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de cada resultado. 
  
O valor do elemento **ItemId** foi reduzido para melhorar a legibilidade. 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Warning">
          <m:MessageText>Multiple results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionMultipleResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:ResolutionSet TotalItemsInView="2"
                           IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_1@contoso.com</t:Name>
                <t:EmailAddress>brian_1@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_2@contoso.com</t:Name>
                <t:EmailAddress>brian_2@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>
```

Agora que você tem o **ItemId** para os contatos que correspondam ao nome ambíguo, você pode [obter, atualizar ou excluir itens de contato como um representante, usando o EWS](#bk_getews) by using the **ItemId** e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;e você não precisará especificar endereço de SMTP do proprietário da caixa de correio. 

<a name="bk_getewsma"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obter, atualizar ou excluir itens de contato como um representante, usando a API gerenciada de EWS

Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir um contato da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante. A única diferença é que o objeto de serviço é para o usuário delegado. A ID do item incluída na chamada do método **vincular** exclusivamente identifica o item no repositório de caixa de correio, na pasta de contatos do proprietário da caixa de correio. 
  
**Tabela 2. Trabalhando com um contato como um representante de métodos de API gerenciada de EWS**

|**Task**|**Método API gerenciada de EWS**|**Exemplo de código**|
|:-----|:-----|:-----|
|Obtenha um contato  <br/> |[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Obter um item usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Atualização de um contato  <br/> |[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido de [atualização](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Atualização de um item usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Excluir um contato  <br/> |[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Excluir](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Excluir um item usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<a name="bk_getews"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a>Obter, atualizar ou excluir itens de contato como um representante usando o EWS

Você pode usar o EWS para obter, atualizar ou excluir um contato de reunião ou compromisso da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante. A única diferença é que o objeto de serviço é para o usuário delegado. A ID do item incluída na solicitação [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) exclusivamente identifica o item no repositório de caixa de correio, na pasta de contatos do proprietário da caixa de correio. 
  
**Tabela 3. Operações do EWS para trabalhar com um contato como um representante**

|**Task**|**Operação do EWS**|**Amostra**|
|:-----|:-----|:-----|
|Obtenha um contato  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obter um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Atualização de um contato  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Atualizar um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Excluir um contato  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Excluir um item usando o EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>Confira também

- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
- [Adicionar e remover representantes usando o EWS no Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [Pessoas e contatos no EWS no Exchange](people-and-contacts-in-ews-in-exchange.md)
- [Resolver nomes de ambíguos, usando o EWS no Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

