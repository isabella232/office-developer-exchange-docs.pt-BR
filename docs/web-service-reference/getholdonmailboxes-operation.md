---
title: Operação GetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Encontre informações sobre a operação do EWS do GetHoldOnMailboxes.
ms.openlocfilehash: 867f38be87e60af8708eeb0b9d0e3ac8eee6ff64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457729"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="dcdad-103">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-103">GetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dcdad-104">A partir de 1º de abril de 2020, a operação GetHoldOnMailboxes não estará mais disponível no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="dcdad-104">Starting on April 1, 2020, the GetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="dcdad-105">Essa operação não será afetada nas versões locais do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="dcdad-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="dcdad-106">Para obter mais informações, consulte [aposentadoria of Legacy eDiscovery Tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="dcdad-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="dcdad-107">Encontre informações sobre a operação do EWS do **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="dcdad-107">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="dcdad-108">A operação **GetHoldOnMailboxes** Obtém as caixas de correio que estão sob uma retenção específica e a consulta de bloqueio associada.</span><span class="sxs-lookup"><span data-stu-id="dcdad-108">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="dcdad-109">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dcdad-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="dcdad-110">Usando a operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-110">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="dcdad-111">A operação **GetHoldOnMailboxes** fornece as informações de cliente sobre quais caixas de correio são colocadas em uma retenção específica, informações sobre a consulta de retenção associada a cada isenção, se aplicável, e informações sobre o status de retenção para cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="dcdad-111">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="dcdad-112">Para obter mais informações sobre retenções de caixa de correio, incluindo bloqueios baseados em consulta, consulte [in-Place Hold in in-loco](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) do TechNet.</span><span class="sxs-lookup"><span data-stu-id="dcdad-112">For more information about mailbox holds, including query-based holds, see [In-Place Hold](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="dcdad-113">Cabeçalhos SOAP de operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-113">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="dcdad-114">A operação **GetHoldOnMailboxes** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="dcdad-114">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="dcdad-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="dcdad-115">**Header name**</span></span>|<span data-ttu-id="dcdad-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dcdad-116">**Element**</span></span>|<span data-ttu-id="dcdad-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dcdad-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dcdad-118">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="dcdad-118">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="dcdad-119">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="dcdad-119">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="dcdad-120">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcdad-120">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="dcdad-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcdad-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="dcdad-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="dcdad-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="dcdad-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="dcdad-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="dcdad-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="dcdad-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="dcdad-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcdad-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="dcdad-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="dcdad-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="dcdad-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="dcdad-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="dcdad-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcdad-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="dcdad-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="dcdad-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="dcdad-130">Exemplo de solicitação de operação GetHoldOnMailboxes: obter informações de retenção de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="dcdad-130">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="dcdad-131">O exemplo a seguir de uma solicitação de operação **GetHoldOnMailboxes** mostra como obter as informações de retenção de caixa de correio para o bloqueio de caixa de correio do HoldId2.</span><span class="sxs-lookup"><span data-stu-id="dcdad-131">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="dcdad-132">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="dcdad-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dcdad-133">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-133">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="dcdad-134">Isenção</span><span class="sxs-lookup"><span data-stu-id="dcdad-134">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="dcdad-135">Resposta de operação GetHoldOnMailboxes bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="dcdad-135">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="dcdad-136">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetHoldOnMailboxes** para obter as informações de retenção de caixa de correio para o bloqueio de caixa de correio do HoldId2.</span><span class="sxs-lookup"><span data-stu-id="dcdad-136">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="dcdad-137">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="dcdad-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dcdad-138">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="dcdad-138">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="dcdad-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dcdad-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dcdad-140">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="dcdad-140">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="dcdad-141">Isenção</span><span class="sxs-lookup"><span data-stu-id="dcdad-141">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="dcdad-142">Query</span><span class="sxs-lookup"><span data-stu-id="dcdad-142">Query</span></span>](query.md)
    
- [<span data-ttu-id="dcdad-143">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="dcdad-143">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="dcdad-144">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="dcdad-144">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="dcdad-145">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="dcdad-145">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="dcdad-146">Status (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="dcdad-146">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="dcdad-147">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="dcdad-147">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="dcdad-148">Resposta de erro de operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-148">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="dcdad-149">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="dcdad-149">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="dcdad-150">Esta é uma resposta a uma solicitação para obter uma retenção que foi excluída.</span><span class="sxs-lookup"><span data-stu-id="dcdad-150">This is a response to a request to get a hold that has been deleted.</span></span> 
  
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
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="dcdad-151">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="dcdad-151">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dcdad-152">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="dcdad-152">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="dcdad-153">MessageText</span><span class="sxs-lookup"><span data-stu-id="dcdad-153">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="dcdad-154">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dcdad-154">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dcdad-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dcdad-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="dcdad-156">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="dcdad-156">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="dcdad-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="dcdad-157">See also</span></span>

- [<span data-ttu-id="dcdad-158">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dcdad-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="dcdad-159">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-159">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="dcdad-160">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-160">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="dcdad-161">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="dcdad-161">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="dcdad-162">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="dcdad-162">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="dcdad-163">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="dcdad-163">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="dcdad-164">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="dcdad-164">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

