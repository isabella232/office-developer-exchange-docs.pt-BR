---
title: Operação GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ed077877-9d98-4434-b8b6-a4a905e7f7a6
description: Encontre informações sobre o EWS GetNonIndexableItemStatistics operação.
ms.openlocfilehash: 35c2d3321c6e1a3154c88307d0e875cd6997e7fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752568"
---
# <a name="getnonindexableitemstatistics-operation"></a><span data-ttu-id="ff6e2-103">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="ff6e2-103">GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="ff6e2-104">Encontre informações sobre a operação de EWS **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="ff6e2-104">Find information about the **GetNonIndexableItemStatistics** EWS operation.</span></span> 
  
<span data-ttu-id="ff6e2-105">A operação **GetNonIndexableItemStatistics** recupera a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-105">The **GetNonIndexableItemStatistics** operation retrieves the count of items that cannot be indexed in a mailbox.</span></span> 
  
<span data-ttu-id="ff6e2-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemstatistics-operation"></a><span data-ttu-id="ff6e2-107">Usando a operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="ff6e2-107">Using the GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="ff6e2-108">A operação **GetNonIndexableItemStatistics** contagens de itens de caixa de correio que não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-108">The **GetNonIndexableItemStatistics** operation counts mailbox items that cannot be indexed.</span></span> <span data-ttu-id="ff6e2-109">Itens que não podem ser indexados não serão pesquisados durante uma pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-109">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemstatistics-operation-soap-headers"></a><span data-ttu-id="ff6e2-110">Cabeçalhos SOAP GetNonIndexableItemStatistics operação</span><span class="sxs-lookup"><span data-stu-id="ff6e2-110">GetNonIndexableItemStatistics operation SOAP headers</span></span>

<span data-ttu-id="ff6e2-111">A operação **GetNonIndexableItemStatistics** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-111">The **GetNonIndexableItemStatistics** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ff6e2-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-112">**Header name**</span></span>|<span data-ttu-id="ff6e2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-113">**Element**</span></span>|<span data-ttu-id="ff6e2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ff6e2-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="ff6e2-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="ff6e2-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="ff6e2-117">Identifica as funções de servidor necessários para que o chamador para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="ff6e2-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ff6e2-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ff6e2-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ff6e2-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ff6e2-121">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="ff6e2-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ff6e2-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ff6e2-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ff6e2-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ff6e2-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ff6e2-125">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ff6e2-126">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemstatistics-operation-request-example-get-the-count-of-items-that-cannot-be-indexed-in-a-mailbox"></a><span data-ttu-id="ff6e2-127">Exemplo de solicitação de operação GetNonIndexableItemStatistics: obter contagem de itens que não podem ser indexados em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="ff6e2-127">GetNonIndexableItemStatistics operation request example: Get the count of items that cannot be indexed in a mailbox</span></span>

<span data-ttu-id="ff6e2-128">O exemplo a seguir de uma solicitação de operação **GetNonIndexableItemStatistics** mostra como solicitar a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-128">The following example of a **GetNonIndexableItemStatistics** operation request shows how to request the count of items that cannot be indexed in a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ff6e2-129">Todos os nomes de domínio herdado neste exemplo ter ser reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-129">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="ff6e2-130">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="ff6e2-130">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ff6e2-131">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="ff6e2-131">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    
- [<span data-ttu-id="ff6e2-132">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="ff6e2-132">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="ff6e2-133">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="ff6e2-133">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="ff6e2-134">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="ff6e2-134">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemstatistics-operation-response"></a><span data-ttu-id="ff6e2-135">Resposta de operação GetNonIndexableItemStatistics bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ff6e2-135">Successful GetNonIndexableItemStatistics operation response</span></span>

<span data-ttu-id="ff6e2-136">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetNonIndexableItemStatistics** para obter a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-136">The following example shows a successful response to a **GetNonIndexableItemStatistics** operation request to get the count of items that cannot be indexed in a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0"
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemStatisticsResponse ResponseClass="Success" 
                                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemStatistics>
            <NonIndexableItemStatistic xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35181acf-Steve</Mailbox>
               <ItemCount>2</ItemCount>
            </NonIndexableItemStatistic>
         </NonIndexableItemStatistics>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="ff6e2-137">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="ff6e2-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ff6e2-138">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="ff6e2-138">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="ff6e2-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ff6e2-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ff6e2-140">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="ff6e2-140">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
    
- [<span data-ttu-id="ff6e2-141">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="ff6e2-141">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
    
- [<span data-ttu-id="ff6e2-142">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="ff6e2-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="ff6e2-143">ItemCount</span><span class="sxs-lookup"><span data-stu-id="ff6e2-143">ItemCount</span></span>](itemcount.md)
    
## <a name="getnonindexableitemstatistics-operation-error-response"></a><span data-ttu-id="ff6e2-144">Resposta de erro de operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="ff6e2-144">GetNonIndexableItemStatistics operation error response</span></span>

<span data-ttu-id="ff6e2-145">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="ff6e2-145">The following example shows an error response to a **GetNonIndexableItemStatistics** operation request.</span></span> <span data-ttu-id="ff6e2-146">Esta é uma resposta a uma solicitação para obter a contagem de itens que não podem ser indexados de mais de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ff6e2-146">This is a response to a request to get the count of items that cannot be indexed from more than one mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemStatisticsResponse ResponseClass="Error" 
                                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="ff6e2-147">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="ff6e2-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ff6e2-148">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="ff6e2-148">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="ff6e2-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="ff6e2-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ff6e2-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ff6e2-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ff6e2-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ff6e2-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="ff6e2-152">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="ff6e2-152">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ff6e2-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff6e2-153">See also</span></span>

- [<span data-ttu-id="ff6e2-154">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ff6e2-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="ff6e2-155">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff6e2-155">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="ff6e2-156">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff6e2-156">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="ff6e2-157">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff6e2-157">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="ff6e2-158">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ff6e2-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="ff6e2-159">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff6e2-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="ff6e2-160">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="ff6e2-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    

