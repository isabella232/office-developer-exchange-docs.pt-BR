---
title: Operação GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Encontre informações sobre o EWS GetSearchableMailboxes operação.
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752620"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="c2300-103">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-103">GetSearchableMailboxes operation</span></span>

<span data-ttu-id="c2300-104">Encontre informações sobre a operação de EWS **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="c2300-104">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="c2300-105">A operação **GetSearchableMailboxes** obtém um conjunto com escopo de caixas de correio pesquisáveis para pesquisas de descoberta.</span><span class="sxs-lookup"><span data-stu-id="c2300-105">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="c2300-106">O escopo de caixas de correio pesquisáveis retornados na resposta é determinado pelo filtro de pesquisa e se a associação de grupo de distribuição é expandida.</span><span class="sxs-lookup"><span data-stu-id="c2300-106">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 
  
<span data-ttu-id="c2300-107">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c2300-107">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="c2300-108">Usando a operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-108">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="c2300-109">A operação **GetSearchableMailboxes** obtém informações sobre caixas de correio pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="c2300-109">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="c2300-110">Os seguintes argumentos podem ser passados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="c2300-110">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="c2300-111">[SearchFilter](searchfilter.md) — aceita um alias de email único como um argumento.</span><span class="sxs-lookup"><span data-stu-id="c2300-111">[SearchFilter](searchfilter.md) —Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="c2300-112">[ExpandGroupMembership](expandgroupmembership.md) — indica se a associação ao grupo de distribuição é expandida nos resultados retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="c2300-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="c2300-113">Se o alias de email definido no filtro de pesquisa é um grupo de distribuição e a associação ao grupo de distribuição não estiver expandida, a resposta conterá as informações de caixa de correio para o grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c2300-113">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="c2300-114">Se o alias de email definido no filtro de pesquisa é um grupo de distribuição e a associação ao grupo de distribuição é expandida, a resposta conterá as informações de caixa de correio para cada caixa de correio que seja membro do grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c2300-114">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="c2300-115">Se o filtro de pesquisa contiver um alias de um único usuário, a resposta conterá as informações de caixa de correio para o usuário único.</span><span class="sxs-lookup"><span data-stu-id="c2300-115">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="c2300-116">A resposta conterá todas as caixas de correio pesquisáveis se o elemento [GetSearchableMailboxes](getsearchablemailboxes.md) está vazio.</span><span class="sxs-lookup"><span data-stu-id="c2300-116">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="c2300-117">Isso é o mesmo como tendo um elemento [SearchFilter](searchfilter.md) vazio e o elemento [ExpandGroupMembership](expandgroupmembership.md) definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="c2300-117">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="c2300-118">Cabeçalhos SOAP GetSearchableMailboxes operação</span><span class="sxs-lookup"><span data-stu-id="c2300-118">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="c2300-119">A operação **GetSearchableMailboxes** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c2300-119">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c2300-120">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="c2300-120">**Header name**</span></span>|<span data-ttu-id="c2300-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2300-121">**Element**</span></span>|<span data-ttu-id="c2300-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2300-122">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c2300-123">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="c2300-123">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="c2300-124">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="c2300-124">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="c2300-125">Identifica as funções de servidor necessários para que o chamador para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2300-125">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="c2300-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2300-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c2300-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c2300-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c2300-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c2300-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c2300-129">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="c2300-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c2300-130">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2300-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c2300-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c2300-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c2300-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c2300-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c2300-133">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2300-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c2300-134">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c2300-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="c2300-135">Exemplo de solicitação de operação GetSearchableMailboxes: solicitar informações sobre um grupo de distribuição</span><span class="sxs-lookup"><span data-stu-id="c2300-135">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="c2300-136">O exemplo a seguir de uma solicitação de operação **GetSearchableMailboxes** mostra como obter as informações de caixa de correio para o grupo de distribuição de lolgroup.</span><span class="sxs-lookup"><span data-stu-id="c2300-136">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="c2300-137">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c2300-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2300-138">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-138">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="c2300-139">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="c2300-139">SearchFilter</span></span>](searchfilter.md)
    
- [<span data-ttu-id="c2300-140">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="c2300-140">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="c2300-141">Resposta bem-sucedida de operação GetSearchableMailboxes: obter informações sobre um grupo de distribuição</span><span class="sxs-lookup"><span data-stu-id="c2300-141">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="c2300-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta para o grupo de distribuição de lolgroup.</span><span class="sxs-lookup"><span data-stu-id="c2300-142">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="c2300-143">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c2300-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2300-144">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="c2300-144">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="c2300-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2300-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c2300-146">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-146">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="c2300-147">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="c2300-147">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="c2300-148">GUID</span><span class="sxs-lookup"><span data-stu-id="c2300-148">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c2300-149">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c2300-149">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="c2300-150">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="c2300-150">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="c2300-151">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c2300-151">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="c2300-152">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="c2300-152">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="c2300-153">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="c2300-153">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="c2300-154">ID de referência</span><span class="sxs-lookup"><span data-stu-id="c2300-154">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="c2300-155">Resposta bem-sucedida de operação GetSearchableMailboxes: obter informações sobre um grupo de distribuição expandido</span><span class="sxs-lookup"><span data-stu-id="c2300-155">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="c2300-156">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta sobre membros do grupo de distribuição expandido lolgroup.</span><span class="sxs-lookup"><span data-stu-id="c2300-156">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="c2300-157">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c2300-157">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2300-158">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="c2300-158">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="c2300-159">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2300-159">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c2300-160">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-160">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="c2300-161">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="c2300-161">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="c2300-162">GUID</span><span class="sxs-lookup"><span data-stu-id="c2300-162">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c2300-163">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c2300-163">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="c2300-164">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="c2300-164">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="c2300-165">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c2300-165">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="c2300-166">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="c2300-166">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="c2300-167">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="c2300-167">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="c2300-168">ID de referência</span><span class="sxs-lookup"><span data-stu-id="c2300-168">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="c2300-169">Resposta de erro de operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-169">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="c2300-170">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="c2300-170">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="c2300-171">Esta é uma resposta a uma solicitação para obter todas as caixas de correio pesquisáveis quando o argumento **ExpandGroupMembership** estiver definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="c2300-171">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="c2300-172">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c2300-172">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c2300-173">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="c2300-173">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="c2300-174">MessageText</span><span class="sxs-lookup"><span data-stu-id="c2300-174">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c2300-175">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2300-175">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c2300-176">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c2300-176">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c2300-177">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-177">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="c2300-178">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="c2300-178">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c2300-179">Confira também</span><span class="sxs-lookup"><span data-stu-id="c2300-179">See also</span></span>

- [<span data-ttu-id="c2300-180">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c2300-180">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="c2300-181">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-181">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="c2300-182">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-182">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="c2300-183">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c2300-183">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="c2300-184">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2300-184">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="c2300-185">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="c2300-185">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="c2300-186">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="c2300-186">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

