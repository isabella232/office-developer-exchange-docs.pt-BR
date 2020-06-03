---
title: Operação GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Encontre informações sobre a operação do EWS do GetDiscoverySearchConfiguration.
ms.openlocfilehash: 4db435988a9954b921e7851986b6f92ffedbad94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461020"
---
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="9b811-103">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="9b811-104">Encontre informações sobre a operação do EWS do **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="9b811-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="9b811-105">A operação **GetDiscoverySearchConfiguration** retorna informações de configuração para bloqueios in-loco, pesquisas salvas de descoberta e caixas de correio habilitadas para pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="9b811-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="9b811-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9b811-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="9b811-107">Usando a operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="9b811-108">A operação **GetDiscoverySearchConfiguration** fornece informações de configuração para pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="9b811-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="9b811-109">As solicitações podem conter um ou mais dos seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="9b811-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="9b811-110">[SearchId](searchid.md) — identifica uma pesquisa de descoberta salva.</span><span class="sxs-lookup"><span data-stu-id="9b811-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="9b811-111">Se esse argumento for enviado na solicitação, os valores dos outros argumentos serão ignorados.</span><span class="sxs-lookup"><span data-stu-id="9b811-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="9b811-112">[ExpandGroupMembership](expandgroupmembership.md) — indica se a associação de grupo está expandida na resposta.</span><span class="sxs-lookup"><span data-stu-id="9b811-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="9b811-113">Um valor **true** indica que a associação de grupo foi expandida para que todas as caixas de correio que podem ser pesquisadas sejam retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="9b811-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="9b811-114">Um valor **false** indica que apenas o grupo é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="9b811-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="9b811-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — indica se todas as caixas de correio que podem ser pesquisadas são retornadas além da configuração de bloqueio in-loco.</span><span class="sxs-lookup"><span data-stu-id="9b811-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="9b811-116">Um valor **true** indica que somente as configurações de bloqueio in-loco são retornadas.</span><span class="sxs-lookup"><span data-stu-id="9b811-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="9b811-117">Um valor **false** indica que todos os identificadores de caixa de correio pesquisáveis são retornados além dos identificadores de bloqueio in-loco.</span><span class="sxs-lookup"><span data-stu-id="9b811-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="9b811-118">Se esse elemento não estiver presente, o comportamento padrão será o equivalente do valor **false**.</span><span class="sxs-lookup"><span data-stu-id="9b811-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="9b811-119">Cabeçalhos SOAP de operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="9b811-120">A operação **GetDiscoverySearchConfiguration** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="9b811-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="9b811-121">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="9b811-121">**Header name**</span></span>|<span data-ttu-id="9b811-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b811-122">**Element**</span></span>|<span data-ttu-id="9b811-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b811-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9b811-124">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="9b811-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="9b811-125">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="9b811-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="9b811-126">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b811-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="9b811-127">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b811-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9b811-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="9b811-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="9b811-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="9b811-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="9b811-130">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="9b811-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="9b811-131">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b811-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9b811-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="9b811-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="9b811-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9b811-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="9b811-134">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b811-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="9b811-135">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="9b811-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="9b811-136">Exemplo de solicitação de operação GetDiscoverySearchConfiguration: obter a configuração de pesquisa de descoberta para uma pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="9b811-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="9b811-137">O exemplo a seguir de uma solicitação de operação **GetDiscoverySearchConfiguration** mostra como solicitar a configuração de uma pesquisa salva chamada "MyDiscSearchFor-sbrown".</span><span class="sxs-lookup"><span data-stu-id="9b811-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="9b811-138">Os argumentos dos elementos [ExpandGroupMembership](expandgroupmembership.md) e [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) são ignorados.</span><span class="sxs-lookup"><span data-stu-id="9b811-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetDiscoverySearchConfiguration>
         <m:SearchId>MyDiscSearchFor-sbrown</m:SearchId>
         <m:ExpandGroupMembership>true</m:ExpandGroupMembership>
         <m:InPlaceHoldConfigurationOnly>false</m:InPlaceHoldConfigurationOnly>
      </m:GetDiscoverySearchConfiguration>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="9b811-139">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9b811-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9b811-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="9b811-141">SearchId</span><span class="sxs-lookup"><span data-stu-id="9b811-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="9b811-142">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="9b811-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="9b811-143">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="9b811-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="9b811-144">Resposta de operação GetDiscoverySearchConfiguration bem-sucedida: solicitação para uma única pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="9b811-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="9b811-145">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetDiscoverySearchConfiguration** para obter a configuração de uma pesquisa salva chamada "MyDiscSearchFor-sbrown".</span><span class="sxs-lookup"><span data-stu-id="9b811-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <SearchId>MyDiscSearchFor-sbrown</SearchId>
          <SearchQuery>test item</SearchQuery>
          <SearchableMailboxes>
            <SearchableMailbox>
              <Guid>3c620d04-8b22-432e-92be-5b9321599576</Guid>
              <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
              <IsExternalMailbox>false</IsExternalMailbox>
              <ExternalEmailAddress/>
              <DisplayName>Steven Brown</DisplayName>
              <IsMembershipGroup>false</IsMembershipGroup>
              <ReferenceId>/o=First/ou=Exchange(FYDILT)/cn=Recipients/cn=313ecf-Steve</ReferenceId>
            </SearchableMailbox>
          </SearchableMailboxes>
        </DiscoverySearchConfiguration>
      </DiscoverySearchConfigurations>
    </GetDiscoverySearchConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="9b811-146">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9b811-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9b811-147">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="9b811-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="9b811-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b811-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9b811-149">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="9b811-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="9b811-150">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="9b811-151">SearchId</span><span class="sxs-lookup"><span data-stu-id="9b811-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="9b811-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="9b811-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="9b811-153">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b811-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="9b811-154">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="9b811-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="9b811-155">Guid</span><span class="sxs-lookup"><span data-stu-id="9b811-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="9b811-156">PrimarySmtpAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="9b811-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="9b811-157">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="9b811-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="9b811-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9b811-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="9b811-159">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="9b811-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="9b811-160">Membro ismembership</span><span class="sxs-lookup"><span data-stu-id="9b811-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="9b811-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="9b811-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="9b811-162">Resposta de operação GetDiscoverySearchConfiguration bem-sucedida: solicitação de bloqueio in-loco</span><span class="sxs-lookup"><span data-stu-id="9b811-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="9b811-163">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetDiscoverySearchConfiguration** para obter bloqueios in-loco apenas.</span><span class="sxs-lookup"><span data-stu-id="9b811-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <InPlaceHoldIdentity>6ea486f0f3f140efb044682a2e782abdf</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="9b811-164">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9b811-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9b811-165">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="9b811-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="9b811-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b811-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9b811-167">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="9b811-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="9b811-168">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="9b811-169">SearchId</span><span class="sxs-lookup"><span data-stu-id="9b811-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="9b811-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="9b811-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="9b811-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="9b811-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="9b811-172">ManagedByOrganization</span><span class="sxs-lookup"><span data-stu-id="9b811-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="9b811-173">Resposta de operação GetDiscoverySearchConfiguration bem-sucedida: solicitação para todas as configurações de pesquisa de descoberta salvas</span><span class="sxs-lookup"><span data-stu-id="9b811-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="9b811-174">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetDiscoverySearchConfiguration** para obter todas as pesquisas de descoberta salvas.</span><span class="sxs-lookup"><span data-stu-id="9b811-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>3c620d04-8b33-435e-95be-5b9351599576</Guid>
                     <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Steven Brown</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=35381a742f0e47e395c8601a60d13ecz-Steve</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>e788c4b0-54a2-458c-83b2-22d5bb02b23f</Guid>
                     <PrimarySmtpAddress>Administrator@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Administrator</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=ebez7871332d4595abe1c62962911a58-Admin</ReferenceId>
                  </SearchableMailbox>
                  <SearchableMailbox>
                     <Guid>6f6cff39-8967-4a60-b43f-328413c25199</Guid>
                     <PrimarySmtpAddress>ADavis@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Anthony Davis</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=f10c9f70519844beb04101d8f40c572z-Antho</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9b811-175">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9b811-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9b811-176">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="9b811-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="9b811-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b811-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9b811-178">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="9b811-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="9b811-179">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="9b811-180">SearchId</span><span class="sxs-lookup"><span data-stu-id="9b811-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="9b811-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="9b811-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="9b811-182">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b811-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="9b811-183">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="9b811-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="9b811-184">Guid</span><span class="sxs-lookup"><span data-stu-id="9b811-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="9b811-185">PrimarySmtpAddress (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="9b811-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="9b811-186">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="9b811-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="9b811-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9b811-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="9b811-188">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="9b811-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="9b811-189">Membro ismembership</span><span class="sxs-lookup"><span data-stu-id="9b811-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="9b811-190">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="9b811-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="9b811-191">Resposta de erro de operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b811-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="9b811-192">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="9b811-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="9b811-193">Esta é uma resposta a uma solicitação para obter uma pesquisa salva que não é encontrada no servidor.</span><span class="sxs-lookup"><span data-stu-id="9b811-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
```XML
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="9b811-194">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="9b811-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9b811-195">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="9b811-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="9b811-196">MessageText</span><span class="sxs-lookup"><span data-stu-id="9b811-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9b811-197">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b811-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9b811-198">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9b811-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="9b811-199">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="9b811-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="9b811-200">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="9b811-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9b811-201">Confira também</span><span class="sxs-lookup"><span data-stu-id="9b811-201">See also</span></span>

- [<span data-ttu-id="9b811-202">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9b811-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="9b811-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b811-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="9b811-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b811-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="9b811-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b811-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="9b811-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b811-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="9b811-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9b811-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="9b811-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="9b811-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

