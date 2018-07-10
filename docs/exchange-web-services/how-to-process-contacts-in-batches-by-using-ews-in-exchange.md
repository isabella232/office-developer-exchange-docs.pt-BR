---
title: Contatos de processo em lotes, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 455f475b-cb19-4e7a-8ff3-92f7028fceb0
description: Saiba como criar, obter, atualizar e excluir os lotes de contatos em uma única chamada usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 7dfbda7fe5e077f92bcf7ebd40af40d76c2d2d22
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750814"
---
# <a name="process-contacts-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="7e505-103">Contatos de processo em lotes, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e505-103">Process contacts in batches by using EWS in Exchange</span></span>

<span data-ttu-id="7e505-104">Saiba como criar, obter, atualizar e excluir os lotes de contatos em uma única chamada usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e505-104">Learn how to create, get, update, and delete batches of contacts in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7e505-105">Você pode usar a API gerenciada de EWS ou torna o EWS para trabalhar com lotes de contatos para reduzir o número de chamadas de um cliente com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e505-105">You can use the EWS Managed API or EWS to work with batches of contacts to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="7e505-106">Quando você usa o EWS Managed API para criar, obter, atualizar e excluir os contatos em lotes, você usar métodos do objeto [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , enquanto que, quando você trabalha com contatos único, você usar os métodos do objeto de [contato](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7e505-106">When you use the EWS Managed API to create, get, update, and delete contacts in batches, you use [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single contacts, you use [Contact](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="7e505-107">Se você estiver usando o EWS, use as mesmas operações para trabalhar com um único contato e de lotes de contatos.</span><span class="sxs-lookup"><span data-stu-id="7e505-107">If you are using EWS, you use the same operations to work with both a single contact and batches of contacts.</span></span> 
  
<span data-ttu-id="7e505-108">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para trabalhar com os lotes de contatos**</span><span class="sxs-lookup"><span data-stu-id="7e505-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of contacts**</span></span>

|<span data-ttu-id="7e505-109">**Para...**</span><span class="sxs-lookup"><span data-stu-id="7e505-109">**In order to…**</span></span>|<span data-ttu-id="7e505-110">**Use este método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="7e505-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="7e505-111">**Use esta operação EWS**</span><span class="sxs-lookup"><span data-stu-id="7e505-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7e505-112">Criar contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="7e505-112">Create contacts in batches</span></span>  <br/> |[<span data-ttu-id="7e505-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="7e505-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7e505-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="7e505-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="7e505-115">Obtenha os contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="7e505-115">Get contacts in batches</span></span>  <br/> |<span data-ttu-id="7e505-116">[ExchangeService.BindToItems](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) ou [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/pt-br/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7e505-116">[ExchangeService.BindToItems](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) or [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/pt-br/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="7e505-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="7e505-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="7e505-118">Contatos de atualização em lotes</span><span class="sxs-lookup"><span data-stu-id="7e505-118">Update contacts in batches</span></span>  <br/> |[<span data-ttu-id="7e505-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="7e505-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/pt-br/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7e505-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="7e505-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="7e505-121">Excluir os contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="7e505-121">Delete contacts in batches</span></span>  <br/> |[<span data-ttu-id="7e505-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="7e505-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/pt-br/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7e505-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="7e505-123">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="7e505-124">Neste artigo, você aprenderá como concluir as tarefas básicas para lotes de contatos usando o EWS Managed API ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="7e505-124">In this article, you'll learn how to complete basic tasks for batches of contacts by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="7e505-125">Criar contatos em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-125">Create contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="7e505-126"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-126"></span></span>

<span data-ttu-id="7e505-127">Você pode criar contatos em lotes, usando o método API gerenciada de EWS [CreateItems](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-127">You can create contacts in batches by using the EWS Managed API [CreateItems](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="7e505-128">Este exemplo cria objetos de [contato](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) três localmente, adiciona a cada contato a uma coleção e chama o método **CreateItems** na coleção de contatos.</span><span class="sxs-lookup"><span data-stu-id="7e505-128">This example creates three [Contact](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) objects locally, adds each contact to a collection, then calls the **CreateItems** method on the collection of contacts.</span></span> 
  
```cs
public static Collection<ItemId> CreateContactsInBatch(ExchangeService service)
{
    // These are unsaved local instances of a Contact object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    Contact contact1 = new Contact(service);
    Contact contact2 = new Contact(service);
    Contact contact3 = new Contact(service);
    // Set the properties on the first contact.
    contact1.DisplayName = "Sadie Daniels";
    contact1.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("sadie@contoso.com");
    
    // Set the properties on the second contact.
    contact2.DisplayName = "Alfred Welker";
    contact2.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("alfred@contoso.com");
    // Set the properties on the third contact.
    contact3.DisplayName = "Hope Gross";
    contact3.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("hope@contoso.com");
    // Add the Contact objects to a collection.
    Collection<Contact> contactItems = new Collection<Contact>() { contact1, contact2, contact3 };
    // Create the batch of contacts on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(contactItems, WellKnownFolderName.Contacts, null, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created contacts.
    foreach (Contact contact in contactItems)
    {
        try
        {
            itemIds.Add(contact.Id);
            Console.WriteLine("Contact '{0}' created successfully.", contact.DisplayName);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating contact {0}: {1}", contact.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Determine whether the CreateItems method call completed successfully.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created contacts were successfully created in the Contacts folder.");
            Console.WriteLine("\r\n");
    }
   
    // If the method did not return success, print the result message for each contact.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (contact {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

## <a name="create-contacts-in-batches-by-using-ews"></a><span data-ttu-id="7e505-129">Criar contatos em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-129">Create contacts in batches by using EWS</span></span>
<span data-ttu-id="7e505-130"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-130"></span></span>

<span data-ttu-id="7e505-131">Você pode criar contatos em lotes, usando a operação [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-131">You can create contacts in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="7e505-132">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS criar [contatos em lotes](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="7e505-132">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create contacts in batches](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:CreateItem>
        <m:SavedItemFolderId>
          <t:DistinguishedFolderId Id="contacts" />
        </m:SavedItemFolderId>
        <m:Items>
          <t:Contact>
            <t:DisplayName>Sadie Daniels</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">sadie@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
          <t:Contact>
            <t:DisplayName>Alfred Welker</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">alfred@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
          <t:Contact>
            <t:DisplayName>Hope Gross</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">hope@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
        </m:Items>
      </m:CreateItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="7e505-133">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada um dos novos contatos, que indica que cada contato foi criado e salvo com êxito.</span><span class="sxs-lookup"><span data-stu-id="7e505-133">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new contacts, which indicates that each contact was created and saved successfully.</span></span> 
  
## <a name="get-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="7e505-134">Obter contatos em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-134">Get contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="7e505-135"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-135"></span></span>

<span data-ttu-id="7e505-136">Você pode obter contatos em lotes, usando o método API gerenciada de EWS [BindToItems](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-136">You can get contacts in batches by using the EWS Managed API [BindToItems](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="7e505-137">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e505-137">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<Contact> BatchGetContactItems(ExchangeService service, Collection<ItemId> itemIds)
        {
            // Create a property set that limits the properties returned by the Bind method to only those that are required.
            PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ContactSchema.DisplayName);
            // Get the items from the server.
            // This method call results in a GetItem call to EWS.
            ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);
            // Instantiate a collection of Contact objects to populate from the values that are returned by the Exchange server.
            Collection<Contact> contactItems = new Collection<Contact>();
            foreach (GetItemResponse getItemResponse in response)
            {
                try
                {
                    Item item = getItemResponse.Item;
                    Contact contact = (Contact)item;
                    contactItems.Add(contact);
                    // Print out confirmation and the last eight characters of the item ID.
                    Console.WriteLine("Found item {0}.", contact.Id.ToString().Substring(144));
                }
                catch (Exception ex)
                {
                    Console.WriteLine("Exception while getting a contact: {0}", ex.Message);
                }
            }
            // Check for success of the BindToItems method call.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("All contacts retrieved successfully.");
                Console.WriteLine("\r\n");
            }
            return contactItems;
        }

```

## <a name="get-contacts-in-batches-by-using-ews"></a><span data-ttu-id="7e505-138">Obter contatos em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-138">Get contacts in batches by using EWS</span></span>
<span data-ttu-id="7e505-139"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-139"></span></span>

<span data-ttu-id="7e505-140">Você pode obter contatos em lotes, usando a operação de EWS [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) e o código no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-140">You can get contacts in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="7e505-141">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [obter os contatos em lotes](#bk_EWSMAGet).</span><span class="sxs-lookup"><span data-stu-id="7e505-141">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get contacts in batches](#bk_EWSMAGet).</span></span> <span data-ttu-id="7e505-142">O atributo **ItemId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e505-142">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetItem>
        <m:ItemShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="contacts:DisplayName" />
          </t:AdditionalProperties>
        </m:ItemShape>
        <m:ItemIds>
          <t:ItemId Id="ceJwVAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yS" />
          <t:ItemId Id="ceJwWAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yT" />
          <t:ItemId Id="ceJwXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yU" />
        </m:ItemIds>
      </m:GetItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="7e505-143">O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui a ID e o nome de exibição para cada um dos contatos solicitados.</span><span class="sxs-lookup"><span data-stu-id="7e505-143">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the ID and the display name for each of the requested contacts.</span></span> 
  
## <a name="update-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="7e505-144">Contatos de atualização em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-144">Update contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="7e505-145"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-145"></span></span>

<span data-ttu-id="7e505-146">Você pode atualizar contatos em lotes, usando o método API gerenciada de EWS [UpdateItems](http://msdn.microsoft.com/pt-br/library/dd634705%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-146">You can update contacts in batches by using the EWS Managed API [UpdateItems](http://msdn.microsoft.com/pt-br/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="7e505-147">O exemplo anterior cria um contato, mas não especifica que eles trabalham para.</span><span class="sxs-lookup"><span data-stu-id="7e505-147">The previous example creates the contact but does not specify who they work for.</span></span> <span data-ttu-id="7e505-148">Você pode usar o código neste exemplo, para atualizar todos os seus contatos ao mesmo tempo para incluir o nome da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="7e505-148">You can use the code in this example to update all your contacts at once to include their company name.</span></span> 
  
<span data-ttu-id="7e505-149">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e505-149">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<Contact> BatchUpdateContactItems(ExchangeService service, Collection<Contact> contactItems)
        {
            // Update the company name of each contact locally.
            foreach (Contact contact in contactItems)
            {
                // Update the company name of the contact.
                contact.CompanyName = "Contoso";
                // Print out confirmation with the last eight characters of the item ID and the contact company name.
                Console.WriteLine("Updated local contact {0} with the company name '{1}'.", contact.Id.ToString().Substring(144), contact.CompanyName);
            }
            
            // Send the item updates to the server.
            // This method call results in an UpdateItem call to EWS.
            ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(contactItems, WellKnownFolderName.Contacts, ConflictResolutionMode.AutoResolve, null, null);
            // Verify the success of the UpdateItems method call.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("All contacts updated successfully.\r\n");
            }
            // If the method did not return success, print the result message for each contact.
            else
            {
                Console.WriteLine("All contacts were not successfully saved on the server.\r\n");
                int counter = 1;
                foreach (ServiceResponse resp in response)
                {
                    Console.WriteLine("Result for (contact {0}): {1}", counter, resp.Result);
                    Console.WriteLine("Error Code: {0}", resp.ErrorCode);
                    Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
                    counter++;
                }
            }
            return contactItems;
        }    

```

## <a name="update-contacts-in-batches-by-using-ews"></a><span data-ttu-id="7e505-150">Contatos de atualização em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-150">Update contacts in batches by using EWS</span></span>
<span data-ttu-id="7e505-151"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-151"></span></span>

<span data-ttu-id="7e505-152">Você pode atualizar contatos em lotes, usando a operação [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-152">You can update contacts in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="7e505-153">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Atualizar contatos em lotes](#bk_EWSMAUpdate).</span><span class="sxs-lookup"><span data-stu-id="7e505-153">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update contacts in batches](#bk_EWSMAUpdate).</span></span> <span data-ttu-id="7e505-154">O atributo **ItemId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e505-154">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:UpdateItem ConflictResolution="AutoResolve">
        <m:SavedItemFolderId>
          <t:DistinguishedFolderId Id="contacts" />
        </m:SavedItemFolderId>
        <m:ItemChanges>
          <t:ItemChange>
            <t:ItemId Id="ceJwVAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yS" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
          <t:ItemChange>
            <t:ItemId Id="ceJwWAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yT" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
          <t:ItemChange>
            <t:ItemId Id="ceJwXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yU" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
        </m:ItemChanges>
      </m:UpdateItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="7e505-155">O servidor responde à solicitação **UpdateItem** com uma mensagem de [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que cada uma das atualizações foi salvo com êxito no servidor.</span><span class="sxs-lookup"><span data-stu-id="7e505-155">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="7e505-156">Todos os conflitos são relatados no elemento [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7e505-156">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="7e505-157">Excluir os contatos em lotes usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-157">Delete contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="7e505-158"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-158"></span></span>

<span data-ttu-id="7e505-159">Você pode excluir os contatos em lotes, usando o método [DeleteItems](http://msdn.microsoft.com/pt-br/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-159">You can delete contacts in batches by using the [DeleteItems](http://msdn.microsoft.com/pt-br/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="7e505-160">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e505-160">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void BatchDeleteContactItems(ExchangeService service, Collection<ItemId> itemIds)
        {
            // Delete the batch of contact objects.
            // This method call results in an DeleteItem call to EWS.
            ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);
            // Check for success of the DeleteItems method call.
            // DeleteItems returns success even if it does not find all the item IDs.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("Contacts deleted successfully.\r\n");
            }
            // If the method did not return success, print a message.
            else
            {
                Console.WriteLine("Not all contacts deleted successfully.\r\n");
            }
        }

```

## <a name="delete-contacts-in-batches-by-using-ews"></a><span data-ttu-id="7e505-161">Excluir os contatos em lotes usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7e505-161">Delete contacts in batches by using EWS</span></span>
<span data-ttu-id="7e505-162"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-162"></span></span>

<span data-ttu-id="7e505-163">Você pode excluir os contatos em lotes, usando a operação [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="7e505-163">You can delete contacts in batches by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="7e505-164">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Excluir os contatos em lotes](#bk_EWSMADelete).</span><span class="sxs-lookup"><span data-stu-id="7e505-164">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete contacts in batches](#bk_EWSMADelete).</span></span> <span data-ttu-id="7e505-165">O atributo **ItemId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e505-165">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:DeleteItem DeleteType="SoftDelete" AffectedTaskOccurrences="AllOccurrences">
        <m:ItemIds>
          <t:ItemId Id="ceJwYAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yY" />
          <t:ItemId Id="ceJwZAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yZ" />
          <t:ItemId Id="ceJwaAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51ya" />
        </m:ItemIds>
      </m:DeleteItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="7e505-166">O servidor responde à solicitação **DeleteItem** com uma mensagem de [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada item que foi removido.</span><span class="sxs-lookup"><span data-stu-id="7e505-166">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="7e505-167">Observe que a operação também retorna sucesso se a ID do item não pôde ser encontrada.</span><span class="sxs-lookup"><span data-stu-id="7e505-167">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="7e505-168">Verificando se um processo em lote foi concluída com êxito</span><span class="sxs-lookup"><span data-stu-id="7e505-168">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="7e505-169"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="7e505-169"></span></span>

<span data-ttu-id="7e505-170">Quando um ou mais contatos em uma solicitação de lote não podem ser processados, conforme solicitado, um erro será retornado para cada contato que falharam e o restante dos contatos no lote são processadas conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="7e505-170">When one or more contacts in a batched request can't be processed as requested, an error is returned for each contact that failed, and the rest of the contacts in the batch are processed as expected.</span></span> <span data-ttu-id="7e505-171">Falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser recuperado ou atualizado, ou se o item movido para uma pasta diferente e, portanto, tem uma nova ID de item e não pode ser modificado com a ID de item enviada.</span><span class="sxs-lookup"><span data-stu-id="7e505-171">Failures in batch processing can occur if the item was deleted, and therefore can't be retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="7e505-172">As informações nesta seção mostram como obter os detalhes de erro sobre falhas no processamento em lotes de contatos.</span><span class="sxs-lookup"><span data-stu-id="7e505-172">The information in this section shows how to get error details about failures in batch processing of contacts.</span></span>
  
<span data-ttu-id="7e505-173">Para verificar o sucesso de um processo em lote usando a API gerenciada de EWS, você pode verificar se a propriedade [OverallResult](http://msdn.microsoft.com/pt-br/library/dd634515%28v=exchg.80%29.aspx) do [ServiceResponseCollection](http://msdn.microsoft.com/pt-br/library/dd633715%28v=exchg.80%29.aspx) for igual a [ServiceResult.Success](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7e505-173">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/pt-br/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/pt-br/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="7e505-174">Nesse caso, todos os contatos foram processados com êxito.</span><span class="sxs-lookup"><span data-stu-id="7e505-174">If so, all the contacts were processed successfully.</span></span> <span data-ttu-id="7e505-175">Se o **OverallResult** não for igual a **ServiceResult.Success**, um ou mais dos contatos que não foram processadas com êxito.</span><span class="sxs-lookup"><span data-stu-id="7e505-175">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the contacts were not processed successfully.</span></span> <span data-ttu-id="7e505-176">Cada um dos objetos retornados no **ServiceResponseCollection** contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="7e505-176">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="7e505-177">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="7e505-177">ErrorCode</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="7e505-178">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7e505-178">ErrorDetails</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="7e505-179">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="7e505-179">ErrorMessage</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="7e505-180">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="7e505-180">ErrorProperties</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="7e505-181">Resultado</span><span class="sxs-lookup"><span data-stu-id="7e505-181">Result</span></span>](http://msdn.microsoft.com/pt-br/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="7e505-182">Essas propriedades contêm informações sobre por que os contatos não pôde ser processados conforme solicitado.</span><span class="sxs-lookup"><span data-stu-id="7e505-182">These properties contain information about why the contacts could not be processed as requested.</span></span> <span data-ttu-id="7e505-183">Os exemplos neste artigo imprimam o **resultado**, **ErrorCode**, e falha de **ErrorMessage** para cada contato.</span><span class="sxs-lookup"><span data-stu-id="7e505-183">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed contact.</span></span> <span data-ttu-id="7e505-184">Você pode usar estes resultados para investigar o problema.</span><span class="sxs-lookup"><span data-stu-id="7e505-184">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="7e505-185">Para o EWS, para verificar o sucesso de um processo em lote, verifique o atributo [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) para cada item que estão sendo processada.</span><span class="sxs-lookup"><span data-stu-id="7e505-185">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="7e505-186">Veja a seguir a estrutura básica do **ResponseMessageType**, o tipo de base da resposta que todas as mensagens são derivadas.</span><span class="sxs-lookup"><span data-stu-id="7e505-186">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="7e505-187">O atributo **ResponseClass** é definido como **sucesso** se o contato foi processado com êxito, ou **erro** se o contato não foi processado com êxito.</span><span class="sxs-lookup"><span data-stu-id="7e505-187">The **ResponseClass** attribute is set to **Success** if the contact was processed successfully, or **Error** if the contact was not processed successfully.</span></span> <span data-ttu-id="7e505-188">Para contatos, você não encontrará um **Aviso** durante o processamento em lotes.</span><span class="sxs-lookup"><span data-stu-id="7e505-188">For contacts, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="7e505-189">Se o **ResponseClass** for **sucesso**, o elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) que segue também sempre é definido como **NoError**.</span><span class="sxs-lookup"><span data-stu-id="7e505-189">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="7e505-190">Se a **ResponseClass** **erro**, você precisará verificar os valores dos elementos [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**e [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) para determinar o que causou o problema.</span><span class="sxs-lookup"><span data-stu-id="7e505-190">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="7e505-191">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) não é usada no momento.</span><span class="sxs-lookup"><span data-stu-id="7e505-191">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7e505-192">Confira também</span><span class="sxs-lookup"><span data-stu-id="7e505-192">See also</span></span>


- [<span data-ttu-id="7e505-193">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e505-193">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="7e505-194">Processar as mensagens de email em lotes, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e505-194">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7e505-195">Processar itens de calendário em lotes no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e505-195">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    

