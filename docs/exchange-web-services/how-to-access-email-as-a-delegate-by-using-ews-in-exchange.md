---
title: Email de acesso como um representante, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Saiba como acessar o email como um representante, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 23dd35f95b1303ff643e3760aa408e308725cb12
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354033"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="52edc-103">Email de acesso como um representante, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52edc-103">Access email as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="52edc-104">Saiba como acessar o email como um representante, usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="52edc-104">Learn how to access email as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="52edc-105">Você pode usar a API gerenciada de EWS ou EWS para conceder a um usuário Delegar acesso à pasta de caixa de entrada de um proprietário caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Inbox folder.</span></span> <span data-ttu-id="52edc-106">O representante pode então criar solicitações de reunião em nome do proprietário da caixa de correio, pesquisar por email, recuperar, atualizar e excluir o email da pasta de caixa de entrada do proprietário da caixa de correio, dependendo de suas permissões.</span><span class="sxs-lookup"><span data-stu-id="52edc-106">The delegate can then create meeting requests on behalf of the mailbox owner, search for email, and retrieve, update, and delete email from the mailbox owner's Inbox folder, depending on their permissions.</span></span>
  
<span data-ttu-id="52edc-107">Como um representante, use os métodos e as mesmas operações para acessar a pasta de caixa de entrada de um proprietário caixa de correio que você pode usar para acessar uma pasta de caixa de entrada sem acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="52edc-107">As a delegate, you use the same methods and operations to access a mailbox owner's Inbox folder that you use to access an Inbox folder without delegate access.</span></span> <span data-ttu-id="52edc-108">A principal diferença é que você precisa usar [acesso explícito](delegate-access-and-ews-in-exchange.md#bk_explicit) para localizar ou criar um item de email e, em seguida, depois de identificar a ID do item, você pode usar [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) para obter, atualizar ou excluir o item.</span><span class="sxs-lookup"><span data-stu-id="52edc-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create an email item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="52edc-109">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para acessar email como um representante**</span><span class="sxs-lookup"><span data-stu-id="52edc-109">**Table 1. EWS Managed API methods and EWS operations for accessing email as a delegate**</span></span>

|<span data-ttu-id="52edc-110">**Se você quiser …**</span><span class="sxs-lookup"><span data-stu-id="52edc-110">**If you want to…**</span></span>|<span data-ttu-id="52edc-111">**Use este método de API gerenciada de EWS …**</span><span class="sxs-lookup"><span data-stu-id="52edc-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="52edc-112">**Use essa operação EWS …**</span><span class="sxs-lookup"><span data-stu-id="52edc-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="52edc-113">Criar e enviar um email como um representante</span><span class="sxs-lookup"><span data-stu-id="52edc-113">Create and send an email as a delegate</span></span>  <br/> |<span data-ttu-id="52edc-114">[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) na pasta Rascunhos do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-114">[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Drafts folder</span></span>  <br/> <span data-ttu-id="52edc-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) onde o parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de itens enviados do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Sent Items folder</span></span>  <br/> |<span data-ttu-id="52edc-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> <span data-ttu-id="52edc-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="52edc-118">Criar várias mensagens de email como um representante</span><span class="sxs-lookup"><span data-stu-id="52edc-118">Create multiple email messages as a delegate</span></span>  <br/> |<span data-ttu-id="52edc-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de caixa de entrada do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="52edc-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="52edc-121">Pesquise ou encontrar um email como um representante</span><span class="sxs-lookup"><span data-stu-id="52edc-121">Search for or find an email as a delegate</span></span>  <br/> |<span data-ttu-id="52edc-122">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) onde o parâmetro **FolderId** fornece [acesso explícitos](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) a pasta de caixa de entrada do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-122">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="52edc-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) onde o elemento de [caixa de correio](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) Especifica o [endereço de email](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) do proprietário da caixa de correio</span><span class="sxs-lookup"><span data-stu-id="52edc-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="52edc-124">Obtenha um email como um representante</span><span class="sxs-lookup"><span data-stu-id="52edc-124">Get an email as a delegate</span></span>  <br/> |[<span data-ttu-id="52edc-125">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="52edc-125">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="52edc-126">GetItem</span><span class="sxs-lookup"><span data-stu-id="52edc-126">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="52edc-127">Atualizar um email como um representante</span><span class="sxs-lookup"><span data-stu-id="52edc-127">Update an email as a delegate</span></span>  <br/> |<span data-ttu-id="52edc-128">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="52edc-128">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="52edc-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="52edc-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="52edc-130">Excluir um email como um representante</span><span class="sxs-lookup"><span data-stu-id="52edc-130">Delete an email as a delegate</span></span>  <br/> |<span data-ttu-id="52edc-131">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="52edc-131">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="52edc-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="52edc-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
<span data-ttu-id="52edc-133">Mantenha as seguintes coisas em mente ao trabalhar com emails como um representante:</span><span class="sxs-lookup"><span data-stu-id="52edc-133">Keep the following things in mind when working with emails as a delegate:</span></span>
  
- <span data-ttu-id="52edc-134">Se um delegado só precisa trabalhar com as solicitações de reunião e respostas, o representante não precisará ter acesso à pasta de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="52edc-134">If a delegate only needs to work with meeting requests and responses, the delegate does not need access to the Inbox folder.</span></span> <span data-ttu-id="52edc-135">Para obter mais informações, consulte [tarefas de pré-requisito para acessar os calendários como um representante](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span><span class="sxs-lookup"><span data-stu-id="52edc-135">For more information, see [prerequisite tasks for accessing calendars as a delegate](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span></span>
    
- <span data-ttu-id="52edc-136">Quando um destinatário recebe uma mensagem que foi enviada em nome de um proprietário de caixa de correio, o remetente aparece como " *representante* em nome do *proprietário da caixa de correio* ".</span><span class="sxs-lookup"><span data-stu-id="52edc-136">When a recipient receives a message that was sent on behalf of a mailbox owner, the sender appears as " *Delegate*  on behalf of  *mailbox owner*  ."</span></span> 
    
> [!NOTE]
> <span data-ttu-id="52edc-137">Os exemplos de código neste artigo, primary@contoso.com é o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-137">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="52edc-138">Tarefas de pré-requisito</span><span class="sxs-lookup"><span data-stu-id="52edc-138">Prerequisite tasks</span></span>
<span data-ttu-id="52edc-139"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-139"></span></span>

<span data-ttu-id="52edc-140">Antes de um usuário pode acessar a pasta de caixa de entrada do proprietário da caixa de correio como um representante, o usuário deve ser [adicionado como um representante com permissões](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para a pasta de caixa de entrada do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-140">Before a user can access the mailbox owner's Inbox folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="52edc-141">Criar e enviar um email como um representante, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-141">Create and send an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="52edc-142"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-142"></span></span>

<span data-ttu-id="52edc-143">A API gerenciada de EWS permite que você use o objeto de serviço para o usuário delegado para criar e enviar emails em nome do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-143">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="52edc-144">Este exemplo mostra como usar o método [Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) para salvar a mensagem na pasta Rascunhos do proprietário da caixa de correio e, em seguida, o método [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) para enviar o email e salve a mensagem na pasta de itens enviados do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-144">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) method to save the message in the mailbox owner's Drafts folder, and then the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) method to send the mail and save the message in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="52edc-145">Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o representante e o delegado recebeu as [permissões apropriadas para a pasta de caixa de entrada, Rascunhos e itens enviados do proprietário da caixa de correio](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="52edc-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the [appropriate permissions for the mailbox owner's Inbox, Drafts, and Sent Items folder](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
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

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="52edc-146">Criar e enviar um email como um representante, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-146">Create and send an email as a delegate by using EWS</span></span>
<span data-ttu-id="52edc-147"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-147"></span></span>

<span data-ttu-id="52edc-148">EWS permite que você use o objeto de serviço para o usuário delegado para criar e enviar emails em nome do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-148">EWS enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="52edc-149">Este exemplo mostra como usar a operação [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) para criar um email e a operação [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) para enviar o tempo e salve-o na pasta de itens enviados do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-149">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an email and the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the time and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="52edc-150">Isso também é a primeira solicitação XML que o EWS Managed API envia quando você usa o método **Save** para [criar e enviar um email](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="52edc-150">This is also the first XML request that the EWS Managed API sends when you use the **Save** method to [create and send an email](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="52edc-151">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que o email foi criado e salva com êxito.</span><span class="sxs-lookup"><span data-stu-id="52edc-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was created and saved successfully.</span></span> <span data-ttu-id="52edc-152">A resposta também contém a ID de item do email recém-criado.</span><span class="sxs-lookup"><span data-stu-id="52edc-152">The response also contains the item ID of the newly created email.</span></span>
  
<span data-ttu-id="52edc-153">O valor de **ItemId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52edc-153">The **ItemId** value has been shortened for readability.</span></span> 
  
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
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="52edc-154">Em seguida, use a operação **SendItem** para enviar a mensagem em nome do proprietário da caixa de correio e salve-o na pasta de itens enviados do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-154">Next, use the **SendItem** operation to send the message on behalf of the mailbox owner and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="52edc-155">O valor de **ItemId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52edc-155">The **ItemId** value has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="52edc-156">O servidor responde à solicitação **SendItem** com uma mensagem de [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que o email foi enviado e salva a pasta de itens enviados do proprietário da caixa de correio com êxito.</span><span class="sxs-lookup"><span data-stu-id="52edc-156">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was sent and saved to the mailbox owner's Sent Items folder successfully.</span></span>
  
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
    <m:SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="52edc-157">Procurar um email como um representante usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-157">Search for an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="52edc-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-158"></span></span>

<span data-ttu-id="52edc-159">Para procurar um email, você deve usar um dos métodos [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) que inclui um parâmetro [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , para que você pode especificar uma pasta de caixa de entrada do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-159">To search for an email, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Inbox folder.</span></span> 
  
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

<span data-ttu-id="52edc-160">Depois que a chamada **FindItems** retornará uma resposta com uma ID, você pode obter, atualização ou exclusão de email usando a ID e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) - e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that email by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="52edc-161">Procure um email como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-161">Search for an email as a delegate by using EWS</span></span>
<span data-ttu-id="52edc-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-162"></span></span>

<span data-ttu-id="52edc-163">EWS permite que você use o objeto de serviço para o usuário delegado para procurar emails que atendam a um conjunto de critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52edc-163">EWS enables you to use the service object for the delegate user to search for emails that meet a set of search criteria.</span></span> <span data-ttu-id="52edc-164">Este exemplo mostra como usar a operação [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para encontrar mensagens na pasta de caixa de entrada do proprietário que contêm a palavra "futebol" no assunto.</span><span class="sxs-lookup"><span data-stu-id="52edc-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find messages in the owner's Inbox folder that contain the word "soccer" in the subject.</span></span> 
  
<span data-ttu-id="52edc-165">Isso também é a solicitação XML que o EWS Managed API envia quando você [Procurar um email](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="52edc-165">This is also the XML request that the EWS Managed API sends when you [search for an email](#bk_searchewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="52edc-166">O servidor responde à solicitação **FindItem** com uma mensagem de [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pesquisa foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="52edc-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="52edc-167">A resposta conterá um elemento de [mensagem](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) para qualquer e-mails que atendidos os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52edc-167">The response contains a [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element for any emails that met the search criteria.</span></span> <span data-ttu-id="52edc-168">Nesse caso, somente um email é encontrado.</span><span class="sxs-lookup"><span data-stu-id="52edc-168">In this case, only one email is found.</span></span> 
  
<span data-ttu-id="52edc-169">O valor do elemento [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52edc-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
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
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="52edc-170">Agora que você tem o **ItemId** para email que atende a seus critérios, você pode obter, update ou delete de email usando o **ItemId** e [acesso implícito](delegate-access-and-ews-in-exchange.md#bk_implicit) - e você não precisará especificar o endereço de SMTP do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-170">Now that you have the **ItemId** for the email that meets your criteria, you can get, update, or delete that email by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="52edc-171">Obter, atualizar ou excluir itens de email como um representante usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-171">Get, update, or delete email items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="52edc-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-172"></span></span>

<span data-ttu-id="52edc-173">Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir um email da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="52edc-173">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="52edc-174">A única diferença é que o objeto **ExchangeService** é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="52edc-174">The only difference is that the **ExchangeService** object is for the delegate user.</span></span> <span data-ttu-id="52edc-175">A ID do item incluída na chamada do método **vincular** exclusivamente identifica o item no repositório de caixa de correio, na pasta de caixa de entrada do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="52edc-176">**Tabela 2. Trabalhando com email como um representante de métodos de API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="52edc-176">**Table 2. EWS Managed API methods working with email as a delegate**</span></span>

|<span data-ttu-id="52edc-177">**Task**</span><span class="sxs-lookup"><span data-stu-id="52edc-177">**Task**</span></span>|<span data-ttu-id="52edc-178">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="52edc-178">**EWS Managed API method**</span></span>|<span data-ttu-id="52edc-179">**Código de exemplo**</span><span class="sxs-lookup"><span data-stu-id="52edc-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="52edc-180">Obtenha um email</span><span class="sxs-lookup"><span data-stu-id="52edc-180">Get an email</span></span>  <br/> |[<span data-ttu-id="52edc-181">Vincular</span><span class="sxs-lookup"><span data-stu-id="52edc-181">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="52edc-182">Obter um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="52edc-183">Atualizar um email</span><span class="sxs-lookup"><span data-stu-id="52edc-183">Update an email</span></span>  <br/> |<span data-ttu-id="52edc-184">[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido de [atualização](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="52edc-184">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="52edc-185">Atualização de um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-185">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="52edc-186">Excluir um email</span><span class="sxs-lookup"><span data-stu-id="52edc-186">Delete an email</span></span>  <br/> |<span data-ttu-id="52edc-187">[Vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) seguido [Excluir](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="52edc-187">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="52edc-188">Excluir um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-188">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="52edc-189">Obter, atualizar ou excluir itens de email como um representante usando o EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-189">Get, update, or delete email items as a delegate by using EWS</span></span>
<span data-ttu-id="52edc-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="52edc-190"></span></span>

<span data-ttu-id="52edc-191">Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir um email da mesma maneira que você executa essas ações quando você não estiver usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="52edc-191">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="52edc-192">A única diferença é que o objeto de serviço é para o usuário delegado.</span><span class="sxs-lookup"><span data-stu-id="52edc-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="52edc-193">A ID do item incluída na solicitação **GetItem** exclusivamente identifica o item no repositório de caixa de correio, na pasta de caixa de entrada do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52edc-193">The item ID included in the **GetItem** request uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="52edc-194">**Tabela 3. Operações do EWS para trabalhar com email como um representante**</span><span class="sxs-lookup"><span data-stu-id="52edc-194">**Table 3. EWS operations for working with email as a delegate**</span></span>

|<span data-ttu-id="52edc-195">**Task**</span><span class="sxs-lookup"><span data-stu-id="52edc-195">**Task**</span></span>|<span data-ttu-id="52edc-196">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="52edc-196">**EWS operation**</span></span>|<span data-ttu-id="52edc-197">**Código de exemplo**</span><span class="sxs-lookup"><span data-stu-id="52edc-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="52edc-198">Obtenha um email</span><span class="sxs-lookup"><span data-stu-id="52edc-198">Get an email</span></span>  <br/> |[<span data-ttu-id="52edc-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="52edc-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="52edc-200">Obter um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="52edc-201">Atualizar um email</span><span class="sxs-lookup"><span data-stu-id="52edc-201">Update an email</span></span>  <br/> |<span data-ttu-id="52edc-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="52edc-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="52edc-203">Atualizar um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-203">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="52edc-204">Excluir um email</span><span class="sxs-lookup"><span data-stu-id="52edc-204">Delete an email</span></span>  <br/> |<span data-ttu-id="52edc-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) seguido [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="52edc-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="52edc-206">Excluir um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="52edc-206">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52edc-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="52edc-207">See also</span></span>

- [<span data-ttu-id="52edc-208">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52edc-208">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)    
- [<span data-ttu-id="52edc-209">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52edc-209">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="52edc-210">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52edc-210">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="52edc-211">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52edc-211">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

