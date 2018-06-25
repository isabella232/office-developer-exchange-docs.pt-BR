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
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="6c67a-103">Contatos de acesso como um representante, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6c67a-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="6c67a-104">Saiba como acessar contatos como um representante, usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c67a-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="6c67a-105">Você pode usar a API gerenciada de EWS ou EWS dar um usuário acesso à pasta de contatos de um proprietário caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-105">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder.</span></span> <span data-ttu-id="6c67a-106">O representante, em seguida, pode criar contatos em nome do proprietário da caixa de correio e recuperar, atualizar e excluir os contatos da pasta de contatos do proprietário da caixa de correio, dependendo de suas permissões.</span><span class="sxs-lookup"><span data-stu-id="6c67a-106">The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="6c67a-107">Como um representante, use os métodos e as mesmas operações para acessar a pasta de contatos de um proprietário caixa de correio que você usa para acessar sua própria pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="6c67a-107">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder.</span></span> <span data-ttu-id="6c67a-108">A principal diferença é que você precisa usar [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de contato e, em seguida, depois de identificar a ID do item, você pode usar [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item.</span><span class="sxs-lookup"><span data-stu-id="6c67a-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="6c67a-109">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para acessar um contato como um representante**</span><span class="sxs-lookup"><span data-stu-id="6c67a-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="6c67a-110">**Se você quiser …**</span><span class="sxs-lookup"><span data-stu-id="6c67a-110">**If you want to…**</span></span>|<span data-ttu-id="6c67a-111">**Use este método de API gerenciada de EWS …**</span><span class="sxs-lookup"><span data-stu-id="6c67a-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="6c67a-112">**Use essa operação EWS …**</span><span class="sxs-lookup"><span data-stu-id="6c67a-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6c67a-113">Criar um contato como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="6c67a-114">[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-114">[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="6c67a-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="6c67a-116">Criar vários contatos como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="6c67a-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="6c67a-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="6c67a-119">Resolver um contato como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="6c67a-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="6c67a-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="6c67a-122">Pesquise ou localizar um contato como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="6c67a-123">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) à pasta de contatos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-123">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="6c67a-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6c67a-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="6c67a-125">Obtenha um contato como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="6c67a-126">Contact.Bind</span><span class="sxs-lookup"><span data-stu-id="6c67a-126">Contact.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="6c67a-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="6c67a-127">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="6c67a-128">Atualizar um contato como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="6c67a-129">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) seguido [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-129">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="6c67a-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="6c67a-131">Excluir um contato como um representante</span><span class="sxs-lookup"><span data-stu-id="6c67a-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="6c67a-132">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) seguido [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-132">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="6c67a-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="6c67a-134">Os exemplos de código neste artigo, primary@contoso.com é o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="6c67a-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-135"></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="6c67a-136">Tarefas de pré-requisito</span><span class="sxs-lookup"><span data-stu-id="6c67a-136">Prerequisite tasks</span></span>

<span data-ttu-id="6c67a-137">Antes de um usuário pode acessar a pasta de contatos do proprietário da caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) à pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="6c67a-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-138"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="6c67a-139">Criar um contato como um representante, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="6c67a-140">A API gerenciada de EWS permite que você use o objeto de serviço para o usuário delegado para criar contatos para o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="6c67a-141">Este exemplo mostra como usar o método [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) para criar uma reunião e enviar solicitações de reunião para os participantes.</span><span class="sxs-lookup"><span data-stu-id="6c67a-141">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="6c67a-142">Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e o delegado recebeu as permissões apropriadas para a pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="6c67a-143">Observe que, quando você salva o item, a chamada do método [Salvar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) deve identificar pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="6c67a-144">Se a pasta de contatos do proprietário da caixa de correio não for especificada, a solicitação de reunião obtém salvos não pasta de contatos do proprietário da caixa de correio e de pasta de contatos do representante.</span><span class="sxs-lookup"><span data-stu-id="6c67a-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="6c67a-145">Você pode incluir uma pasta de contatos do proprietário da caixa de correio na chamada do método **Salvar** na forma dois.</span><span class="sxs-lookup"><span data-stu-id="6c67a-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="6c67a-146">Recomendamos que você criar uma nova instância do objeto [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) usando o [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e o endereço SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="6c67a-147">No entanto, você também pode [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para a pasta Contatos em primeiro lugar e, em seguida, usar a identificação da pasta na chamada do método **Salvar** .</span><span class="sxs-lookup"><span data-stu-id="6c67a-147">However, you can also [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="6c67a-148">Lembre-se, no entanto, se esse cria uma chamada de EWS extra.</span><span class="sxs-lookup"><span data-stu-id="6c67a-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="6c67a-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-149"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="6c67a-150">Criar um contato como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="6c67a-151">EWS permite que você use o objeto de serviço para o usuário delegado para criar itens de contato do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-151">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner.</span></span> <span data-ttu-id="6c67a-152">Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar um contato.</span><span class="sxs-lookup"><span data-stu-id="6c67a-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="6c67a-153">Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **Save** para [criar um contato](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="6c67a-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
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

<span data-ttu-id="6c67a-154">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se o contato foi criado com êxito.</span><span class="sxs-lookup"><span data-stu-id="6c67a-154">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully.</span></span> <span data-ttu-id="6c67a-155">A resposta também contém a ID de item do contato recém-criado.</span><span class="sxs-lookup"><span data-stu-id="6c67a-155">The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="6c67a-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-156"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="6c67a-157">Resolver um contato como um representante, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="6c67a-158">Para localizar um contato, com base em um nome ambíguo possivelmente ou termo, você deve usar um dos métodos [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você pode especificar uma pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="6c67a-159">Depois que a chamada do método **ResolveNames** retornará uma resposta com uma ID, você pode [obter, atualizar ou excluir o contato](#bk_getewsma) usando a ID e o [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="6c67a-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-160"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="6c67a-161">Resolver um contato como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="6c67a-162">EWS permite que você use o objeto de serviço para o usuário delegado para resolver nomes de parciais na pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-162">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="6c67a-163">Este exemplo mostra como usar a operação [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) para localizar reuniões na pasta de contatos do proprietário da caixa de correio que contêm a palavra "johnson".</span><span class="sxs-lookup"><span data-stu-id="6c67a-163">This example shows how to use the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="6c67a-164">Isso também é a solicitação XML que o EWS Managed API envia quando você usa o método **ResolveName** resolver [um contato](#bk_resolveewsma).</span><span class="sxs-lookup"><span data-stu-id="6c67a-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
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

<span data-ttu-id="6c67a-165">O servidor responde à solicitação **ResolveNames** com uma mensagem de [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a operação concluída com êxito e encontrados apenas um resultado ou **ErrorNameResolutionMultipleResults** se vários resultados encontrados - que é o que é mostrado no exemplo de código de terceiro com base no contato [criar um contato como um representante usando a API gerenciada de EWS](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="6c67a-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="6c67a-166">A resposta também contém o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de cada resultado.</span><span class="sxs-lookup"><span data-stu-id="6c67a-166">The response also contains the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="6c67a-167">O valor do elemento **ItemId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6c67a-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="6c67a-168">Agora que você tem o **ItemId** para os contatos que correspondam ao nome ambíguo, você pode [obter, atualizar ou excluir itens de contato como um representante, usando o EWS](#bk_getews) by using the **ItemId** e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;e você não precisará especificar endereço de SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="6c67a-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-169"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="6c67a-170">Obter, atualizar ou excluir itens de contato como um representante, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="6c67a-171">Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir um contato da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="6c67a-171">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="6c67a-172">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="6c67a-172">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="6c67a-173">A ID do item incluída na chamada do método **vincular** exclusivamente identifica o item no repositório de caixa de correio, na pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-173">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="6c67a-174">**Tabela 2. Trabalhando com um contato como um representante de métodos de API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="6c67a-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="6c67a-175">**Task**</span><span class="sxs-lookup"><span data-stu-id="6c67a-175">**Task**</span></span>|<span data-ttu-id="6c67a-176">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="6c67a-176">**EWS Managed API method**</span></span>|<span data-ttu-id="6c67a-177">**Exemplo de código**</span><span class="sxs-lookup"><span data-stu-id="6c67a-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6c67a-178">Obtenha um contato</span><span class="sxs-lookup"><span data-stu-id="6c67a-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="6c67a-179">Vincular</span><span class="sxs-lookup"><span data-stu-id="6c67a-179">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="6c67a-180">Obter um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="6c67a-181">Atualização de um contato</span><span class="sxs-lookup"><span data-stu-id="6c67a-181">Update a contact</span></span>  <br/> |<span data-ttu-id="6c67a-182">[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido de [atualização](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-182">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="6c67a-183">Atualização de um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="6c67a-184">Excluir um contato</span><span class="sxs-lookup"><span data-stu-id="6c67a-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="6c67a-185">[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) seguido [Excluir](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-185">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="6c67a-186">Excluir um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="6c67a-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="6c67a-187"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="6c67a-188">Obter, atualizar ou excluir itens de contato como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="6c67a-189">Você pode usar o EWS para obter, atualizar ou excluir um contato de reunião ou compromisso da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="6c67a-189">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="6c67a-190">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="6c67a-190">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="6c67a-191">A ID do item incluída na solicitação [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) exclusivamente identifica o item no repositório de caixa de correio, na pasta de contatos do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6c67a-191">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="6c67a-192">**Tabela 3. Operações do EWS para trabalhar com um contato como um representante**</span><span class="sxs-lookup"><span data-stu-id="6c67a-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="6c67a-193">**Task**</span><span class="sxs-lookup"><span data-stu-id="6c67a-193">**Task**</span></span>|<span data-ttu-id="6c67a-194">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="6c67a-194">**EWS operation**</span></span>|<span data-ttu-id="6c67a-195">**Amostra**</span><span class="sxs-lookup"><span data-stu-id="6c67a-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6c67a-196">Obtenha um contato</span><span class="sxs-lookup"><span data-stu-id="6c67a-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="6c67a-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="6c67a-197">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="6c67a-198">Obter um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="6c67a-199">Atualização de um contato</span><span class="sxs-lookup"><span data-stu-id="6c67a-199">Update a contact</span></span>  <br/> |<span data-ttu-id="6c67a-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="6c67a-201">Atualizar um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="6c67a-202">Excluir um contato</span><span class="sxs-lookup"><span data-stu-id="6c67a-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="6c67a-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c67a-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="6c67a-204">Excluir um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="6c67a-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c67a-205">Confira também</span><span class="sxs-lookup"><span data-stu-id="6c67a-205">See also</span></span>

- [<span data-ttu-id="6c67a-206">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6c67a-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="6c67a-207">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6c67a-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6c67a-208">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6c67a-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6c67a-209">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6c67a-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="6c67a-210">Resolver nomes de ambíguos, usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6c67a-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

