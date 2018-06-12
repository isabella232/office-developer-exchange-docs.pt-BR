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
description: A operação SyncFolderItems sincroniza os itens entre o Exchange server e o cliente.
ms.openlocfilehash: 6b2e4694ac793e17a2b7cb2edb2cb9e6a4a105ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837688"
---
# <a name="syncfolderitems-operation"></a><span data-ttu-id="3ff34-103">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="3ff34-103">SyncFolderItems operation</span></span>

<span data-ttu-id="3ff34-104">A operação SyncFolderItems sincroniza os itens entre o Exchange server e o cliente.</span><span class="sxs-lookup"><span data-stu-id="3ff34-104">The SyncFolderItems operation synchronizes items between the Exchange server and the client.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3ff34-105">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3ff34-105">Remarks</span></span>

<span data-ttu-id="3ff34-106">A operação SyncFolderItems retornará um máximo de 512 alterações.</span><span class="sxs-lookup"><span data-stu-id="3ff34-106">The SyncFolderItems operation will return a maximum of 512 changes.</span></span> <span data-ttu-id="3ff34-107">As solicitações SyncFolderItems subsequentes devem ser executadas para fazer alterações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3ff34-107">Subsequent SyncFolderItems requests must be performed to get additional changes.</span></span> 
  
<span data-ttu-id="3ff34-108">SyncFolderItems é semelhante à operação FindItem em que ele não é possível retornar propriedades como corpo ou anexos.</span><span class="sxs-lookup"><span data-stu-id="3ff34-108">SyncFolderItems is similar to the FindItem operation in that it cannot return properties like Body or Attachments.</span></span> <span data-ttu-id="3ff34-109">Se a operação SyncFolderItems não retorna as propriedades que você precisa, você pode usar a [operação GetItem](getitem-operation.md) para obter um conjunto específico de propriedades para cada item que ele retornado pelo SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="3ff34-109">If the SyncFolderItems operation does not return the properties that you need, you can use the [GetItem operation](getitem-operation.md) to get a specific set of properties for each item that it returned by SyncFolderItems.</span></span> 
  
## <a name="syncfolderitems-request-example"></a><span data-ttu-id="3ff34-110">Exemplo de solicitação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="3ff34-110">SyncFolderItems request example</span></span>

### <a name="description"></a><span data-ttu-id="3ff34-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff34-111">Description</span></span>

<span data-ttu-id="3ff34-112">O exemplo a seguir de uma solicitação de SyncFolderItems mostra como sincronizar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3ff34-112">The following example of a SyncFolderItems request shows how to synchronize items in a folder.</span></span> <span data-ttu-id="3ff34-113">Este exemplo mostra a sincronização de um item pasta que não seja a primeira sincronização que ocorreram para a pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="3ff34-113">This example shows a folder item's synchronization that is not the first synchronization to have occurred for the Sent Items folder.</span></span> <span data-ttu-id="3ff34-114">O elemento de [estado de sincronização](syncstate-ex15websvcsotherref.md) não está incluído na solicitação para a primeira tentativa sincronizar um cliente com o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="3ff34-114">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="3ff34-115">A primeira tentativa de sincronizar os itens em uma hierarquia de pasta retornará todos os itens na caixa de correio, excluindo itens que são identificados no elemento [Ignorar](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="3ff34-115">The first attempt to synchronize the items in a folder hierarchy will return all the items in the mailbox, excluding items that are identified in the [Ignore](ignore.md) element.</span></span> <span data-ttu-id="3ff34-116">Essa solicitação SyncFolderItems tentará sincronizar todas as mudanças para os itens da pasta desde a última sincronização.</span><span class="sxs-lookup"><span data-stu-id="3ff34-116">This SyncFolderItems request will try to synchronize all changes to the folder items since the last synchronization.</span></span> <span data-ttu-id="3ff34-117">Essa solicitação irá ignorar a tentativa de sincronizar o um item que é identificado no elemento [Ignorar](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="3ff34-117">This request will ignore the attempt to synchronize the one item that is identified in the [Ignore](ignore.md) element.</span></span> 
  
### <a name="code"></a><span data-ttu-id="3ff34-118">Código</span><span class="sxs-lookup"><span data-stu-id="3ff34-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="3ff34-119">Comments</span><span class="sxs-lookup"><span data-stu-id="3ff34-119">Comments</span></span>

<span data-ttu-id="3ff34-120">Os dados de [estado de sincronização](syncstate-ex15websvcsotherref.md) do elemento codificado na base64 e o atributo de **Id** do elemento [ItemId](itemid.md) foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3ff34-120">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="3ff34-121">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff34-121">Request elements</span></span>

<span data-ttu-id="3ff34-122">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="3ff34-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="3ff34-123">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="3ff34-123">SyncFolderItems</span></span>](syncfolderitems.md)
    
- [<span data-ttu-id="3ff34-124">ItemShape</span><span class="sxs-lookup"><span data-stu-id="3ff34-124">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="3ff34-125">BaseShape</span><span class="sxs-lookup"><span data-stu-id="3ff34-125">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="3ff34-126">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="3ff34-126">SyncFolderId</span></span>](syncfolderid.md)
    
- [<span data-ttu-id="3ff34-127">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="3ff34-127">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="3ff34-128">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="3ff34-128">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="3ff34-129">Ignore</span><span class="sxs-lookup"><span data-stu-id="3ff34-129">Ignore</span></span>](ignore.md)
    
- [<span data-ttu-id="3ff34-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="3ff34-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="3ff34-131">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="3ff34-131">MaxChangesReturned</span></span>](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a><span data-ttu-id="3ff34-132">Resposta de SyncFolderItems bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="3ff34-132">Successful SyncFolderItems Response</span></span>

### <a name="description"></a><span data-ttu-id="3ff34-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff34-133">Description</span></span>

<span data-ttu-id="3ff34-134">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="3ff34-134">The following example shows a successful response to the SyncFolderItems request.</span></span> <span data-ttu-id="3ff34-135">Neste exemplo, uma solicitação de reunião é sincronizada da pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="3ff34-135">In this example, a meeting request is synchronized from the Sent Items folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="3ff34-136">Código</span><span class="sxs-lookup"><span data-stu-id="3ff34-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="3ff34-137">Comments</span><span class="sxs-lookup"><span data-stu-id="3ff34-137">Comments</span></span>

<span data-ttu-id="3ff34-138">Os dados de [estado de sincronização](syncstate-ex15websvcsotherref.md) do elemento codificado na base64 e o atributo de **Id** do elemento [ItemId](itemid.md) foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3ff34-138">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="3ff34-139">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="3ff34-139">Successful response elements</span></span>

<span data-ttu-id="3ff34-140">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="3ff34-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="3ff34-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3ff34-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3ff34-142">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="3ff34-142">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="3ff34-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3ff34-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3ff34-144">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3ff34-144">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="3ff34-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3ff34-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3ff34-146">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="3ff34-146">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="3ff34-147">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="3ff34-147">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
- [<span data-ttu-id="3ff34-148">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="3ff34-148">Changes (Items)</span></span>](changes-items.md)
    
- [<span data-ttu-id="3ff34-149">Criar (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="3ff34-149">Create (ItemSync)</span></span>](create-itemsync.md)
    
- [<span data-ttu-id="3ff34-150">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3ff34-150">MeetingRequest</span></span>](meetingrequest.md)
    
- [<span data-ttu-id="3ff34-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="3ff34-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="3ff34-152">Assunto</span><span class="sxs-lookup"><span data-stu-id="3ff34-152">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="3ff34-153">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="3ff34-153">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="3ff34-154">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="3ff34-154">IsOutOfDate</span></span>](isoutofdate.md)
    
- [<span data-ttu-id="3ff34-155">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="3ff34-155">HasBeenProcessed</span></span>](hasbeenprocessed.md)
    
- [<span data-ttu-id="3ff34-156">ResponseType</span><span class="sxs-lookup"><span data-stu-id="3ff34-156">ResponseType</span></span>](responsetype.md)
    
- [<span data-ttu-id="3ff34-157">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="3ff34-157">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md)
    
- [<span data-ttu-id="3ff34-158">Start</span><span class="sxs-lookup"><span data-stu-id="3ff34-158">Start</span></span>](start.md)
    
- [<span data-ttu-id="3ff34-159">End</span><span class="sxs-lookup"><span data-stu-id="3ff34-159">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="3ff34-160">Location</span><span class="sxs-lookup"><span data-stu-id="3ff34-160">Location</span></span>](location.md)
    
- [<span data-ttu-id="3ff34-161">Organizer</span><span class="sxs-lookup"><span data-stu-id="3ff34-161">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="3ff34-162">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="3ff34-162">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="3ff34-163">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3ff34-163">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="3ff34-164">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="3ff34-164">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="3ff34-165">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="3ff34-165">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a><span data-ttu-id="3ff34-166">Resposta de erro SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="3ff34-166">SyncFolderItems error response</span></span>

### <a name="description"></a><span data-ttu-id="3ff34-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff34-167">Description</span></span>

<span data-ttu-id="3ff34-168">O exemplo a seguir mostra uma resposta de erro a uma solicitação de SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="3ff34-168">The following example shows an error response to a SyncFolderItems request.</span></span> <span data-ttu-id="3ff34-169">Esse erro foi causado por um estado de sincronização inválido.</span><span class="sxs-lookup"><span data-stu-id="3ff34-169">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="3ff34-170">Código</span><span class="sxs-lookup"><span data-stu-id="3ff34-170">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="3ff34-171">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="3ff34-171">Error response elements</span></span>

<span data-ttu-id="3ff34-172">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="3ff34-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="3ff34-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3ff34-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3ff34-174">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="3ff34-174">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="3ff34-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3ff34-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3ff34-176">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3ff34-176">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="3ff34-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="3ff34-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3ff34-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3ff34-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3ff34-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3ff34-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="3ff34-180">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="3ff34-180">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="3ff34-181">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="3ff34-181">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
## <a name="see-also"></a><span data-ttu-id="3ff34-182">Confira também</span><span class="sxs-lookup"><span data-stu-id="3ff34-182">See also</span></span>



- [<span data-ttu-id="3ff34-183">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3ff34-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

