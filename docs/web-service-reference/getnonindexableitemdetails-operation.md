---
title: Operação GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Encontre informações sobre a operação do EWS do GetNonIndexableItemDetails.
ms.openlocfilehash: a443e04b0622ddbaaeb1bc8c04bfd05679c6207e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530208"
---
# <a name="getnonindexableitemdetails-operation"></a><span data-ttu-id="35f00-103">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="35f00-103">GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="35f00-104">Encontre informações sobre a operação do EWS do **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="35f00-104">Find information about the **GetNonIndexableItemDetails** EWS operation.</span></span> 
  
<span data-ttu-id="35f00-105">A operação **GetNonIndexableItemDetails** recupera os detalhes sobre os itens que não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="35f00-105">The **GetNonIndexableItemDetails** operation retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="35f00-106">Isso inclui, mas não está limitado a, o identificador de item, um código de erro, uma descrição de erro, quando uma tentativa é feita para indexar o item e informações adicionais sobre o arquivo.</span><span class="sxs-lookup"><span data-stu-id="35f00-106">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="35f00-107">Embora o esquema indique que mais de uma caixa de correio pode ser pesquisada, na versão inicial do Exchange 2013, o serviço só oferece suporte para obter detalhes do item para itens não indexados em uma única caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="35f00-107">Although the schema indicates that more than one mailbox can be searched, in the initial release version of Exchange 2013, the service only supports getting item details for nonindexable items in a single mailbox.</span></span> 
  
<span data-ttu-id="35f00-108">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="35f00-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemdetails-operation"></a><span data-ttu-id="35f00-109">Usando a operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="35f00-109">Using the GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="35f00-110">A operação **GetNonIndexableItemDetails** identifica itens de caixa de correio que não podem ser indexados e fornece informações sobre o motivo pelo qual os itens não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="35f00-110">The **GetNonIndexableItemDetails** operation identifies mailbox items that cannot be indexed and provides information about why the items cannot be indexed.</span></span> <span data-ttu-id="35f00-111">Os itens que não podem ser indexados não são pesquisados durante uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="35f00-111">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a><span data-ttu-id="35f00-112">Cabeçalhos SOAP de operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="35f00-112">GetNonIndexableItemDetails operation SOAP headers</span></span>

<span data-ttu-id="35f00-113">A operação **GetNonIndexableItemDetails** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="35f00-113">The **GetNonIndexableItemDetails** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="35f00-114">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="35f00-114">**Header name**</span></span>|<span data-ttu-id="35f00-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="35f00-115">**Element**</span></span>|<span data-ttu-id="35f00-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="35f00-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="35f00-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="35f00-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="35f00-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="35f00-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="35f00-119">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="35f00-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="35f00-120">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="35f00-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="35f00-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="35f00-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="35f00-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="35f00-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="35f00-123">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="35f00-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="35f00-124">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="35f00-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="35f00-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="35f00-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="35f00-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="35f00-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="35f00-127">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="35f00-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="35f00-128">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="35f00-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a><span data-ttu-id="35f00-129">Exemplo de solicitação de operação GetNonIndexableItemDetails: obter os detalhes de um item que não pode ser indexado</span><span class="sxs-lookup"><span data-stu-id="35f00-129">GetNonIndexableItemDetails operation request example: Get the details of an item that cannot be indexed</span></span>

<span data-ttu-id="35f00-130">O exemplo a seguir de uma solicitação de operação **GetNonIndexableItemDetails** mostra como solicitar os detalhes de itens que não podem ser indexados para uma única caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="35f00-130">The following example of a **GetNonIndexableItemDetails** operation request shows how to request the details for items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="35f00-131">A pesquisa é realizada nas caixas de correio primárias e de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="35f00-131">The search is performed across both primary and archive mailboxes.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="35f00-132">Todos os nomes de domínio herdados neste exemplo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="35f00-132">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="35f00-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="35f00-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="35f00-134">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="35f00-134">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="35f00-135">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="35f00-135">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="35f00-136">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="35f00-136">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="35f00-137">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="35f00-137">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a><span data-ttu-id="35f00-138">Resposta de operação GetNonIndexableItemDetails bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="35f00-138">Successful GetNonIndexableItemDetails operation response</span></span>

<span data-ttu-id="35f00-139">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetNonIndexableItemDetails** para obter itens que não podem ser indexados para uma única caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="35f00-139">The following example shows a successful response to a **GetNonIndexableItemDetails** operation request to get items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="35f00-140">O item neste exemplo que não pode ser indexado é o arquivo binaryfile. ABC, que é de um formato desconhecido.</span><span class="sxs-lookup"><span data-stu-id="35f00-140">The item in this example that cannot be indexed is the binaryfile.abc file, which is of an unknown format.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="35f00-141">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="35f00-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="35f00-142">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="35f00-142">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="35f00-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="35f00-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="35f00-144">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="35f00-144">NonIndexableItemDetailsResult</span></span>](nonindexableitemdetailsresult.md)
    
- [<span data-ttu-id="35f00-145">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="35f00-145">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
    
- [<span data-ttu-id="35f00-146">ItemId</span><span class="sxs-lookup"><span data-stu-id="35f00-146">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="35f00-147">ErrorCode (ItemIndexErrorType)</span><span class="sxs-lookup"><span data-stu-id="35f00-147">ErrorCode (ItemIndexErrorType)</span></span>](errorcode-itemindexerrortype.md)
    
- [<span data-ttu-id="35f00-148">ErrorDescription</span><span class="sxs-lookup"><span data-stu-id="35f00-148">ErrorDescription</span></span>](errordescription.md)
    
- [<span data-ttu-id="35f00-149">IsPartiallyIndexed</span><span class="sxs-lookup"><span data-stu-id="35f00-149">IsPartiallyIndexed</span></span>](ispartiallyindexed.md)
    
- [<span data-ttu-id="35f00-150">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="35f00-150">IsPermanentFailure</span></span>](ispermanentfailure.md)
    
- [<span data-ttu-id="35f00-151">Sortvalue</span><span class="sxs-lookup"><span data-stu-id="35f00-151">SortValue</span></span>](sortvalue.md)
    
- [<span data-ttu-id="35f00-152">AttemptCount</span><span class="sxs-lookup"><span data-stu-id="35f00-152">AttemptCount</span></span>](attemptcount.md)
    
- [<span data-ttu-id="35f00-153">LastAttemptTime</span><span class="sxs-lookup"><span data-stu-id="35f00-153">LastAttemptTime</span></span>](lastattempttime.md)
    
- [<span data-ttu-id="35f00-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="35f00-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a><span data-ttu-id="35f00-155">Resposta de erro de operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="35f00-155">GetNonIndexableItemDetails operation error response</span></span>

<span data-ttu-id="35f00-156">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="35f00-156">The following example shows an error response to a **GetNonIndexableItemDetails** operation request.</span></span> <span data-ttu-id="35f00-157">Esta é uma resposta a uma solicitação para obter detalhes do item para itens que não podem ser indexados de mais de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="35f00-157">This is a response to a request to get item details for items that cannot be indexed from more than one mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="35f00-158">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="35f00-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="35f00-159">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="35f00-159">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="35f00-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="35f00-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="35f00-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="35f00-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="35f00-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="35f00-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="35f00-163">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="35f00-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="35f00-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="35f00-164">See also</span></span>

- [<span data-ttu-id="35f00-165">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="35f00-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="35f00-166">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="35f00-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="35f00-167">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="35f00-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="35f00-168">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="35f00-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="35f00-169">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="35f00-169">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="35f00-170">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="35f00-170">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="35f00-171">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="35f00-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

