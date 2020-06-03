---
title: Operação GetSearchableMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Encontre informações sobre a operação do EWS do GetSearchableMailboxes.
ms.openlocfilehash: e893a66eb1b638479eeccc6bd7548cb020f37243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530836"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="7f0a4-103">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-103">GetSearchableMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7f0a4-104">A partir de 1º de abril de 2020, a operação GetSearchableMailboxes não estará mais disponível no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-104">Starting on April 1, 2020, the GetSearchableMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="7f0a4-105">Essa operação não será afetada nas versões locais do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="7f0a4-106">Para obter mais informações, consulte [aposentadoria of Legacy eDiscovery Tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="7f0a4-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="7f0a4-107">Encontre informações sobre a operação do EWS do **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="7f0a4-107">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="7f0a4-108">A operação **GetSearchableMailboxes** Obtém um conjunto com escopo de caixas de correio pesquisáveis para pesquisas de descoberta.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-108">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="7f0a4-109">O escopo das caixas de correio que podem ser pesquisadas retornadas na resposta é determinado pelo filtro de pesquisa e se a associação do grupo de distribuição está expandida.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-109">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 

> [!NOTE] 
> <span data-ttu-id="7f0a4-110">Esta operação deve ser usada com o filtro de pesquisa e para recuperar apenas as primeiras milhares; Não se destina à recuperação exaustiva.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-110">This operation is intended to be used with the search filter and to retrieve only the first few thousands; it's not intended for exhaustive retrieval.</span></span>
  
<span data-ttu-id="7f0a4-111">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-111">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="7f0a4-112">Usando a operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-112">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="7f0a4-113">A operação **GetSearchableMailboxes** Obtém informações sobre caixas de correio pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-113">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="7f0a4-114">Os seguintes argumentos podem ser passados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="7f0a4-114">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="7f0a4-115">[SearchFilter](searchfilter.md) -aceita um único alias de email como um argumento.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-115">[SearchFilter](searchfilter.md) - Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="7f0a4-116">[ExpandGroupMembership](expandgroupmembership.md) -indica se a associação do grupo de distribuição está expandida nos resultados retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-116">[ExpandGroupMembership](expandgroupmembership.md) - Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="7f0a4-117">Se o alias de email definido no filtro de pesquisa for um grupo de distribuição e a associação do grupo de distribuição não for expandida, a resposta conterá as informações de caixa de correio para o grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-117">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="7f0a4-118">Se o alias de email definido no filtro de pesquisa for um grupo de distribuição e a associação do grupo de distribuição for expandida, a resposta conterá as informações de caixa de correio para cada caixa de correio que seja membro do grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-118">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="7f0a4-119">Se o filtro de pesquisa contiver um alias de usuário único, a resposta conterá as informações de caixa de correio para o único usuário.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-119">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="7f0a4-120">A resposta conterá todas as caixas de correio que poderão ser pesquisadas se o elemento [GetSearchableMailboxes](getsearchablemailboxes.md) estiver vazio.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-120">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="7f0a4-121">Isso é o mesmo que ter um elemento [SearchFilter](searchfilter.md) vazio e o elemento [ExpandGroupMembership](expandgroupmembership.md) definido como **false**.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-121">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="7f0a4-122">Cabeçalhos SOAP de operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-122">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="7f0a4-123">A operação **GetSearchableMailboxes** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-123">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7f0a4-124">Nome de cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f0a4-124">Header name</span></span>|<span data-ttu-id="7f0a4-125">Elemento</span><span class="sxs-lookup"><span data-stu-id="7f0a4-125">Element</span></span>|<span data-ttu-id="7f0a4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0a4-126">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7f0a4-127">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="7f0a4-127">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="7f0a4-128">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="7f0a4-128">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="7f0a4-129">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-129">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="7f0a4-130">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7f0a4-131">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7f0a4-131">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7f0a4-132">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7f0a4-132">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7f0a4-133">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-133">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7f0a4-134">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-134">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7f0a4-135">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7f0a4-135">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7f0a4-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7f0a4-136">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7f0a4-137">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-137">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7f0a4-138">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-138">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="7f0a4-139">Exemplo de solicitação de operação GetSearchableMailboxes: solicitar informações sobre um grupo de distribuição</span><span class="sxs-lookup"><span data-stu-id="7f0a4-139">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="7f0a4-140">O exemplo a seguir de uma solicitação de operação **GetSearchableMailboxes** mostra como obter as informações de caixa de correio para o grupo de distribuição lolgroup.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-140">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="7f0a4-141">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7f0a4-141">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7f0a4-142">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-142">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)   
- [<span data-ttu-id="7f0a4-143">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="7f0a4-143">SearchFilter</span></span>](searchfilter.md)    
- [<span data-ttu-id="7f0a4-144">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="7f0a4-144">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="7f0a4-145">Resposta de operação GetSearchableMailboxes bem-sucedida: obter informações sobre um grupo de distribuição</span><span class="sxs-lookup"><span data-stu-id="7f0a4-145">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="7f0a4-146">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta para o grupo de distribuição lolgroup.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-146">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="7f0a4-147">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7f0a4-147">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7f0a4-148">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="7f0a4-148">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)   
- [<span data-ttu-id="7f0a4-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f0a4-149">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="7f0a4-150">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-150">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="7f0a4-151">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="7f0a4-151">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="7f0a4-152">Guid</span><span class="sxs-lookup"><span data-stu-id="7f0a4-152">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="7f0a4-153">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7f0a4-153">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="7f0a4-154">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="7f0a4-154">IsExternalMailbox</span></span>](isexternalmailbox.md)   
- [<span data-ttu-id="7f0a4-155">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7f0a4-155">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="7f0a4-156">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7f0a4-156">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="7f0a4-157">Membro ismembership</span><span class="sxs-lookup"><span data-stu-id="7f0a4-157">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="7f0a4-158">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="7f0a4-158">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="7f0a4-159">Resposta de operação GetSearchableMailboxes bem-sucedida: obter informações sobre um grupo de distribuição expandido</span><span class="sxs-lookup"><span data-stu-id="7f0a4-159">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="7f0a4-160">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta sobre os membros do grupo de distribuição lolgroup expandido.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-160">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="7f0a4-161">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7f0a4-161">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7f0a4-162">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="7f0a4-162">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)    
- [<span data-ttu-id="7f0a4-163">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f0a4-163">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="7f0a4-164">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-164">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="7f0a4-165">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="7f0a4-165">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="7f0a4-166">Guid</span><span class="sxs-lookup"><span data-stu-id="7f0a4-166">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="7f0a4-167">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7f0a4-167">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="7f0a4-168">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="7f0a4-168">IsExternalMailbox</span></span>](isexternalmailbox.md)    
- [<span data-ttu-id="7f0a4-169">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7f0a4-169">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="7f0a4-170">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7f0a4-170">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="7f0a4-171">Membro ismembership</span><span class="sxs-lookup"><span data-stu-id="7f0a4-171">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="7f0a4-172">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="7f0a4-172">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="7f0a4-173">Resposta de erro de operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-173">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="7f0a4-174">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="7f0a4-174">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="7f0a4-175">Esta é uma resposta a uma solicitação para obter todas as caixas de correio pesquisáveis quando o argumento **ExpandGroupMembership** estiver definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="7f0a4-175">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="7f0a4-176">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7f0a4-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7f0a4-177">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="7f0a4-177">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)  
- [<span data-ttu-id="7f0a4-178">MessageText</span><span class="sxs-lookup"><span data-stu-id="7f0a4-178">MessageText</span></span>](messagetext.md)   
- [<span data-ttu-id="7f0a4-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f0a4-179">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="7f0a4-180">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7f0a4-180">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) 
- [<span data-ttu-id="7f0a4-181">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-181">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="7f0a4-182">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="7f0a4-182">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7f0a4-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="7f0a4-183">See also</span></span>

- [<span data-ttu-id="7f0a4-184">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7f0a4-184">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="7f0a4-185">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-185">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)   
- [<span data-ttu-id="7f0a4-186">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-186">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)   
- [<span data-ttu-id="7f0a4-187">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f0a4-187">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)    
- [<span data-ttu-id="7f0a4-188">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f0a4-188">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)   
- [<span data-ttu-id="7f0a4-189">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="7f0a4-189">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)   
- [<span data-ttu-id="7f0a4-190">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="7f0a4-190">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

