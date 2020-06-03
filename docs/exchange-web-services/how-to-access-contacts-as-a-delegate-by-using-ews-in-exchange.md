---
title: Acessar contatos como um representante usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Saiba como acessar contatos como um representante usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 06faf7dd7459b14792abbea21761e909c8eb9fb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455342"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="fa6d1-103">Acessar contatos como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa6d1-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="fa6d1-104">Saiba como acessar contatos como um representante usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="fa6d1-105">Você pode usar a API gerenciada do EWS ou o EWS para conceder a um usuário acesso a uma pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-105">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder.</span></span> <span data-ttu-id="fa6d1-106">O representante pode então criar contatos em nome do proprietário da caixa de correio e recuperar, atualizar e excluir contatos da pasta de contatos do proprietário da caixa de correio, dependendo de suas permissões.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-106">The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="fa6d1-107">Como representante, você usa os mesmos métodos e operações para acessar a pasta de contatos do proprietário da caixa de correio que você usa para acessar sua própria pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-107">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder.</span></span> <span data-ttu-id="fa6d1-108">A principal diferença é que você precisa usar o [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de contato e depois depois de identificar a ID do item, você pode usar o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="fa6d1-109">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para acessar um contato como um representante**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="fa6d1-110">**Se você quiser...**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-110">**If you want to…**</span></span>|<span data-ttu-id="fa6d1-111">**Use este método de API gerenciada do EWS...**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="fa6d1-112">**Use esta operação do EWS...**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fa6d1-113">Criar um contato como representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="fa6d1-114">[Item. Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-114">[Item.Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="fa6d1-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="fa6d1-116">Criar vários contatos como um representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="fa6d1-117">[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="fa6d1-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="fa6d1-119">Resolver um contato como representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="fa6d1-120">[ExchangeService. ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-120">[ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="fa6d1-121">[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-121">[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="fa6d1-122">Procurar ou localizar um contato como representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="fa6d1-123">[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-123">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="fa6d1-124">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) especifica o [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="fa6d1-124">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="fa6d1-125">Obter um contato como representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="fa6d1-126">Contato. bind</span><span class="sxs-lookup"><span data-stu-id="fa6d1-126">Contact.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fa6d1-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="fa6d1-127">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="fa6d1-128">Atualizar um contato como representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="fa6d1-129">[Contato. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) seguido por [Contact. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-129">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="fa6d1-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="fa6d1-131">Excluir um contato como representante</span><span class="sxs-lookup"><span data-stu-id="fa6d1-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="fa6d1-132">[Contato. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) seguido por [Contact. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-132">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="fa6d1-133">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-133">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="fa6d1-134">Nos exemplos de código deste artigo, primary@contoso.com é o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="fa6d1-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-135"><a name="bk_prereq"> </a></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="fa6d1-136">Tarefas de pré-requisito</span><span class="sxs-lookup"><span data-stu-id="fa6d1-136">Prerequisite tasks</span></span>

<span data-ttu-id="fa6d1-137">Antes que um usuário possa acessar a pasta de contatos do proprietário da caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para a pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="fa6d1-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-138"><a name="bk_createewsma"> </a></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="fa6d1-139">Criar um contato como um representante usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="fa6d1-140">A API gerenciada do EWS permite que você use o objeto de serviço para que o usuário delegado crie contatos para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="fa6d1-141">Este exemplo mostra como usar o método [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-141">This example shows how to use the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="fa6d1-142">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e que o representante recebeu as permissões apropriadas para a pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-142">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="fa6d1-143">Observe que, quando você salva o item, a chamada do método [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) deve identificar a pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-143">Note that when you save the item, the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="fa6d1-144">Se a pasta de contatos do proprietário da caixa de correio não for especificada, a solicitação de reunião será salva na pasta contatos do representante e não na pasta contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="fa6d1-145">Você pode incluir a pasta de contatos do proprietário da caixa de correio na chamada do método **Save** de duas vias.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="fa6d1-146">Recomendamos que você instancie uma nova instância do objeto [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) usando o [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-146">We recommend that you instantiate a new instance of the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="fa6d1-147">No entanto, você também pode [vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) a pasta contatos primeiro e, em seguida, usar a ID da pasta na chamada do método **Save** .</span><span class="sxs-lookup"><span data-stu-id="fa6d1-147">However, you can also [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="fa6d1-148">No entanto, lembre-se de que isso cria uma chamada EWS extra.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="fa6d1-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-149"><a name="bk_createews"> </a></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="fa6d1-150">Criar um contato como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="fa6d1-151">O EWS permite que você use o objeto de serviço para que o usuário delegado crie itens de contato para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-151">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner.</span></span> <span data-ttu-id="fa6d1-152">Este exemplo mostra como usar a operação [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar um contato.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-152">This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="fa6d1-153">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **Save** para [criar um contato](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="fa6d1-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
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

<span data-ttu-id="fa6d1-154">O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o contato foi criado com êxito.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-154">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully.</span></span> <span data-ttu-id="fa6d1-155">A resposta também contém a ID do item do contato recém-criado.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-155">The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="fa6d1-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-156"><a name="bk_resolveewsma"> </a></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="fa6d1-157">Resolver um contato como um representante usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="fa6d1-158">Para localizar um contato com base em um nome ou termo possivelmente ambíguo, você deve usar um dos métodos [ExchangeService. ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você possa especificar a pasta contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="fa6d1-159">Após a chamada do método **ResolveNames** retornar uma resposta com uma ID, você pode [obter, atualizar ou excluir o contato](#bk_getewsma) usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) &mdash; e não precisa especificar o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="fa6d1-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-160"><a name="bk_resolveews"> </a></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="fa6d1-161">Resolver um contato como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="fa6d1-162">O EWS permite que você use o objeto de serviço do usuário delegado para resolver nomes parciais na pasta contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-162">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="fa6d1-163">Este exemplo mostra como usar a operação [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) para localizar reuniões na pasta de contatos do proprietário da caixa de correio que contêm a palavra "Johnson".</span><span class="sxs-lookup"><span data-stu-id="fa6d1-163">This example shows how to use the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="fa6d1-164">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **ResolveName** para [resolver um contato](#bk_resolveewsma).</span><span class="sxs-lookup"><span data-stu-id="fa6d1-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fa6d1-165">O servidor responde à solicitação **ResolveNames** com uma mensagem [ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a operação foi concluída com êxito e que encontrou apenas um resultado, ou **ErrorNameResolutionMultipleResults** se vários resultados forem encontrados, o que é mostrado no terceiro exemplo de código com base no contato [criar um contato como um representante usando a API gerenciada do EWS](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="fa6d1-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="fa6d1-166">A resposta também contém o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de cada resultado.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-166">The response also contains the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="fa6d1-167">O valor do elemento **ItemId** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
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
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="fa6d1-168">Agora que você tem o **ItemId** para os contatos que correspondam ao nome ambíguo, é possível [obter, atualizar ou excluir itens de contato como um representante usando o EWS](#bk_getews) usando o **ItemId** e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) &mdash; e não é necessário especificar o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="fa6d1-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-169"><a name="bk_getewsma"> </a></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="fa6d1-170">Obter, atualizar ou excluir itens de contato como um representante usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="fa6d1-171">Você pode usar a API gerenciada do EWS para obter, atualizar ou excluir um contato da mesma maneira que executará essas ações quando não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-171">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="fa6d1-172">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-172">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="fa6d1-173">A ID do item incluída na chamada do método **BIND** identifica exclusivamente o item no repositório de caixa de correio, na pasta contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-173">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="fa6d1-174">**Tabela 2. Métodos da API gerenciada do EWS trabalhando com um contato como um representante**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="fa6d1-175">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-175">**Task**</span></span>|<span data-ttu-id="fa6d1-176">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-176">**EWS Managed API method**</span></span>|<span data-ttu-id="fa6d1-177">**Exemplo de código**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fa6d1-178">Obter um contato</span><span class="sxs-lookup"><span data-stu-id="fa6d1-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="fa6d1-179">Associá</span><span class="sxs-lookup"><span data-stu-id="fa6d1-179">Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fa6d1-180">Obter um item usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="fa6d1-181">Atualizar um contato</span><span class="sxs-lookup"><span data-stu-id="fa6d1-181">Update a contact</span></span>  <br/> |<span data-ttu-id="fa6d1-182">[Vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido por [atualização](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-182">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="fa6d1-183">Atualizar um item usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="fa6d1-184">Excluir um contato</span><span class="sxs-lookup"><span data-stu-id="fa6d1-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="fa6d1-185">[Vincular](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido por [delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-185">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="fa6d1-186">Excluir um item usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="fa6d1-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="fa6d1-187"><a name="bk_getews"> </a></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="fa6d1-188">Obter, atualizar ou excluir itens de contato como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="fa6d1-189">Você pode usar o EWS para obter, atualizar ou excluir um contato de reunião ou compromisso da mesma maneira que você executa essas ações quando não está usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-189">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="fa6d1-190">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-190">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="fa6d1-191">A ID do item incluída na solicitação [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) identifica exclusivamente o item no repositório de caixa de correio, na pasta contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fa6d1-191">The item ID included in the [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="fa6d1-192">**Tabela 3. Operações do EWS para trabalhar com um contato como representante**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="fa6d1-193">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-193">**Task**</span></span>|<span data-ttu-id="fa6d1-194">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-194">**EWS operation**</span></span>|<span data-ttu-id="fa6d1-195">**Amostra**</span><span class="sxs-lookup"><span data-stu-id="fa6d1-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fa6d1-196">Obter um contato</span><span class="sxs-lookup"><span data-stu-id="fa6d1-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="fa6d1-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="fa6d1-197">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="fa6d1-198">Obter um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="fa6d1-199">Atualizar um contato</span><span class="sxs-lookup"><span data-stu-id="fa6d1-199">Update a contact</span></span>  <br/> |<span data-ttu-id="fa6d1-200">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-200">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="fa6d1-201">Atualizar um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="fa6d1-202">Excluir um contato</span><span class="sxs-lookup"><span data-stu-id="fa6d1-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="fa6d1-203">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido por [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="fa6d1-203">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="fa6d1-204">Excluir um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fa6d1-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa6d1-205">Confira também</span><span class="sxs-lookup"><span data-stu-id="fa6d1-205">See also</span></span>

- [<span data-ttu-id="fa6d1-206">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa6d1-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="fa6d1-207">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa6d1-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="fa6d1-208">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa6d1-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="fa6d1-209">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa6d1-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="fa6d1-210">Resolver nomes ambíguos usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fa6d1-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

