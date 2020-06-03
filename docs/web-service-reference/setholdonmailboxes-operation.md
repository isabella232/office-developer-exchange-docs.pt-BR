---
title: Operação SetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Encontre informações sobre a operação do EWS do SetHoldOnMailboxes.
ms.openlocfilehash: 4d79ba9f616974b9415ae9eae23b8f5fdb0ab205
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448391"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="a8e16-103">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-103">SetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a8e16-104">A partir de 1º de abril de 2020, a operação SetHoldOnMailboxes não estará mais disponível no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a8e16-104">Starting on April 1, 2020, the SetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="a8e16-105">Essa operação não será afetada nas versões locais do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a8e16-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="a8e16-106">Para obter mais informações, consulte [aposentadoria of Legacy eDiscovery Tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="a8e16-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="a8e16-107">Encontre informações sobre a operação do EWS do **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="a8e16-107">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="a8e16-108">A operação **SetHoldOnMailboxes** define uma política de retenção de caixa de correio em caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="a8e16-108">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="a8e16-109">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a8e16-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="a8e16-110">Usando a operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-110">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="a8e16-111">A operação **SetHoldOnMailboxes** define uma retenção de caixa de correio em uma ou mais caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="a8e16-111">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="a8e16-112">Cabeçalhos SOAP de operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-112">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="a8e16-113">A operação **SetHoldOnMailboxes** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8e16-113">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="a8e16-114">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="a8e16-114">**Header name**</span></span>|<span data-ttu-id="a8e16-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a8e16-115">**Element**</span></span>|<span data-ttu-id="a8e16-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a8e16-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a8e16-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="a8e16-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="a8e16-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="a8e16-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="a8e16-119">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e16-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="a8e16-120">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e16-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a8e16-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="a8e16-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a8e16-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a8e16-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a8e16-123">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="a8e16-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a8e16-124">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e16-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a8e16-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="a8e16-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a8e16-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a8e16-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a8e16-127">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8e16-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a8e16-128">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e16-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="a8e16-129">Exemplo de solicitação de operação SetHoldOnMailboxes: aplicar uma retenção em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="a8e16-129">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="a8e16-130">O exemplo a seguir de uma solicitação de operação **SetHoldOnMailboxes** mostra como aplicar uma retenção em duas caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="a8e16-130">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="a8e16-131">A retenção de caixa de correio foi criada usando o comando [New-MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a8e16-131">The mailbox hold was created by using the [New-MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="a8e16-132">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="a8e16-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a8e16-133">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-133">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="a8e16-134">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="a8e16-134">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="a8e16-135">Isenção</span><span class="sxs-lookup"><span data-stu-id="a8e16-135">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="a8e16-136">Query</span><span class="sxs-lookup"><span data-stu-id="a8e16-136">Query</span></span>](query.md)
    
- [<span data-ttu-id="a8e16-137">Caixas de correio (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="a8e16-137">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="a8e16-138">String</span><span class="sxs-lookup"><span data-stu-id="a8e16-138">String</span></span>](string.md)
    
- [<span data-ttu-id="a8e16-139">Language</span><span class="sxs-lookup"><span data-stu-id="a8e16-139">Language</span></span>](language.md)
    
- [<span data-ttu-id="a8e16-140">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="a8e16-140">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="a8e16-141">Duplicidades</span><span class="sxs-lookup"><span data-stu-id="a8e16-141">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="a8e16-142">Resposta de operação SetHoldOnMailboxes bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a8e16-142">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="a8e16-143">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SetHoldOnMailboxes** para colocar duas caixas de correio em espera.</span><span class="sxs-lookup"><span data-stu-id="a8e16-143">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="a8e16-144">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="a8e16-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a8e16-145">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="a8e16-145">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="a8e16-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8e16-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a8e16-147">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="a8e16-147">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="a8e16-148">Isenção</span><span class="sxs-lookup"><span data-stu-id="a8e16-148">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="a8e16-149">Query</span><span class="sxs-lookup"><span data-stu-id="a8e16-149">Query</span></span>](query.md)
    
- [<span data-ttu-id="a8e16-150">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="a8e16-150">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="a8e16-151">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="a8e16-151">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="a8e16-152">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="a8e16-152">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="a8e16-153">Status (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="a8e16-153">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="a8e16-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="a8e16-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="a8e16-155">Resposta de erro de operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-155">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="a8e16-156">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="a8e16-156">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="a8e16-157">Esta é uma resposta a uma solicitação que contém um identificador de caixa de correio especificado incorretamente.</span><span class="sxs-lookup"><span data-stu-id="a8e16-157">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="a8e16-158">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="a8e16-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a8e16-159">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="a8e16-159">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="a8e16-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="a8e16-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a8e16-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8e16-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a8e16-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a8e16-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="a8e16-163">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="a8e16-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a8e16-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="a8e16-164">See also</span></span>

- [<span data-ttu-id="a8e16-165">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a8e16-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="a8e16-166">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="a8e16-167">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="a8e16-168">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a8e16-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="a8e16-169">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e16-169">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="a8e16-170">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="a8e16-170">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="a8e16-171">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="a8e16-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

