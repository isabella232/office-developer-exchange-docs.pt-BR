---
title: Processar contatos em lotes usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 455f475b-cb19-4e7a-8ff3-92f7028fceb0
description: Saiba como criar, obter, atualizar e excluir lotes de contatos em uma única chamada usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 2e122f67693b4ba46120104d9a1f6d36b4d86f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527800"
---
# <a name="process-contacts-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="5f747-103">Processar contatos em lotes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5f747-103">Process contacts in batches by using EWS in Exchange</span></span>

<span data-ttu-id="5f747-104">Saiba como criar, obter, atualizar e excluir lotes de contatos em uma única chamada usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f747-104">Learn how to create, get, update, and delete batches of contacts in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5f747-105">Você pode usar a API gerenciada do EWS ou o EWS para trabalhar com lotes de contatos para reduzir o número de chamadas feitas por um cliente para um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f747-105">You can use the EWS Managed API or EWS to work with batches of contacts to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="5f747-106">Quando você usa a API gerenciada do EWS para criar, obter, atualizar e excluir contatos em lotes, usa métodos de objeto do [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , enquanto quando você trabalha com contatos únicos, usa métodos de objeto de [contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5f747-106">When you use the EWS Managed API to create, get, update, and delete contacts in batches, you use [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single contacts, you use [Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="5f747-107">Se você estiver usando o EWS, use as mesmas operações para trabalhar com um único contato e lotes de contatos.</span><span class="sxs-lookup"><span data-stu-id="5f747-107">If you are using EWS, you use the same operations to work with both a single contact and batches of contacts.</span></span> 
  
<span data-ttu-id="5f747-108">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com lotes de contatos**</span><span class="sxs-lookup"><span data-stu-id="5f747-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of contacts**</span></span>

|<span data-ttu-id="5f747-109">**Para...**</span><span class="sxs-lookup"><span data-stu-id="5f747-109">**In order to…**</span></span>|<span data-ttu-id="5f747-110">**Usar este método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="5f747-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="5f747-111">**Use esta operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="5f747-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5f747-112">Criar contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="5f747-112">Create contacts in batches</span></span>  <br/> |[<span data-ttu-id="5f747-113">ExchangeService. CreateItems</span><span class="sxs-lookup"><span data-stu-id="5f747-113">ExchangeService.CreateItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5f747-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="5f747-114">CreateItem</span></span>](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5f747-115">Obter contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="5f747-115">Get contacts in batches</span></span>  <br/> |<span data-ttu-id="5f747-116">[ExchangeService. BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) ou [ExchangeService. LoadPropertiesForItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5f747-116">[ExchangeService.BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) or [ExchangeService.LoadPropertiesForItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="5f747-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="5f747-117">GetItem</span></span>](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5f747-118">Atualizar contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="5f747-118">Update contacts in batches</span></span>  <br/> |[<span data-ttu-id="5f747-119">ExchangeService. UpdateItems</span><span class="sxs-lookup"><span data-stu-id="5f747-119">ExchangeService.UpdateItems</span></span>](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5f747-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5f747-120">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5f747-121">Excluir contatos em lotes</span><span class="sxs-lookup"><span data-stu-id="5f747-121">Delete contacts in batches</span></span>  <br/> |[<span data-ttu-id="5f747-122">ExchangeService. DeleteItems</span><span class="sxs-lookup"><span data-stu-id="5f747-122">ExchangeService.DeleteItems</span></span>](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5f747-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5f747-123">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="5f747-124">Neste artigo, você aprenderá a concluir tarefas básicas para lotes de contatos usando a API gerenciada do EWS ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="5f747-124">In this article, you'll learn how to complete basic tasks for batches of contacts by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="5f747-125">Criar contatos em lotes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-125">Create contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="5f747-126"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-126"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="5f747-127">Você pode criar contatos em lotes usando o método [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) da API gerenciada do EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-127">You can create contacts in batches by using the EWS Managed API [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="5f747-128">Este exemplo cria três objetos de [contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) localmente, adiciona cada contato a uma coleção e, em seguida, chama o método **CreateItems** na coleção de contatos.</span><span class="sxs-lookup"><span data-stu-id="5f747-128">This example creates three [Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) objects locally, adds each contact to a collection, then calls the **CreateItems** method on the collection of contacts.</span></span> 
  
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

## <a name="create-contacts-in-batches-by-using-ews"></a><span data-ttu-id="5f747-129">Criar contatos em lotes usando o EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-129">Create contacts in batches by using EWS</span></span>
<span data-ttu-id="5f747-130"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-130"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="5f747-131">Você pode criar contatos em lotes usando a operação [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-131">You can create contacts in batches by using the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="5f747-132">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [criar contatos em lotes](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="5f747-132">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create contacts in batches](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5f747-133">O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para cada um dos novos contatos, que indica que cada contato foi criado e salvo com êxito.</span><span class="sxs-lookup"><span data-stu-id="5f747-133">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new contacts, which indicates that each contact was created and saved successfully.</span></span> 
  
## <a name="get-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="5f747-134">Obter contatos em lotes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-134">Get contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="5f747-135"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-135"><a name="bk_EWSMAGet"> </a></span></span>

<span data-ttu-id="5f747-136">Você pode obter contatos em lotes usando o método [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) da API gerenciada do EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-136">You can get contacts in batches by using the EWS Managed API [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="5f747-137">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f747-137">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="get-contacts-in-batches-by-using-ews"></a><span data-ttu-id="5f747-138">Obter contatos em lotes usando o EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-138">Get contacts in batches by using EWS</span></span>
<span data-ttu-id="5f747-139"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-139"><a name="bk_EWSMAGet"> </a></span></span>

<span data-ttu-id="5f747-140">Você pode obter contatos em lotes usando a operação [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) do EWS e o código no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-140">You can get contacts in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="5f747-141">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [obter contatos em lotes](#bk_EWSMAGet).</span><span class="sxs-lookup"><span data-stu-id="5f747-141">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get contacts in batches](#bk_EWSMAGet).</span></span> <span data-ttu-id="5f747-142">O atributo **ItemId** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f747-142">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5f747-143">O servidor responde à solicitação **GetItem** com uma mensagem [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui a ID e o nome para exibição de cada um dos contatos solicitados.</span><span class="sxs-lookup"><span data-stu-id="5f747-143">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the ID and the display name for each of the requested contacts.</span></span> 
  
## <a name="update-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="5f747-144">Atualizar contatos em lotes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-144">Update contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="5f747-145"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-145"><a name="bk_EWSMAUpdate"> </a></span></span>

<span data-ttu-id="5f747-146">Você pode atualizar contatos em lotes usando o método [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) da API gerenciada do EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-146">You can update contacts in batches by using the EWS Managed API [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="5f747-147">O exemplo anterior cria o contato, mas não especifica de quem eles trabalham.</span><span class="sxs-lookup"><span data-stu-id="5f747-147">The previous example creates the contact but does not specify who they work for.</span></span> <span data-ttu-id="5f747-148">Você pode usar o código neste exemplo para atualizar todos os seus contatos ao mesmo tempo para incluir o nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="5f747-148">You can use the code in this example to update all your contacts at once to include their company name.</span></span> 
  
<span data-ttu-id="5f747-149">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f747-149">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="update-contacts-in-batches-by-using-ews"></a><span data-ttu-id="5f747-150">Atualizar contatos em lotes usando o EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-150">Update contacts in batches by using EWS</span></span>
<span data-ttu-id="5f747-151"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-151"><a name="bk_EWSMAUpdate"> </a></span></span>

<span data-ttu-id="5f747-152">Você pode atualizar contatos em lotes usando a operação [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) do EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-152">You can update contacts in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="5f747-153">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [atualizar contatos em lotes](#bk_EWSMAUpdate).</span><span class="sxs-lookup"><span data-stu-id="5f747-153">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update contacts in batches](#bk_EWSMAUpdate).</span></span> <span data-ttu-id="5f747-154">O atributo **ItemId** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f747-154">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5f747-155">O servidor responde à solicitação **UpdateItem** com uma mensagem [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que cada uma das atualizações foi salva com êxito no servidor.</span><span class="sxs-lookup"><span data-stu-id="5f747-155">The server responds to the **UpdateItem** request with an [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="5f747-156">Todos os conflitos são relatados no elemento [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5f747-156">Any conflicts are reported in the [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="5f747-157">Excluir contatos em lotes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-157">Delete contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="5f747-158"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-158"><a name="bk_EWSMADelete"> </a></span></span>

<span data-ttu-id="5f747-159">Você pode excluir contatos em lotes usando o método de API gerenciada do EWS [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-159">You can delete contacts in batches by using the [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="5f747-160">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f747-160">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-contacts-in-batches-by-using-ews"></a><span data-ttu-id="5f747-161">Excluir contatos em lotes usando EWS</span><span class="sxs-lookup"><span data-stu-id="5f747-161">Delete contacts in batches by using EWS</span></span>
<span data-ttu-id="5f747-162"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-162"><a name="bk_EWSMADelete"> </a></span></span>

<span data-ttu-id="5f747-163">Você pode excluir contatos em lotes usando a operação [DeleteItem](../web-service-reference/deleteitem-operation.md) do EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f747-163">You can delete contacts in batches by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="5f747-164">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [excluir contatos em lotes](#bk_EWSMADelete).</span><span class="sxs-lookup"><span data-stu-id="5f747-164">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete contacts in batches](#bk_EWSMADelete).</span></span> <span data-ttu-id="5f747-165">O atributo **ItemId** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f747-165">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="5f747-166">O servidor responde à solicitação **DeleteItem** com uma mensagem [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para cada item que foi removido.</span><span class="sxs-lookup"><span data-stu-id="5f747-166">The server responds to the **DeleteItem** request with a [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="5f747-167">Observe que a operação também retorna êxito se a ID do item não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="5f747-167">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="5f747-168">Verificar se um processo em lote foi concluído com êxito</span><span class="sxs-lookup"><span data-stu-id="5f747-168">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="5f747-169"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="5f747-169"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="5f747-170">Quando um ou mais contatos em uma solicitação em lote não puderem ser processados como solicitados, um erro será retornado para cada contato que falhou e o restante dos contatos no lote será processado conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="5f747-170">When one or more contacts in a batched request can't be processed as requested, an error is returned for each contact that failed, and the rest of the contacts in the batch are processed as expected.</span></span> <span data-ttu-id="5f747-171">As falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser recuperado ou atualizado, ou se o item foi movido para uma pasta diferente e, portanto, tem uma nova ID de item e não pode ser modificado com a ID de item enviada.</span><span class="sxs-lookup"><span data-stu-id="5f747-171">Failures in batch processing can occur if the item was deleted, and therefore can't be retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="5f747-172">As informações desta seção mostram como obter detalhes de erro sobre falhas no processamento em lotes de contatos.</span><span class="sxs-lookup"><span data-stu-id="5f747-172">The information in this section shows how to get error details about failures in batch processing of contacts.</span></span>
  
<span data-ttu-id="5f747-173">Para verificar o sucesso de um processo em lote usando a API gerenciada do EWS, você pode verificar se a propriedade [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de [myresponsecollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) é igual a [falha. êxito](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="5f747-173">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="5f747-174">Em caso afirmativo, todos os contatos foram processados com êxito.</span><span class="sxs-lookup"><span data-stu-id="5f747-174">If so, all the contacts were processed successfully.</span></span> <span data-ttu-id="5f747-175">Se o **OverallResult** não for igual a **pararesult. Success**, um ou mais dos contatos não foram processados com êxito.</span><span class="sxs-lookup"><span data-stu-id="5f747-175">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the contacts were not processed successfully.</span></span> <span data-ttu-id="5f747-176">Cada um dos objetos retornados em **Naresponsecollection** contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="5f747-176">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="5f747-177">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="5f747-177">ErrorCode</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5f747-178">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="5f747-178">ErrorDetails</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5f747-179">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="5f747-179">ErrorMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5f747-180">Errorproperties</span><span class="sxs-lookup"><span data-stu-id="5f747-180">ErrorProperties</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5f747-181">Resultado</span><span class="sxs-lookup"><span data-stu-id="5f747-181">Result</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="5f747-182">Essas propriedades contêm informações sobre o motivo pelo qual os contatos não puderam ser processados conforme solicitado.</span><span class="sxs-lookup"><span data-stu-id="5f747-182">These properties contain information about why the contacts could not be processed as requested.</span></span> <span data-ttu-id="5f747-183">Os exemplos neste artigo imprimem o **resultado**, **ErrorCode**e **ErrorMessage** de cada contato com falha.</span><span class="sxs-lookup"><span data-stu-id="5f747-183">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed contact.</span></span> <span data-ttu-id="5f747-184">Você pode usar esses resultados para investigar o problema.</span><span class="sxs-lookup"><span data-stu-id="5f747-184">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="5f747-185">Para o EWS, para verificar o sucesso de um processo em lote, verifique o atributo [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) para cada item que está sendo processado.</span><span class="sxs-lookup"><span data-stu-id="5f747-185">For EWS, to verify the success of a batched process, check the [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="5f747-186">Veja a seguir a estrutura básica do **ResponseMessageType**, o tipo base do qual todas as mensagens de resposta são derivadas.</span><span class="sxs-lookup"><span data-stu-id="5f747-186">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="5f747-187">O atributo **ResponseClass** será definido como **Success** se o contato tiver sido processado com êxito ou um **erro** se o contato não tiver sido processado com êxito.</span><span class="sxs-lookup"><span data-stu-id="5f747-187">The **ResponseClass** attribute is set to **Success** if the contact was processed successfully, or **Error** if the contact was not processed successfully.</span></span> <span data-ttu-id="5f747-188">Para contatos, você não encontrará um **aviso** durante o processamento em lotes.</span><span class="sxs-lookup"><span data-stu-id="5f747-188">For contacts, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="5f747-189">Se o **ResponseClass** for **bem-sucedido**, o elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) que segue também é sempre definido como **NOERROR**.</span><span class="sxs-lookup"><span data-stu-id="5f747-189">If the **ResponseClass** is **Success**, the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="5f747-190">Se o **ResponseClass** for **erro**, você precisa verificar os valores dos elementos [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**e [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) para determinar o que causou o problema.</span><span class="sxs-lookup"><span data-stu-id="5f747-190">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="5f747-191">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) não está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="5f747-191">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5f747-192">Confira também</span><span class="sxs-lookup"><span data-stu-id="5f747-192">See also</span></span>


- [<span data-ttu-id="5f747-193">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5f747-193">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="5f747-194">Processar mensagens de email em lotes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5f747-194">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5f747-195">Processar itens de calendário em lotes no Exchange</span><span class="sxs-lookup"><span data-stu-id="5f747-195">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    

