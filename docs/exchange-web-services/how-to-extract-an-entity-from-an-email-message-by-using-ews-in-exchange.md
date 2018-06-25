---
title: Extrair uma entidade de uma mensagem de email usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 6396b009-5f6e-41eb-a75a-224d43e864ae
description: Saiba como extrair informações do corpo de uma mensagem de email usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: d3d5c4b756347a4cedede184709884d5ed8f08b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750717"
---
# <a name="extract-an-entity-from-an-email-message-by-using-ews-in-exchange"></a><span data-ttu-id="0cd2a-103">Extrair uma entidade de uma mensagem de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0cd2a-103">Extract an entity from an email message by using EWS in Exchange</span></span>

<span data-ttu-id="0cd2a-104">Saiba como extrair informações do corpo de uma mensagem de email usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-104">Learn how to extract information from the body of an email message by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="0cd2a-105">Você pode usar a API gerenciada de EWS ou o EWS para acessar os endereços, contatos, endereços de email, sugestões de reunião, números de telefone, tarefas e URLs que um servidor Exchange extrai mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-105">You can use the EWS Managed API or EWS to access the addresses, contacts, email addresses, meeting suggestions, phone numbers, tasks, and URLs that an Exchange server extracts from email messages.</span></span> <span data-ttu-id="0cd2a-106">Em seguida, você pode usar essas informações para novos aplicativos ou para sugerir ações em aplicativos existentes de acompanhamento.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-106">You can then use this information for new applications or to suggest follow up actions in existing applications.</span></span> <span data-ttu-id="0cd2a-107">Por exemplo, se uma entidade de visita, sugestão de reunião ou sugestão de tarefa é identificado em um email, seu aplicativo pode sugerir que um novo item com informações preenchidos ser criado.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-107">For example, if a contact entity, meeting suggestion, or task suggestion is identified in an email, your application can suggest that a new item with prepopulated information be created.</span></span> <span data-ttu-id="0cd2a-108">Usando as entidades extraídas, que possa tirar proveito a intenção atrás dos dados — e ajude os usuários perfeitamente integrar seu conteúdo da mensagem de email resultados acionáveis.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-108">By using extracted entities, you can capitalize on the intent behind the data — and help users seamlessly integrate their email message content into actionable results.</span></span>
  
<span data-ttu-id="0cd2a-109">Extração de entidade para endereços, contatos, endereços de email, sugestões de reunião, números de telefone, tarefas e URLs já está incorporada para cada item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-109">Entity extraction for addresses, contacts, email addresses, meeting suggestions, phone numbers, tasks, and URLs is already built in to every item in the Exchange store.</span></span> <span data-ttu-id="0cd2a-110">Se você estiver usando o EWS Managed API, a propriedade [Item.EntityExtractionResult](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx) recupera as entidades para você em uma chamada de método [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0cd2a-110">If you're using the EWS Managed API, the [Item.EntityExtractionResult](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx) property retrieves the entities for you in an [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method call.</span></span> <span data-ttu-id="0cd2a-111">Se você estiver usando o EWS, o elemento [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) obtém todas as entidades extraídas para você em uma chamada de operação [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0cd2a-111">If you're using EWS, the [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) element gets all the extracted entities for you in a [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="0cd2a-112">Após recuperar os resultados das entidades extraídos, você pode percorrer cada conjunto de entidade para coletar informações pertinentes.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-112">After you retrieve the results of the extracted entities, you can walk through each entity collection to gather pertinent information.</span></span> <span data-ttu-id="0cd2a-113">Por exemplo, se uma sugestão de reunião foi extraída, é possível recuperar o assunto da reunião sugerido, lista de participantes, a hora de início e hora de término.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-113">For example, if a meeting suggestion was extracted, you can retrieve the suggested meeting subject, attendee list, start time, and end time.</span></span> 
  
<span data-ttu-id="0cd2a-114">**Tabela 1. Propriedades de API gerenciada de EWS e elementos EWS que contêm as entidades extraídas**</span><span class="sxs-lookup"><span data-stu-id="0cd2a-114">**Table 1. EWS Managed API properties and EWS elements that contain extracted entities**</span></span>

|<span data-ttu-id="0cd2a-115">**Entidade extraída**</span><span class="sxs-lookup"><span data-stu-id="0cd2a-115">**Extracted entity**</span></span>|<span data-ttu-id="0cd2a-116">**Propriedade API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="0cd2a-116">**EWS Managed API property**</span></span>|<span data-ttu-id="0cd2a-117">**Elemento EWS**</span><span class="sxs-lookup"><span data-stu-id="0cd2a-117">**EWS element**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0cd2a-118">Endereços</span><span class="sxs-lookup"><span data-stu-id="0cd2a-118">Addresses</span></span>  <br/> |[<span data-ttu-id="0cd2a-119">EntityExtractionResult.Addresses</span><span class="sxs-lookup"><span data-stu-id="0cd2a-119">EntityExtractionResult.Addresses</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-120">Endereços</span><span class="sxs-lookup"><span data-stu-id="0cd2a-120">Addresses</span></span>](http://msdn.microsoft.com/library/0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0cd2a-121">Contatos</span><span class="sxs-lookup"><span data-stu-id="0cd2a-121">Contacts</span></span>  <br/> |[<span data-ttu-id="0cd2a-122">EntityExtractionResult.Contacts</span><span class="sxs-lookup"><span data-stu-id="0cd2a-122">EntityExtractionResult.Contacts</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.contacts%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-123">Contatos</span><span class="sxs-lookup"><span data-stu-id="0cd2a-123">Contacts</span></span>](http://msdn.microsoft.com/library/a2c1e833-5f8c-438d-bad7-bb5dcc29ca9e%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0cd2a-124">Emails</span><span class="sxs-lookup"><span data-stu-id="0cd2a-124">Email addresses</span></span>  <br/> |[<span data-ttu-id="0cd2a-125">EntityExtractionResult.EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0cd2a-125">EntityExtractionResult.EmailAddresses</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.emailaddresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-126">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0cd2a-126">EmailAddresses</span></span>](http://msdn.microsoft.com/library/2fc4a8e8-5377-4059-8fb4-3fdabfd30fe3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0cd2a-127">Sugestões de reunião</span><span class="sxs-lookup"><span data-stu-id="0cd2a-127">Meeting suggestions</span></span>  <br/> |[<span data-ttu-id="0cd2a-128">EntityExtractionResult.MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="0cd2a-128">EntityExtractionResult.MeetingSuggestions</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.meetingsuggestions%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-129">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="0cd2a-129">MeetingSuggestions</span></span>](http://msdn.microsoft.com/library/c99e9a60-9e38-425d-ad03-47c8917f41da%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0cd2a-130">Números de telefone</span><span class="sxs-lookup"><span data-stu-id="0cd2a-130">Phone numbers</span></span>  <br/> |[<span data-ttu-id="0cd2a-131">EntityExtractionResult.PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="0cd2a-131">EntityExtractionResult.PhoneNumbers</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.phonenumbers%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-132">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="0cd2a-132">PhoneNumbers</span></span>](http://msdn.microsoft.com/library/9ff6ae98-34a1-47f7-bde5-608251a789f7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0cd2a-133">Sugestões de tarefa</span><span class="sxs-lookup"><span data-stu-id="0cd2a-133">Task suggestions</span></span>  <br/> |[<span data-ttu-id="0cd2a-134">EntityExtractionResult.TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="0cd2a-134">EntityExtractionResult.TaskSuggestions</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-135">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="0cd2a-135">TaskSuggestions</span></span>](http://msdn.microsoft.com/library/7d3c6314-2a5c-4fc3-b5f9-ae6d4946aac3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="0cd2a-136">URLs</span><span class="sxs-lookup"><span data-stu-id="0cd2a-136">URLs</span></span>  <br/> |[<span data-ttu-id="0cd2a-137">EntityExtractionResult.Urls</span><span class="sxs-lookup"><span data-stu-id="0cd2a-137">EntityExtractionResult.Urls</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0cd2a-138">URLs</span><span class="sxs-lookup"><span data-stu-id="0cd2a-138">Urls</span></span>](http://msdn.microsoft.com/library/c39744ea-0cee-4954-8653-8279d6b10161%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="0cd2a-139">Como extração de entidade depende de reconhecimento de linguagem natural, o reconhecimento das entidades que pode ser não determinantes e sucesso depende em alguns casos, o contexto.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-139">Because entity extraction relies on natural language recognition, the recognition of entities can be non-deterministic and success sometimes relies on the context.</span></span> <span data-ttu-id="0cd2a-140">Para demonstrar como funciona o reconhecimento de linguagem natural, os exemplos neste artigo usam o email a seguir como entrada.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-140">To demonstrate how natural language recognition works, the examples in this article use the following email as input.</span></span>
  
 `From: Ronnie Sturgis`
  
 `To: Sadie Daniels`
  
 `Subject: Dinner party`
  
 `Hi Sadie`
  
 `Are you free this Friday at 7 to join us for a dinner party at our house?`
  
 `We're at 789 International Blvd, St Paul MN 55104.`
  
 `Our number is 612-555-0158 if you have trouble finding it.`
  
 `Please RSVP to either myself or Mara (mara@contoso.com) before Friday morning. Best for you organics (http://www.bestforyouorganics.com) will be catering so we can fully enjoy ourselves!`
  
 `Also, can you forward this to Magdalena? I don't have her contact information.`
  
 `See you then!`
  
 `Ronnie`
  
## <a name="extract-all-entities-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="0cd2a-141">Extrair todas as entidades de um email usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="0cd2a-141">Extract all entities from an email by using the EWS Managed API</span></span>
<span data-ttu-id="0cd2a-142"><a name="bk_extractewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="0cd2a-142"></span></span>

<span data-ttu-id="0cd2a-143">O exemplo de código a seguir mostra como exibir todas as entidades extraídas pelo servidor, usando o método [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) e, em seguida, enumerando através de cada uma das entidades extraídas e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-143">The following code example shows how to display all the entities extracted by the server, by using the [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method, and then enumerating through each of the extracted entities and their properties.</span></span> 
  
<span data-ttu-id="0cd2a-144">Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , e esse **ItemId** é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email para mover ou copiar.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-144">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
```cs
public static void ExtractEntities(ExchangeService service, ItemId ItemId)
{
    // Create a property set that limits the properties returned 
    // by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.EntityExtractionResult);
    // Get the item from the server.
    // This method call results in an GetItem call to EWS.
    Item item = Item.Bind(service, ItemId, propSet);
    Console.WriteLine("The following entities have been extracted from the message:");
    Console.WriteLine(" ");
    // If address entities are extracted from the message, print the results.
    if (item.EntityExtractionResult != null)
    {
        if (item.EntityExtractionResult.Addresses != null)
        {
            Console.WriteLine("--------------------Addresses---------------------------");
            foreach (AddressEntity address in item.EntityExtractionResult.Addresses)
            {
                Console.WriteLine("Address: {0}", address.Address);
            }
            Console.WriteLine(" ");
        }
        // If contact entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.Contacts != null)
        {
            Console.WriteLine("--------------------Contacts----------------------------");
            foreach (ContactEntity contact in item.EntityExtractionResult.Contacts)
            {
                Console.WriteLine("Addresses:       {0}", contact.Addresses);
                Console.WriteLine("Business name:   {0}", contact.BusinessName);
                Console.WriteLine("Contact string:  {0}", contact.ContactString);
                Console.WriteLine("Email addresses: {0}", contact.EmailAddresses);
                Console.WriteLine("Person name:     {0}", contact.PersonName);
                Console.WriteLine("Phone numbers:   {0}", contact.PhoneNumbers);
                Console.WriteLine("URLs:            {0}", contact.Urls);
            }
            Console.WriteLine(" ");
        }
        // If email address entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.EmailAddresses != null)
        {
            Console.WriteLine("--------------------Email addresses---------------------");
            foreach (EmailAddressEntity email in item.EntityExtractionResult.EmailAddresses)
            {
                Console.WriteLine("Email addresses: {0}", email.EmailAddress);
            }
            Console.WriteLine(" ");
        }
        // If meeting suggestion entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.MeetingSuggestions != null)
        {
            Console.WriteLine("--------------------Meeting suggestions-----------------");
            foreach (MeetingSuggestion meetingSuggestion in item.EntityExtractionResult.MeetingSuggestions)
            {
                Console.WriteLine("Meeting subject:  {0}", meetingSuggestion.Subject);
                Console.WriteLine("Meeting string:   {0}", meetingSuggestion.MeetingString);
                foreach (EmailUserEntity attendee in meetingSuggestion.Attendees)
                {
                    Console.WriteLine("Attendee name:    {0}", attendee.Name);
                    Console.WriteLine("Attendee user ID: {0}", attendee.UserId);
                }
                Console.WriteLine("Start time:       {0}", meetingSuggestion.StartTime);
                Console.WriteLine("End time:         {0}", meetingSuggestion.EndTime);
                Console.WriteLine("Location:         {0}", meetingSuggestion.Location);
            }
            Console.WriteLine(" ");
        }
        // If phone number entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.PhoneNumbers != null)
        {
            Console.WriteLine("--------------------Phone numbers-----------------------");
            foreach (PhoneEntity phone in item.EntityExtractionResult.PhoneNumbers)
            {
                Console.WriteLine("Original phone string:  {0}", phone.OriginalPhoneString);
                Console.WriteLine("Phone string:           {0}", phone.PhoneString);
                Console.WriteLine("Type:                   {0}", phone.Type);
            }
            Console.WriteLine(" ");
        }
        // If task suggestion entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.TaskSuggestions != null)
        {
            Console.WriteLine("--------------------Task suggestions--------------------");
            foreach (TaskSuggestion task in item.EntityExtractionResult.TaskSuggestions)
            {
                foreach (EmailUserEntity assignee in task.Assignees)
                {
                    Console.WriteLine("Assignee name:    {0}", assignee.Name);
                    Console.WriteLine("Assignee user ID: {0}", assignee.UserId);
                }
                Console.WriteLine("Task string:      {0}", task.TaskString);
            }
            Console.WriteLine(" ");
        }
        // If URL entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.Urls != null)
        {
            Console.WriteLine("--------------------URLs--------------------------------");
            foreach (UrlEntity url in item.EntityExtractionResult.Urls)
            {
                Console.WriteLine("URL: {0}", url.Url);
            }
            Console.WriteLine(" ");
        }
    }
    // If no entities are extracted from the message, print the result.
    else if (item.EntityExtractionResult == null)
    {
        Console.WriteLine("No entities extracted");
    }
}
```

<span data-ttu-id="0cd2a-145">A seguinte saída é exibida no console.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-145">The following output is displayed on the console.</span></span>
  
```text
The following entities have been extracted from the message:
 
--------------------Addresses---------------------------
Address: 789 International Blvd, St Paul MN 55104
 
--------------------Contacts----------------------------
Addresses:       
Business name:   
Contact string:  Mara (mara@contoso.com)
Email addresses: mara@contoso.com
Person name:     Mara
Phone numbers:   
URLs:            
 
--------------------Email addresses---------------------
Email addresses: mara@contoso.com
 
--------------------Meeting suggestions-----------------
Meeting subject:  dinner party
Meeting string:   Are you free this Friday at 7 to join us for a dinner party at our house?
Attendee name:    Ronnie Sturgis
Attendee user ID: ronnie@contoso.com
Attendee name:    Sadie Daniels
Attendee user ID: sadie@cntoso.com
Start time:       10/1/0104 2:00:00 PM
End time:         10/1/0104 2:30:00 PM
Location:         
 
--------------------Phone numbers-----------------------
Original phone string:  612-555-0158
Phone string:           6125550158
Type:                   Unspecified
 
--------------------Task suggestions--------------------
Assignee name:    Sadie Daniels
Assignee user ID: sadie@contoso.com
Task string:      Also, can you forward this to Magdalena?
 
--------------------URLs--------------------------------
URL: http://www.bestforyouorganics.com
```

<span data-ttu-id="0cd2a-146">Observe que todos os endereços, contatos, endereços de email, números de telefone, tarefas e URLs foram extraídos conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-146">Notice that all addresses, contacts, email addresses, phone numbers, tasks, and URLs were extracted as expected.</span></span> <span data-ttu-id="0cd2a-147">A sugestão de reunião, no entanto, é um pouco mais complexa.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-147">The meeting suggestion, however, is a bit more complex.</span></span> <span data-ttu-id="0cd2a-148">Observe a hora de início e a hora de término da sugestão de reunião são não o que você pode esperar.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-148">Notice the start time and end time of the meeting suggestion are not what you might expect.</span></span> <span data-ttu-id="0cd2a-149">A hora de início no email é "Este sexta-feira em 7", mas o valor extraído para a hora de início é 10/1/0104 2:00:00 PM.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-149">The start time in the email is "this Friday at 7", but the extracted value for the start time is 10/1/0104 2:00:00 PM.</span></span> <span data-ttu-id="0cd2a-150">Isso ocorre porque a hora de início e a hora de término extraídas pelo servidor são datas codificadas.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-150">This is because the start time and end time extracted by the server are encoded dates.</span></span> <span data-ttu-id="0cd2a-151">Para obter mais informações sobre como interpretar os valores de **data/hora** em sugestões de reunião, consulte [[MS-OXCEXT]: protocolo de objeto de mensagem de extensão de cliente](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0cd2a-151">For more information about how to interpret **dateTime** values in meeting suggestions, see [[MS-OXCEXT]: Client Extension Message Object Protocol](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).</span></span>
  
## <a name="extract-all-entities-from-an-email-by-using-ews"></a><span data-ttu-id="0cd2a-152">Extrair todas as entidades de um email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="0cd2a-152">Extract all entities from an email by using EWS</span></span>
<span data-ttu-id="0cd2a-153"><a name="bk_extractews"> </a></span><span class="sxs-lookup"><span data-stu-id="0cd2a-153"></span></span>

<span data-ttu-id="0cd2a-154">O exemplo de código a seguir mostra como usar a operação [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) e o elemento [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) para recuperar as entidades extraídas de um item.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-154">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation and the [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) element to retrieve the extracted entities from an item.</span></span> 
  
<span data-ttu-id="0cd2a-155">Isso também é a solicitação XML que é enviada pela API gerenciada de EWS quando você usa o método **ligar** para [extrair todas as entidades a partir de um email usando a API gerenciada de EWS](#bk_extractewsma).</span><span class="sxs-lookup"><span data-stu-id="0cd2a-155">This is also the XML request that is sent by the EWS Managed API when you use the **Bind** method to [Extract all entities from an email by using the EWS Managed API](#bk_extractewsma).</span></span>
  
<span data-ttu-id="0cd2a-156">O valor do elemento [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-156">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element is shortened for readability.</span></span> 
  
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
          <t:FieldURI FieldURI="item:EntityExtractionResult" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="sVC5AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a mensagem de email foi recuperada com êxito. <span data-ttu-id="0cd2a-158">A resposta também inclui o **EntityExtractionResult** para cada entidade extraída.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-158">The response also includes the **EntityExtractionResult** for each extracted entity.</span></span> 
  
<span data-ttu-id="0cd2a-159">O valor do elemento **ItemId** é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-159">The value of the **ItemId** element is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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
              <t:ItemId Id="sVC5AAA="
                        ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAOOqJN" />
              <t:EntityExtractionResult>
                <t:Addresses>
                  <t:AddressEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:Address>789 International Blvd, St Paul MN 55104</t:Address>
                  </t:AddressEntity>
                </t:Addresses>
                <t:MeetingSuggestions>
                  <t:MeetingSuggestion>
                    <t:Position>LatestReply</t:Position>
                    <t:Attendees>
                      <t:EmailUser>
                        <t:Name>Ronnie Sturgis</t:Name>
                        <t:UserId>ronnie@contoso.com</t:UserId>
                      </t:EmailUser>
                      <t:EmailUser>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:UserId>sadie@contoso.com</t:UserId>
                      </t:EmailUser>
                    </t:Attendees>
                    <t:Subject>dinner party</t:Subject>
                    <t:MeetingString>Are you free this Friday at 7 to join us for a dinner party at our house?</t:MeetingString>
                    <t:StartTime>0104-10-01T19:00:00Z</t:StartTime>
                    <t:EndTime>0104-10-01T19:30:00Z</t:EndTime>
                  </t:MeetingSuggestion>
                </t:MeetingSuggestions>
                <t:TaskSuggestions>
                  <t:TaskSuggestion>
                    <t:Position>LatestReply</t:Position>
                    <t:TaskString>Also, can you forward this to Magdalena?</t:TaskString>
                    <t:Assignees>
                      <t:EmailUser>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:UserId>sadie@contoso.com</t:UserId>
                      </t:EmailUser>
                    </t:Assignees>
                  </t:TaskSuggestion>
                </t:TaskSuggestions>
                <t:EmailAddresses>
                  <t:EmailAddressEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:EmailAddress>mara@contoso.com</t:EmailAddress>
                  </t:EmailAddressEntity>
                </t:EmailAddresses>
                <t:Contacts>
                  <t:Contact>
                    <t:Position>LatestReply</t:Position>
                    <t:PersonName>Mara</t:PersonName>
                    <t:EmailAddresses>
                      <t:EmailAddress>mara@contoso.com</t:EmailAddress>
                    </t:EmailAddresses>
                    <t:ContactString>Mara (mara@contoso.com</t:ContactString>
                  </t:Contact>
                </t:Contacts>
                <t:Urls>
                  <t:UrlEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:Url>http://www.bestforyouorganics.com</t:Url>
                  </t:UrlEntity>
                </t:Urls>
                <t:PhoneNumbers>
                  <t:Phone>
                    <t:Position>LatestReply</t:Position>
                    <t:OriginalPhoneString>612-555-0158</t:OriginalPhoneString>
                    <t:PhoneString>6125550158</t:PhoneString>
                    <t:Type>Unspecified</t:Type>
                  </t:Phone>
                </t:PhoneNumbers>
              </t:EntityExtractionResult>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0cd2a-160">Observe que todos os endereços, contatos, endereços de email, números de telefone, tarefas e URLs foram extraídos conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-160">Notice that all addresses, contacts, email addresses, phone numbers, tasks, and URLs were extracted as expected.</span></span> <span data-ttu-id="0cd2a-161">A sugestão de reunião, no entanto, é um pouco mais complexa.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-161">The meeting suggestion, however, is a bit more complex.</span></span> <span data-ttu-id="0cd2a-162">Observe a hora de início e a hora de término da sugestão de reunião são não o que você pode esperar.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-162">Notice the start time and end time of the meeting suggestion are not what you might expect.</span></span> <span data-ttu-id="0cd2a-163">A hora de início do e-mail foi "Este sextas-feiras às 7", mas o valor extraído para a hora de início é 10/1/0104 2:00:00 PM.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-163">The start time in the email was "this Friday at 7", but the extracted value for the start time is 10/1/0104 2:00:00 PM.</span></span> <span data-ttu-id="0cd2a-164">Isso ocorre porque a hora de início e a hora de término extraídas pelo servidor são datas codificadas.</span><span class="sxs-lookup"><span data-stu-id="0cd2a-164">This is because the start time and end time extracted by the server are encoded dates.</span></span> <span data-ttu-id="0cd2a-165">Para obter mais informações sobre como interpretar os valores de **data/hora** em sugestões de reunião, consulte [[MS-OXCEXT]: protocolo de objeto de mensagem de extensão de cliente](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0cd2a-165">For more information about interpreting **dateTime** values in meeting suggestions, see [[MS-OXCEXT]: Client Extension Message Object Protocol](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0cd2a-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="0cd2a-166">See also</span></span>

- [<span data-ttu-id="0cd2a-167">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0cd2a-167">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="0cd2a-168">Item.EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="0cd2a-168">Item.EntityExtractionResult</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="0cd2a-169">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="0cd2a-169">EntityExtractionResult</span></span>](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx)
    

