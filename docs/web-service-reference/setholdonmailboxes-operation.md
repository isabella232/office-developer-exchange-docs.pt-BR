---
title: Operação SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Encontre informações sobre o EWS SetHoldOnMailboxes operação.
ms.openlocfilehash: 1091ed14ceb25dfd275499b9db47ae4e41b5f1a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825412"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="b059b-103">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-103">SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="b059b-104">Encontre informações sobre a operação de EWS **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b059b-104">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="b059b-105">A operação **SetHoldOnMailboxes** define uma política de retenção de caixa de correio em caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="b059b-105">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="b059b-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b059b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="b059b-107">Usando a operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-107">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="b059b-108">A operação de **SetHoldOnMailboxes** define uma isenção de caixa de correio em uma ou mais caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="b059b-108">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="b059b-109">Cabeçalhos SOAP SetHoldOnMailboxes operação</span><span class="sxs-lookup"><span data-stu-id="b059b-109">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="b059b-110">A operação **SetHoldOnMailboxes** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b059b-110">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b059b-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="b059b-111">**Header name**</span></span>|<span data-ttu-id="b059b-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b059b-112">**Element**</span></span>|<span data-ttu-id="b059b-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b059b-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b059b-114">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="b059b-114">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="b059b-115">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="b059b-115">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="b059b-116">Identifica as funções de servidor necessários para que o chamador para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b059b-116">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="b059b-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b059b-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b059b-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b059b-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b059b-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b059b-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b059b-120">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="b059b-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b059b-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b059b-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b059b-122">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b059b-122">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b059b-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b059b-123">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b059b-124">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="b059b-124">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b059b-125">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b059b-125">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="b059b-126">Exemplo de solicitação de operação SetHoldOnMailboxes: aplicar uma retenção em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="b059b-126">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="b059b-127">O exemplo a seguir de uma solicitação de operação **SetHoldOnMailboxes** mostra como aplicar uma retenção em duas caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="b059b-127">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="b059b-128">A retenção de caixa de correio foi criada usando o comando [New-MailboxSearch](http://technet.microsoft.com/pt-br/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b059b-128">The mailbox hold was created by using the [New-MailboxSearch](http://technet.microsoft.com/pt-br/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="b059b-129">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b059b-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b059b-130">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-130">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="b059b-131">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="b059b-131">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="b059b-132">HoldId</span><span class="sxs-lookup"><span data-stu-id="b059b-132">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="b059b-133">Query</span><span class="sxs-lookup"><span data-stu-id="b059b-133">Query</span></span>](query.md)
    
- [<span data-ttu-id="b059b-134">Caixas de correio (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="b059b-134">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="b059b-135">String</span><span class="sxs-lookup"><span data-stu-id="b059b-135">String</span></span>](string.md)
    
- [<span data-ttu-id="b059b-136">Idioma</span><span class="sxs-lookup"><span data-stu-id="b059b-136">Language</span></span>](language.md)
    
- [<span data-ttu-id="b059b-137">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="b059b-137">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="b059b-138">Eliminação da duplicação</span><span class="sxs-lookup"><span data-stu-id="b059b-138">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="b059b-139">Resposta de operação SetHoldOnMailboxes bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b059b-139">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="b059b-140">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SetHoldOnMailboxes** para colocar as duas caixas de correio em espera.</span><span class="sxs-lookup"><span data-stu-id="b059b-140">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b059b-141">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b059b-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b059b-142">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="b059b-142">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="b059b-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b059b-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b059b-144">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="b059b-144">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="b059b-145">HoldId</span><span class="sxs-lookup"><span data-stu-id="b059b-145">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="b059b-146">Query</span><span class="sxs-lookup"><span data-stu-id="b059b-146">Query</span></span>](query.md)
    
- [<span data-ttu-id="b059b-147">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="b059b-147">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="b059b-148">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="b059b-148">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="b059b-149">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="b059b-149">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="b059b-150">Status (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="b059b-150">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="b059b-151">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="b059b-151">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="b059b-152">Resposta de erro de operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-152">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="b059b-153">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b059b-153">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="b059b-154">Esta é uma resposta a uma solicitação que contém um identificador de caixa de correio especificada incorretamente.</span><span class="sxs-lookup"><span data-stu-id="b059b-154">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="b059b-155">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b059b-155">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b059b-156">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="b059b-156">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="b059b-157">MessageText</span><span class="sxs-lookup"><span data-stu-id="b059b-157">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b059b-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b059b-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b059b-159">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b059b-159">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b059b-160">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b059b-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b059b-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="b059b-161">See also</span></span>

- [<span data-ttu-id="b059b-162">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b059b-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="b059b-163">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-163">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="b059b-164">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-164">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="b059b-165">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b059b-165">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="b059b-166">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b059b-166">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="b059b-167">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="b059b-167">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="b059b-168">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="b059b-168">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

