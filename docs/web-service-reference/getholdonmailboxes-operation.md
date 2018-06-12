---
title: Operação GetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Encontre informações sobre o EWS GetHoldOnMailboxes operação.
ms.openlocfilehash: 1d0bc2f9d26e11d8d2710693d67843ad2f339a5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752516"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="b206a-103">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-103">GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="b206a-104">Encontre informações sobre a operação de EWS **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b206a-104">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="b206a-105">A operação **GetHoldOnMailboxes** obtém as caixas de correio que estão em uma isenção específica e o associado mantenha a consulta.</span><span class="sxs-lookup"><span data-stu-id="b206a-105">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="b206a-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b206a-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="b206a-107">Usando a operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-107">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="b206a-108">A operação **GetHoldOnMailboxes** fornece as informações de cliente sobre quais as caixas de correio são colocadas em uma isenção específica, informações sobre a consulta de espera associada a cada isenção, se aplicável e informações sobre o status de retenção para cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b206a-108">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="b206a-109">Para obter mais informações sobre isenções de caixa de correio, incluindo isenções baseado em consulta, consulte [Bloqueio In-loco](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) no TechNet.</span><span class="sxs-lookup"><span data-stu-id="b206a-109">For more information about mailbox holds, including query-based holds, see [In-Place Hold](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="b206a-110">Cabeçalhos SOAP GetHoldOnMailboxes operação</span><span class="sxs-lookup"><span data-stu-id="b206a-110">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="b206a-111">A operação **GetHoldOnMailboxes** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b206a-111">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b206a-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="b206a-112">**Header name**</span></span>|<span data-ttu-id="b206a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b206a-113">**Element**</span></span>|<span data-ttu-id="b206a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b206a-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b206a-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="b206a-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="b206a-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="b206a-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="b206a-117">Identifica as funções de servidor necessários para que o chamador para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b206a-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="b206a-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b206a-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b206a-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b206a-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b206a-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b206a-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b206a-121">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="b206a-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b206a-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b206a-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b206a-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b206a-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b206a-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b206a-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b206a-125">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="b206a-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b206a-126">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b206a-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="b206a-127">Exemplo de solicitação de operação GetHoldOnMailboxes: obter informações de espera de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="b206a-127">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="b206a-128">O exemplo a seguir de uma solicitação de operação **GetHoldOnMailboxes** mostra como obter as informações de espera de caixa de correio para a retenção de caixa de correio HoldId2.</span><span class="sxs-lookup"><span data-stu-id="b206a-128">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetHoldOnMailboxes>
         <m:HoldId>HoldId2</m:HoldId>
      </m:GetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="b206a-129">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b206a-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b206a-130">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-130">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="b206a-131">HoldId</span><span class="sxs-lookup"><span data-stu-id="b206a-131">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="b206a-132">Resposta de operação GetHoldOnMailboxes bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b206a-132">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="b206a-133">O exemplo a seguir mostra uma resposta bem-sucedida a uma operação **GetHoldOnMailboxes** solicitação para obter a caixa de correio mantenha informações para a retenção de caixa de correio HoldId2.</span><span class="sxs-lookup"><span data-stu-id="b206a-133">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=ecc0fd98c2cadf-Willi</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=dasdat341q8de95-Micha</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b206a-134">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b206a-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b206a-135">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="b206a-135">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="b206a-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b206a-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b206a-137">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="b206a-137">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="b206a-138">HoldId</span><span class="sxs-lookup"><span data-stu-id="b206a-138">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="b206a-139">Query</span><span class="sxs-lookup"><span data-stu-id="b206a-139">Query</span></span>](query.md)
    
- [<span data-ttu-id="b206a-140">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="b206a-140">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="b206a-141">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="b206a-141">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="b206a-142">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="b206a-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="b206a-143">Status (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="b206a-143">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="b206a-144">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="b206a-144">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="b206a-145">Resposta de erro de operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-145">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="b206a-146">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b206a-146">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="b206a-147">Esta é uma resposta a uma solicitação para fazer uma pausa que tenha sido excluída.</span><span class="sxs-lookup"><span data-stu-id="b206a-147">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b206a-148">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b206a-148">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b206a-149">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="b206a-149">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="b206a-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="b206a-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b206a-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b206a-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b206a-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b206a-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b206a-153">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b206a-153">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b206a-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="b206a-154">See also</span></span>

- [<span data-ttu-id="b206a-155">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b206a-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="b206a-156">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-156">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="b206a-157">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-157">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="b206a-158">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b206a-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="b206a-159">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b206a-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="b206a-160">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="b206a-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="b206a-161">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="b206a-161">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

