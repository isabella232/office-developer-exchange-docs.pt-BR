---
title: Operação GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ed077877-9d98-4434-b8b6-a4a905e7f7a6
description: Encontre informações sobre a operação do EWS do GetNonIndexableItemStatistics.
ms.openlocfilehash: c7d49f9e0d7b4191c7403cb4d1a20e70a96c3882
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452815"
---
# <a name="getnonindexableitemstatistics-operation"></a><span data-ttu-id="8b638-103">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8b638-103">GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="8b638-104">Encontre informações sobre a operação do EWS do **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="8b638-104">Find information about the **GetNonIndexableItemStatistics** EWS operation.</span></span> 
  
<span data-ttu-id="8b638-105">A operação **GetNonIndexableItemStatistics** recupera a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8b638-105">The **GetNonIndexableItemStatistics** operation retrieves the count of items that cannot be indexed in a mailbox.</span></span> 
  
<span data-ttu-id="8b638-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8b638-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemstatistics-operation"></a><span data-ttu-id="8b638-107">Usando a operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8b638-107">Using the GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="8b638-108">A operação **GetNonIndexableItemStatistics** conta os itens de caixa de correio que não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="8b638-108">The **GetNonIndexableItemStatistics** operation counts mailbox items that cannot be indexed.</span></span> <span data-ttu-id="8b638-109">Os itens que não podem ser indexados não são pesquisados durante uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="8b638-109">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemstatistics-operation-soap-headers"></a><span data-ttu-id="8b638-110">Cabeçalhos SOAP de operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8b638-110">GetNonIndexableItemStatistics operation SOAP headers</span></span>

<span data-ttu-id="8b638-111">A operação **GetNonIndexableItemStatistics** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8b638-111">The **GetNonIndexableItemStatistics** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="8b638-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="8b638-112">**Header name**</span></span>|<span data-ttu-id="8b638-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b638-113">**Element**</span></span>|<span data-ttu-id="8b638-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b638-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8b638-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="8b638-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="8b638-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="8b638-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="8b638-117">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b638-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="8b638-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b638-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8b638-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="8b638-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="8b638-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="8b638-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="8b638-121">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="8b638-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="8b638-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b638-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8b638-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="8b638-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="8b638-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8b638-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8b638-125">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b638-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="8b638-126">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8b638-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemstatistics-operation-request-example-get-the-count-of-items-that-cannot-be-indexed-in-a-mailbox"></a><span data-ttu-id="8b638-127">Exemplo de solicitação de operação GetNonIndexableItemStatistics: obter a contagem de itens que não podem ser indexados em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="8b638-127">GetNonIndexableItemStatistics operation request example: Get the count of items that cannot be indexed in a mailbox</span></span>

<span data-ttu-id="8b638-128">O exemplo a seguir de uma solicitação de operação **GetNonIndexableItemStatistics** mostra como solicitar a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8b638-128">The following example of a **GetNonIndexableItemStatistics** operation request shows how to request the count of items that cannot be indexed in a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8b638-129">Todos os nomes de domínio herdados neste exemplo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b638-129">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemStatistics>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIDLT)/cn=Recipients/cn=3518cf-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemStatistics>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="8b638-130">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="8b638-130">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8b638-131">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8b638-131">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    
- [<span data-ttu-id="8b638-132">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="8b638-132">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="8b638-133">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="8b638-133">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="8b638-134">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="8b638-134">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemstatistics-operation-response"></a><span data-ttu-id="8b638-135">Resposta de operação GetNonIndexableItemStatistics bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="8b638-135">Successful GetNonIndexableItemStatistics operation response</span></span>

<span data-ttu-id="8b638-136">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetNonIndexableItemStatistics** para obter a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8b638-136">The following example shows a successful response to a **GetNonIndexableItemStatistics** operation request to get the count of items that cannot be indexed in a mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Success" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemStatistics>
            <NonIndexableItemStatistic xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35181acf-Steve</Mailbox>
               <ItemCount>2</ItemCount>
            </NonIndexableItemStatistic>
         </NonIndexableItemStatistics>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="8b638-137">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="8b638-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8b638-138">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="8b638-138">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="8b638-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8b638-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8b638-140">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8b638-140">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
    
- [<span data-ttu-id="8b638-141">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="8b638-141">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
    
- [<span data-ttu-id="8b638-142">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="8b638-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="8b638-143">ItemCount</span><span class="sxs-lookup"><span data-stu-id="8b638-143">ItemCount</span></span>](itemcount.md)
    
## <a name="getnonindexableitemstatistics-operation-error-response"></a><span data-ttu-id="8b638-144">Resposta de erro de operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8b638-144">GetNonIndexableItemStatistics operation error response</span></span>

<span data-ttu-id="8b638-145">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="8b638-145">The following example shows an error response to a **GetNonIndexableItemStatistics** operation request.</span></span> <span data-ttu-id="8b638-146">Esta é uma resposta a uma solicitação para obter a contagem de itens que não podem ser indexados de mais de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8b638-146">This is a response to a request to get the count of items that cannot be indexed from more than one mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Error" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="8b638-147">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="8b638-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8b638-148">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="8b638-148">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="8b638-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="8b638-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8b638-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8b638-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8b638-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8b638-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="8b638-152">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="8b638-152">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8b638-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="8b638-153">See also</span></span>

- [<span data-ttu-id="8b638-154">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8b638-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="8b638-155">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="8b638-155">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="8b638-156">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="8b638-156">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="8b638-157">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8b638-157">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="8b638-158">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8b638-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="8b638-159">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b638-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="8b638-160">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="8b638-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    

