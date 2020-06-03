---
title: Obter listas de salas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 15980e4a-e41c-4194-829a-cadbdf365bf1
description: Saiba como obter uma lista de todas as listas de salas em sua organização ou uma única lista de salas de um servidor do Exchange usando a API gerenciada do EWS ou o EWS.
localization_priority: Priority
ms.openlocfilehash: 7c571b0550f861552cdbe8c5b30138101c9fc788
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455790"
---
# <a name="get-room-lists-by-using-ews-in-exchange"></a><span data-ttu-id="17891-103">Obter listas de salas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="17891-103">Get room lists by using EWS in Exchange</span></span>

<span data-ttu-id="17891-104">Saiba como obter uma lista de todas as listas de salas em sua organização ou uma única lista de salas de um servidor do Exchange usando a API gerenciada do EWS ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="17891-104">Learn how to get a list of all the room lists in your organization or a single room list from an Exchange server by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="17891-105">Você pode usar a API gerenciada do EWS ou o EWS para obter informações sobre salas e como as salas são agrupadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="17891-105">You can use the EWS Managed API or EWS to get information about rooms and how the rooms are grouped in your organization.</span></span> <span data-ttu-id="17891-106">As listas de salas não existem por padrão; o administrador precisa criar e organizá-los.</span><span class="sxs-lookup"><span data-stu-id="17891-106">Room lists don't exist by default; your administrator needs to create and organize them.</span></span> <span data-ttu-id="17891-107">Normalmente, eles são organizados por local ou departamento, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="17891-107">Typically, they're organized by location or department, as shown in the following example.</span></span>
  
<span data-ttu-id="17891-108">**Nomes de lista de salas da Contoso e endereços de email**</span><span class="sxs-lookup"><span data-stu-id="17891-108">**Contoso room list names and email addresses**</span></span>

|<span data-ttu-id="17891-109">**Nome da lista de salas**</span><span class="sxs-lookup"><span data-stu-id="17891-109">**Name of room list**</span></span>|<span data-ttu-id="17891-110">**Endereço de email da lista de salas**</span><span class="sxs-lookup"><span data-stu-id="17891-110">**Email address of room list**</span></span>|
|:-----|:-----|
|<span data-ttu-id="17891-111">Construindo 11 lista de salas</span><span class="sxs-lookup"><span data-stu-id="17891-111">Building 11 room list</span></span>  <br/> |<span data-ttu-id="17891-112">Bldg11rooms@contoso.com</span><span class="sxs-lookup"><span data-stu-id="17891-112">Bldg11rooms@contoso.com</span></span>  <br/> |
|<span data-ttu-id="17891-113">Lista de salas de conferência de construção de Ciências de saúde</span><span class="sxs-lookup"><span data-stu-id="17891-113">Health Science Building Conference Room List</span></span>  <br/> |<span data-ttu-id="17891-114">HSbldgrooms@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="17891-114">HSbldgrooms@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="17891-115">Salas de reunião de chão de contas</span><span class="sxs-lookup"><span data-stu-id="17891-115">Accounting Floor Meeting Rooms</span></span>  <br/> |<span data-ttu-id="17891-116">Acctfloor300@contoso.com</span><span class="sxs-lookup"><span data-stu-id="17891-116">Acctfloor300@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="17891-117">Cada sala em uma lista de salas tem um nome e endereço de email associado a ela.</span><span class="sxs-lookup"><span data-stu-id="17891-117">Each room in a room list has a name and email address associated with it.</span></span>
  
<span data-ttu-id="17891-118">**Nomes de sala e endereços de email da contoso**</span><span class="sxs-lookup"><span data-stu-id="17891-118">**Contoso room names and email addresses**</span></span>

|<span data-ttu-id="17891-119">**Nome da sala**</span><span class="sxs-lookup"><span data-stu-id="17891-119">**Name of room**</span></span>|<span data-ttu-id="17891-120">**Endereço de email da sala**</span><span class="sxs-lookup"><span data-stu-id="17891-120">**Email address of room**</span></span>|
|:-----|:-----|
|<span data-ttu-id="17891-121">Conf sala 11/101 (8) AV</span><span class="sxs-lookup"><span data-stu-id="17891-121">Conf Room 11/101 (8) AV</span></span>  <br/> |<span data-ttu-id="17891-122">Cf11101@contoso.com</span><span class="sxs-lookup"><span data-stu-id="17891-122">Cf11101@contoso.com</span></span>  <br/> |
|<span data-ttu-id="17891-123">Laboratório de demonstração HS (100)</span><span class="sxs-lookup"><span data-stu-id="17891-123">HS Demonstration Lab (100)</span></span>  <br/> |<span data-ttu-id="17891-124">Hs101@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="17891-124">Hs101@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="17891-125">Estatísticas 305 WB</span><span class="sxs-lookup"><span data-stu-id="17891-125">Accounting 305 WB</span></span>  <br/> |<span data-ttu-id="17891-126">Acct305@contoso.com</span><span class="sxs-lookup"><span data-stu-id="17891-126">Acct305@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="17891-127">Você pode obter uma lista que contém todas as listas de salas usando o método [ExchangeService. GetRoomLists](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS Managed API ou a operação [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="17891-127">You can get a list that contains all room lists by using either the [ExchangeService.GetRoomLists](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="17891-128">Você pode recuperar uma única lista de salas que contenha todas as salas de um local ou departamento fornecendo seu endereço de email usando o método de API gerenciada do EWS de [Getrooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) ou a operação EWS de [getrooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="17891-128">You can retrieve a single room list that contains all the rooms for a location or department by supplying its email address by using the [GetRooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="17891-129">Quando você tem uma coleção de salas associada a uma lista de salas, você pode pesquisar pela coleção para identificar a sala ou as salas desejadas por endereço de email ou procurando palavras-chave no nome, como "AV" ou "Lab".</span><span class="sxs-lookup"><span data-stu-id="17891-129">When you have a collection of rooms associated with a room list, you can then search through the collection to identify the room or rooms you want, either by email address, or by looking for key words in the name, such as "AV", or "Lab".</span></span> 
  
## <a name="get-all-room-lists-by-using-the-ews-managed-api"></a><span data-ttu-id="17891-130">Obter todas as listas de salas usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="17891-130">Get all room lists by using the EWS Managed API</span></span>
<span data-ttu-id="17891-131"><a name="bk_GetRoomListewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="17891-131"><a name="bk_GetRoomListewsma"> </a></span></span>

<span data-ttu-id="17891-132">O exemplo a seguir mostra como obter uma lista que contém todas as listas de salas em sua organização usando o método [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) .</span><span class="sxs-lookup"><span data-stu-id="17891-132">The following example shows how to get a list that contains all the room lists in your organization by using the [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) method.</span></span> 
  
<span data-ttu-id="17891-133">Este exemplo pressupõe que você tenha autenticado em um servidor do Exchange e tenha adquirido um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) chamado **Service**.</span><span class="sxs-lookup"><span data-stu-id="17891-133">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
// Return all the room lists in the organization.
// This method call results in a GetRoomLists call to EWS.
EmailAddressCollection myRoomLists = service.GetRoomLists();
// Display the room lists.
foreach (EmailAddress address in myRoomLists)
{
    Console.WriteLine("Email Address: {0} Mailbox Type: {1}", address.Address, address.MailboxType);
}

```

## <a name="get-all-room-lists-by-using-ews"></a><span data-ttu-id="17891-134">Obter todas as listas de salas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="17891-134">Get all room lists by using EWS</span></span>
<span data-ttu-id="17891-135"><a name="bk_GetRoomListews"> </a></span><span class="sxs-lookup"><span data-stu-id="17891-135"><a name="bk_GetRoomListews"> </a></span></span>

<span data-ttu-id="17891-136">O exemplo a seguir mostra como obter uma coleção de todos os [RoomLists](https://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) da sua organização usando a operação [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="17891-136">The following example shows how to get a collection of all your organization's [RoomLists](https://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) by using the [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="17891-137">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [obter todas as listas de salas](#bk_GetRoomListewsma).</span><span class="sxs-lookup"><span data-stu-id="17891-137">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all room lists](#bk_GetRoomListewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="17891-138">O servidor responde à solicitação [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) com uma mensagem [GetRoomListsResponse](https://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) que contém as listas de salas da sua organização.</span><span class="sxs-lookup"><span data-stu-id="17891-138">The server responds to the [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) request with a [GetRoomListsResponse](https://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) message that contains the room lists for your organization.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="868" MinorBuildNumber="8" Version="V2_9" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomListsResponse ResponseClass="Success" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:RoomLists>
        <t:Address>
          <t:Name>Contoso Building 1 Room List</t:Name>
          <t:EmailAddress>bldg1rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 2 Room List</t:Name>
          <t:EmailAddress>bldg2rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 3 Room List</t:Name>
          <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </m:GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-the-ews-managed-api"></a><span data-ttu-id="17891-139">Obter todas as salas em uma lista de salas usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="17891-139">Get all the rooms in a room list by using the EWS Managed API</span></span>
<span data-ttu-id="17891-140"><a name="bk_FindRoomewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="17891-140"><a name="bk_FindRoomewsma"> </a></span></span>

<span data-ttu-id="17891-141">O exemplo a seguir mostra como obter uma coleção de salas em uma lista de salas usando o método [Getrooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) .</span><span class="sxs-lookup"><span data-stu-id="17891-141">The following example shows how to get a collection of rooms in a room list by using the [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) method.</span></span> 
  
```cs
EmailAddress myRoomList = "bldg3rooms@contoso.com";
// This method call results in a GetRooms call to EWS.
System.Collections.ObjectModel.Collection<EmailAddress> myRoomAddresses = service.GetRooms(myRoomList);
// Display the individual rooms.
foreach (EmailAddress address in myRoomAddresses)
{
    Console.WriteLine("Email Address: {0}", address.Address);
}

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-ews"></a><span data-ttu-id="17891-142">Obter todas as salas em uma lista de salas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="17891-142">Get all the rooms in a room list by using EWS</span></span>
<span data-ttu-id="17891-143"><a name="bk_FindRoomews"> </a></span><span class="sxs-lookup"><span data-stu-id="17891-143"><a name="bk_FindRoomews"> </a></span></span>

<span data-ttu-id="17891-144">O exemplo a seguir mostra como obter uma lista de [salas](https://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) em uma [sala](https://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) de salas usando a operação [getrooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="17891-144">The following example shows how to get a list of [rooms](https://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) in a [RoomList](https://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) by using the [GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="17891-145">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [obter todas as salas em uma lista de salas](#bk_FindRoomewsma).</span><span class="sxs-lookup"><span data-stu-id="17891-145">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all the rooms in a room list](#bk_FindRoomewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="17891-146">O servidor responde à solicitação [Getrooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) com uma mensagem do [GetRoomsResponse](https://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) que contém as salas na lista de salas.</span><span class="sxs-lookup"><span data-stu-id="17891-146">The server responds to the [GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) request with a [GetRoomsResponse](https://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) message that contains the rooms in the room list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="873" MinorBuildNumber="9" 
                         Version="V2_9" xmlns:h="http://scemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomsResponse ResponseClass="Success" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://scemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Rooms>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/101 (16) AV</t:Name>
            <t:EmailAddress>cf3101@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/102 (8) AV</t:Name>
            <t:EmailAddress>cf3102@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/103 (14) AV RoundTable</t:Name>
            <t:EmailAddress>cf3103@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </m:GetRoomsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="17891-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="17891-147">See also</span></span>


- [<span data-ttu-id="17891-148">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="17891-148">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="17891-149">Obter informações de disponibilidade usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="17891-149">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="17891-150">Criar e Gerenciar Caixas de Correio</span><span class="sxs-lookup"><span data-stu-id="17891-150">Create and Manage Room Mailboxes</span></span>](https://technet.microsoft.com/library/jj215781%28v=exchg.150%29.aspx)
    

