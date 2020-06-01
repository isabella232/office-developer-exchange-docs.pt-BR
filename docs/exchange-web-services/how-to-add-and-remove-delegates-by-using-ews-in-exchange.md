---
title: Adicionar e remover representantes usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cc7760bf-633b-483a-84ae-b52f437af2d3
description: Saiba como adicionar ou remover representantes de caixas de correio dos usuários usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 9db0171db51c0847d54bbcec7e28937eaed18d43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455335"
---
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a><span data-ttu-id="284cc-103">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="284cc-103">Add and remove delegates by using EWS in Exchange</span></span>

<span data-ttu-id="284cc-104">Saiba como adicionar ou remover representantes de caixas de correio dos usuários usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="284cc-104">Learn how to add delegates to or remove delegates from users' mailboxes by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="284cc-105">Você pode usar a API gerenciada do EWS ou o EWS para permitir que os representantes atuem em nome de um proprietário da caixa de correio ou removam o acesso de um representante a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="284cc-105">You can use the EWS Managed API or EWS to enable delegates to act on behalf of a mailbox owner or remove a delegate's access to a mailbox.</span></span> <span data-ttu-id="284cc-106">Os usuários adicionados como um representante e recebem permissões podem executar tarefas em nome do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="284cc-106">Users who are added as a delegate, and are given permissions, can perform tasks on behalf of the mailbox owner.</span></span> <span data-ttu-id="284cc-107">Por exemplo, eles podem criar e enviar convites de reunião, enviar emails e responder a solicitações de reunião no nome do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="284cc-107">For example, they can create and send meeting invitations, send emails, and respond to meeting requests on the mailbox owner's behalf.</span></span> 
  
<span data-ttu-id="284cc-108">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para adicionar e remover representantes**</span><span class="sxs-lookup"><span data-stu-id="284cc-108">**Table 1. EWS Managed API methods and EWS operations for adding and removing delegates**</span></span>

|<span data-ttu-id="284cc-109">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="284cc-109">**Task**</span></span>|<span data-ttu-id="284cc-110">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="284cc-110">**EWS Managed API method**</span></span>|<span data-ttu-id="284cc-111">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="284cc-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="284cc-112">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="284cc-112">Add delegates</span></span>  <br/> |[<span data-ttu-id="284cc-113">ExchangeService. adddelegates</span><span class="sxs-lookup"><span data-stu-id="284cc-113">ExchangeService.AddDelegates</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="284cc-114">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="284cc-114">AddDelegate</span></span>](https://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="284cc-115">Remover representantes</span><span class="sxs-lookup"><span data-stu-id="284cc-115">Remove delegates</span></span>  <br/> |[<span data-ttu-id="284cc-116">ExchangeService. RemoveDelegates</span><span class="sxs-lookup"><span data-stu-id="284cc-116">ExchangeService.RemoveDelegates</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="284cc-117">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="284cc-117">RemoveDelegate</span></span>](https://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="284cc-118">Após a concessão de permissões a uma pasta para um representante, elas podem atuar nos itens da pasta e em todas as subpastas, de acordo com suas [permissões de representante](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="284cc-118">After a delegate is granted permissions to a folder, they can act on items in the folder and any subfolders, according to their [delegate permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span> <span data-ttu-id="284cc-119">As permissões para representantes só se aplicam a subpastas criadas depois que o acesso de representante foi concedido.</span><span class="sxs-lookup"><span data-stu-id="284cc-119">Permissions for delegates only apply to subfolders that are created after the delegate access was granted.</span></span> <span data-ttu-id="284cc-120">Para atualizar permissões de pasta para pastas pré-existentes ou outras pastas, confira [definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="284cc-120">To update folder permissions for pre-existing folders, or other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="284cc-121">Observe que os representantes só podem ser adicionados às contas habilitadas para caixa de correio, incluindo grupos de segurança habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="284cc-121">Note that delegates can only be added to mailbox-enabled accounts, including mail-enabled security groups.</span></span> <span data-ttu-id="284cc-122">Por padrão, uma única chamada de acesso de representante do EWS pode acessar um máximo de 255 diferentes caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="284cc-122">By default, a single EWS delegate access call can access a maximum of 255 different mailboxes.</span></span>

<span data-ttu-id="284cc-123"><a name="bk_adddelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="284cc-123"><a name="bk_adddelegateewsma"> </a></span></span>

## <a name="add-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="284cc-124">Adicionar representantes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="284cc-124">Add delegates by using the EWS Managed API</span></span>

<span data-ttu-id="284cc-125">Você pode adicionar representantes a uma caixa de correio usando o método [Adddelegas](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="284cc-125">You can add delegates to a mailbox by using the [AddDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="284cc-126">Neste exemplo, um novo objeto de calendário, contato e email [DelegateUser](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) é criado, e cada representante recebe permissões de [Editor](delegate-access-and-ews-in-exchange.md#bk_delegateperms) para suas respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="284cc-126">In this example, a new calendar, contact, and email [DelegateUser](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) object is created, and each delegate is given [Editor permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms) for their respective folder.</span></span> <span data-ttu-id="284cc-127">Você pode modificar o exemplo para adicionar um representante a qualquer uma das pastas especificadas pelas [Propriedades DelegatePermissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), e você pode definir as permissões para qualquer um dos valores especificados pela enumeração [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="284cc-127">You can modify the example to add a delegate to any of the folders specified by the [DelegatePermissions properties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), and you can set the permissions to any of the values specified by the [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) enumeration.</span></span> 
  
<span data-ttu-id="284cc-128">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="284cc-128">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> AddDelegates(ExchangeService service)
{
    // Create a list to hold the new delegates to add.
    List<DelegateUser> newDelegates = new System.Collections.Generic.List<DelegateUser>();
    // Create a new delegate that has editor access to the mailbox owner's Calendar folder.
    DelegateUser calendarDelegate = new DelegateUser("calendardelegate@contoso.com");
    calendarDelegate.Permissions.CalendarFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(calendarDelegate);
    // Create a new delegate that has editor access to the mailbox owner's Contacts folder.
    DelegateUser contactDelegate = new DelegateUser("contactdelegate@contoso.com");
    contactDelegate.Permissions.ContactsFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(contactDelegate);
            
    // Create a new delegate that has editor access to the mailbox owner's Inbox folder.
    DelegateUser emailDelegate = new DelegateUser("emaildelegate@contoso.com");
    emailDelegate.Permissions.InboxFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(emailDelegate);
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.AddDelegates(mailbox, MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe, newDelegates);
            
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("For delegate " + resp.DelegateUser.UserId.PrimarySmtpAddress.ToString());
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        Console.WriteLine("\r\n");
    }
    return response;
}
```

<span data-ttu-id="284cc-129"><a name="bk_adddelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="284cc-129"><a name="bk_adddelegateews"> </a></span></span>

## <a name="add-delegates-by-using-ews"></a><span data-ttu-id="284cc-130">Adicionar representantes usando o EWS</span><span class="sxs-lookup"><span data-stu-id="284cc-130">Add delegates by using EWS</span></span>

<span data-ttu-id="284cc-131">O exemplo de código a seguir mostra como adicionar representantes de calendário, contato e email separados usando a operação do EWS [AddDelegate](https://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="284cc-131">The following code example shows how to add separate calendar, contact, and email delegates by using the [AddDelegate](https://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="284cc-132">A caixa de correio a ser modificada é especificada pelo elemento [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) , e as configurações de [permissão](delegate-access-and-ews-in-exchange.md#bk_delegateperms) para cada representante estão contidas no elemento [DelegateUser](https://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="284cc-132">The mailbox to modify is specified by the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element, and the [permission](delegate-access-and-ews-in-exchange.md#bk_delegateperms) settings for each delegate are contained in the [DelegateUser](https://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="284cc-133">Cada um dos representantes recebeu permissões de editor para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="284cc-133">Each of the delegates has been granted Editor permissions to their target folder.</span></span> 
  
<span data-ttu-id="284cc-134">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **Adddelegates** para [adicionar representantes](#bk_adddelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="284cc-134">This is also the XML request that the EWS Managed API sends when you use the **AddDelegates** method to [add delegates](#bk_adddelegateewsma).</span></span>
  
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
    <m:AddDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Editor</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Editor</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>Editor</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </m:DelegateUsers>
      <m:DeliverMeetingRequests>DelegatesAndSendInformationToMe</m:DeliverMeetingRequests>
    </m:AddDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="284cc-135">O servidor responde à solicitação **Adddelegar** com uma mensagem [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que os representantes foram criados com êxito.</span><span class="sxs-lookup"><span data-stu-id="284cc-135">The server responds to the **AddDelegate** request with an [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully created.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="888"
                         MinorBuildNumber="9"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:AddDelegateResponse ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535221</t:SID>
              <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>calendardelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535264</t:SID>
              <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>contactdelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
              <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>emaildelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="284cc-136"><a name="bk_removedelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="284cc-136"><a name="bk_removedelegateewsma"> </a></span></span>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="284cc-137">Remover representantes usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="284cc-137">Remove delegates by using the EWS Managed API</span></span>

<span data-ttu-id="284cc-138">Você pode remover representantes de uma caixa de correio de destino usando o método de API gerenciada do EWS [ExchangeService. RemoveDelegates](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="284cc-138">You can remove delegates from a target mailbox by using the [ExchangeService.RemoveDelegates](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="284cc-139">Neste exemplo, as permissões de representante definidas no [exemplo de adicionar um representante](#bk_adddelegateewsma) serão removidas.</span><span class="sxs-lookup"><span data-stu-id="284cc-139">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateewsma) are removed.</span></span> 
  
<span data-ttu-id="284cc-140">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="284cc-140">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> RemoveDelegates(ExchangeService service)
{
    // Create a list to hold the delegates to delete.
    List<UserId> deletedDelegates = new System.Collections.Generic.List<UserId>();
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("calendardelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("contactdelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("emaildelegate@contoso.com");
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.RemoveDelegates(mailbox, deletedDelegates);
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
    }
    return response;
}
```

<span data-ttu-id="284cc-141"><a name="bk_removedelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="284cc-141"><a name="bk_removedelegateews"> </a></span></span>

## <a name="remove-delegates-by-using-ews"></a><span data-ttu-id="284cc-142">Remover representantes usando EWS</span><span class="sxs-lookup"><span data-stu-id="284cc-142">Remove delegates by using EWS</span></span>

<span data-ttu-id="284cc-143">Você pode remover representantes de uma caixa de correio usando a operação [RemoveDelegate](https://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="284cc-143">You can remove delegates from a mailbox by using the [RemoveDelegate](https://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="284cc-144">Neste exemplo, as permissões de representante definidas no [exemplo de adicionar um representante](#bk_adddelegateews) serão removidas.</span><span class="sxs-lookup"><span data-stu-id="284cc-144">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateews) are removed.</span></span> 
  
<span data-ttu-id="284cc-145">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **RemoveDelegates** para [remover representantes](#bk_removedelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="284cc-145">This is also the XML request that the EWS Managed API sends when you use the **RemoveDelegates** method to [remove delegates](#bk_removedelegateewsma).</span></span>
  
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
    <m:RemoveDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
      </m:UserIds>
    </m:RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="284cc-146">O servidor responde à solicitação **RemoveDelegate** com uma mensagem [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que os representantes foram removidos com êxito.</span><span class="sxs-lookup"><span data-stu-id="284cc-146">The server responds to the **RemoveDelegate** request with a [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully removed.</span></span>

<span data-ttu-id="284cc-147"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="284cc-147"><a name="bk_nextsteps"> </a></span></span>

## <a name="next-steps"></a><span data-ttu-id="284cc-148">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="284cc-148">Next steps</span></span>

<span data-ttu-id="284cc-149">Após adicionar representantes às pastas de calendário, email e tarefas, o representante pode acessar os itens nas pastas.</span><span class="sxs-lookup"><span data-stu-id="284cc-149">After you add delegates to calendar, email, and task folders, the delegate can access the items in the folders.</span></span> <span data-ttu-id="284cc-150">Para saber mais, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="284cc-150">To learn more, see the following articles:</span></span>
  
- [<span data-ttu-id="284cc-151">Acessar email como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="284cc-151">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="284cc-152">Acessar um calendário como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="284cc-152">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="284cc-153">Acessar contatos como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="284cc-153">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
<span data-ttu-id="284cc-154">Se as pastas para as quais você adicionou representantes incluírem pastas filhas que foram criadas antes de você conceder acesso de representante, o representante não poderá acessar essas pastas sem permissões adicionais.</span><span class="sxs-lookup"><span data-stu-id="284cc-154">If the folders for which you added delegates include child folders that were created before you granted the delegate access, the delegate will not be able to access those folders without additional permissions.</span></span> <span data-ttu-id="284cc-155">Para adicionar essas permissões ou modificar permissões para qualquer outra pasta, confira [definir permissões de pasta para outro usuário usando o EWS no Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="284cc-155">To add these permissions, or modify permissions for any other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="284cc-156">Também consulte</span><span class="sxs-lookup"><span data-stu-id="284cc-156">See also</span></span>

- [<span data-ttu-id="284cc-157">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="284cc-157">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="284cc-158">Exchange 2013: adicionar usuários delegados a uma conta de email programaticamente</span><span class="sxs-lookup"><span data-stu-id="284cc-158">Exchange 2013: Add delegate users to an email account programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [<span data-ttu-id="284cc-159">Exchange 2013: atualizar representantes associados às contas de email programaticamente</span><span class="sxs-lookup"><span data-stu-id="284cc-159">Exchange 2013: Update delegates associated with email accounts programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [<span data-ttu-id="284cc-160">Exchange 2013: remover representantes associados às contas de email programaticamente</span><span class="sxs-lookup"><span data-stu-id="284cc-160">Exchange 2013: Remove delegates associated with email accounts programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

