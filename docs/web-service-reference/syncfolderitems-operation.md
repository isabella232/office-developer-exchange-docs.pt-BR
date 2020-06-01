---
title: Operação SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: A operação SyncFolderItems sincroniza itens entre o servidor Exchange e o cliente.
ms.openlocfilehash: 1a28d895eda11dd43f77ec2662a60a426cfc463c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468142"
---
# <a name="syncfolderitems-operation"></a><span data-ttu-id="09db0-103">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="09db0-103">SyncFolderItems operation</span></span>

<span data-ttu-id="09db0-104">A operação SyncFolderItems sincroniza itens entre o servidor Exchange e o cliente.</span><span class="sxs-lookup"><span data-stu-id="09db0-104">The SyncFolderItems operation synchronizes items between the Exchange server and the client.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09db0-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="09db0-105">Remarks</span></span>

<span data-ttu-id="09db0-106">A operação SyncFolderItems retornará um máximo de 512 alterações.</span><span class="sxs-lookup"><span data-stu-id="09db0-106">The SyncFolderItems operation will return a maximum of 512 changes.</span></span> <span data-ttu-id="09db0-107">As solicitações SyncFolderItems subsequentes devem ser executadas para obter alterações adicionais.</span><span class="sxs-lookup"><span data-stu-id="09db0-107">Subsequent SyncFolderItems requests must be performed to get additional changes.</span></span> 
  
<span data-ttu-id="09db0-108">SyncFolderItems é semelhante à operação FindItem, pois não é possível retornar propriedades como Body ou Attachments.</span><span class="sxs-lookup"><span data-stu-id="09db0-108">SyncFolderItems is similar to the FindItem operation in that it cannot return properties like Body or Attachments.</span></span> <span data-ttu-id="09db0-109">Se a operação SyncFolderItems não retornar as propriedades que você precisa, você pode usar a [operação GetItem](getitem-operation.md) para obter um conjunto específico de propriedades para cada item retornado por SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="09db0-109">If the SyncFolderItems operation does not return the properties that you need, you can use the [GetItem operation](getitem-operation.md) to get a specific set of properties for each item that it returned by SyncFolderItems.</span></span> 
  
## <a name="syncfolderitems-request-example"></a><span data-ttu-id="09db0-110">Exemplo de solicitação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="09db0-110">SyncFolderItems request example</span></span>

### <a name="description"></a><span data-ttu-id="09db0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="09db0-111">Description</span></span>

<span data-ttu-id="09db0-112">O exemplo a seguir de uma solicitação SyncFolderItems mostra como sincronizar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="09db0-112">The following example of a SyncFolderItems request shows how to synchronize items in a folder.</span></span> <span data-ttu-id="09db0-113">Este exemplo mostra uma sincronização de item de pasta que não é a primeira sincronização que ocorreu para a pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="09db0-113">This example shows a folder item's synchronization that is not the first synchronization to have occurred for the Sent Items folder.</span></span> <span data-ttu-id="09db0-114">O elemento [SyncState](syncstate-ex15websvcsotherref.md) não está incluído na solicitação para a primeira tentativa de sincronizar um cliente com o Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="09db0-114">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="09db0-115">A primeira tentativa de sincronizar os itens em uma hierarquia de pastas retornará todos os itens da caixa de correio, excluindo os itens identificados no elemento [ignore](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="09db0-115">The first attempt to synchronize the items in a folder hierarchy will return all the items in the mailbox, excluding items that are identified in the [Ignore](ignore.md) element.</span></span> <span data-ttu-id="09db0-116">Essa solicitação de SyncFolderItems tentará sincronizar todas as alterações feitas nos itens de pasta desde a última sincronização.</span><span class="sxs-lookup"><span data-stu-id="09db0-116">This SyncFolderItems request will try to synchronize all changes to the folder items since the last synchronization.</span></span> <span data-ttu-id="09db0-117">Essa solicitação ignorará a tentativa de sincronização de um item identificado no elemento [ignore](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="09db0-117">This request will ignore the attempt to synchronize the one item that is identified in the [Ignore](ignore.md) element.</span></span> 
  
### <a name="code"></a><span data-ttu-id="09db0-118">Código</span><span class="sxs-lookup"><span data-stu-id="09db0-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="09db0-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="09db0-119">Comments</span></span>

<span data-ttu-id="09db0-120">O elemento [SyncState](syncstate-ex15websvcsotherref.md) dados codificados em Base64 e o atributo **ID** do elemento [ItemId](itemid.md) foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="09db0-120">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="09db0-121">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="09db0-121">Request elements</span></span>

<span data-ttu-id="09db0-122">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="09db0-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="09db0-123">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="09db0-123">SyncFolderItems</span></span>](syncfolderitems.md)
    
- [<span data-ttu-id="09db0-124">Shape</span><span class="sxs-lookup"><span data-stu-id="09db0-124">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="09db0-125">BaseShape</span><span class="sxs-lookup"><span data-stu-id="09db0-125">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="09db0-126">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="09db0-126">SyncFolderId</span></span>](syncfolderid.md)
    
- [<span data-ttu-id="09db0-127">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="09db0-127">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="09db0-128">SyncState</span><span class="sxs-lookup"><span data-stu-id="09db0-128">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="09db0-129">Ignore</span><span class="sxs-lookup"><span data-stu-id="09db0-129">Ignore</span></span>](ignore.md)
    
- [<span data-ttu-id="09db0-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="09db0-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="09db0-131">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="09db0-131">MaxChangesReturned</span></span>](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a><span data-ttu-id="09db0-132">Resposta SyncFolderItems bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="09db0-132">Successful SyncFolderItems Response</span></span>

### <a name="description"></a><span data-ttu-id="09db0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="09db0-133">Description</span></span>

<span data-ttu-id="09db0-134">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="09db0-134">The following example shows a successful response to the SyncFolderItems request.</span></span> <span data-ttu-id="09db0-135">Neste exemplo, uma solicitação de reunião é sincronizada a partir da pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="09db0-135">In this example, a meeting request is synchronized from the Sent Items folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="09db0-136">Código</span><span class="sxs-lookup"><span data-stu-id="09db0-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="09db0-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="09db0-137">Comments</span></span>

<span data-ttu-id="09db0-138">O elemento [SyncState](syncstate-ex15websvcsotherref.md) dados codificados em Base64 e o atributo **ID** do elemento [ItemId](itemid.md) foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="09db0-138">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="09db0-139">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="09db0-139">Successful response elements</span></span>

<span data-ttu-id="09db0-140">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="09db0-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="09db0-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="09db0-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="09db0-142">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="09db0-142">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="09db0-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="09db0-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="09db0-144">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="09db0-144">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="09db0-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="09db0-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="09db0-146">SyncState</span><span class="sxs-lookup"><span data-stu-id="09db0-146">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="09db0-147">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="09db0-147">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
- [<span data-ttu-id="09db0-148">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="09db0-148">Changes (Items)</span></span>](changes-items.md)
    
- [<span data-ttu-id="09db0-149">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="09db0-149">Create (ItemSync)</span></span>](create-itemsync.md)
    
- [<span data-ttu-id="09db0-150">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="09db0-150">MeetingRequest</span></span>](meetingrequest.md)
    
- [<span data-ttu-id="09db0-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="09db0-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="09db0-152">Assunto</span><span class="sxs-lookup"><span data-stu-id="09db0-152">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="09db0-153">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="09db0-153">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="09db0-154">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="09db0-154">IsOutOfDate</span></span>](isoutofdate.md)
    
- [<span data-ttu-id="09db0-155">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="09db0-155">HasBeenProcessed</span></span>](hasbeenprocessed.md)
    
- [<span data-ttu-id="09db0-156">ResponseType</span><span class="sxs-lookup"><span data-stu-id="09db0-156">ResponseType</span></span>](responsetype.md)
    
- [<span data-ttu-id="09db0-157">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="09db0-157">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md)
    
- [<span data-ttu-id="09db0-158">Start</span><span class="sxs-lookup"><span data-stu-id="09db0-158">Start</span></span>](start.md)
    
- [<span data-ttu-id="09db0-159">Ponto</span><span class="sxs-lookup"><span data-stu-id="09db0-159">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="09db0-160">Localização</span><span class="sxs-lookup"><span data-stu-id="09db0-160">Location</span></span>](location.md)
    
- [<span data-ttu-id="09db0-161">Organizador</span><span class="sxs-lookup"><span data-stu-id="09db0-161">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="09db0-162">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="09db0-162">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="09db0-163">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="09db0-163">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="09db0-164">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="09db0-164">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="09db0-165">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="09db0-165">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a><span data-ttu-id="09db0-166">Resposta de erro SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="09db0-166">SyncFolderItems error response</span></span>

### <a name="description"></a><span data-ttu-id="09db0-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="09db0-167">Description</span></span>

<span data-ttu-id="09db0-168">O exemplo a seguir mostra uma resposta de erro a uma solicitação SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="09db0-168">The following example shows an error response to a SyncFolderItems request.</span></span> <span data-ttu-id="09db0-169">Esse erro foi causado por um SyncState inválido.</span><span class="sxs-lookup"><span data-stu-id="09db0-169">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="09db0-170">Código</span><span class="sxs-lookup"><span data-stu-id="09db0-170">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="09db0-171">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="09db0-171">Error response elements</span></span>

<span data-ttu-id="09db0-172">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="09db0-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="09db0-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="09db0-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="09db0-174">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="09db0-174">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="09db0-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="09db0-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="09db0-176">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="09db0-176">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="09db0-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="09db0-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="09db0-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="09db0-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="09db0-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="09db0-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="09db0-180">SyncState</span><span class="sxs-lookup"><span data-stu-id="09db0-180">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="09db0-181">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="09db0-181">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
## <a name="see-also"></a><span data-ttu-id="09db0-182">Também consulte</span><span class="sxs-lookup"><span data-stu-id="09db0-182">See also</span></span>



- [<span data-ttu-id="09db0-183">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="09db0-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

