---
title: Operação GetItem (contato)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 6b96dace-1260-4b83-869a-7c31c5583daa
description: A operação GetItem é usada para obter os itens de contato do armazenamento do Exchange.
ms.openlocfilehash: 8d7436421f0c54a49345e8ef6b37cb442bca4277
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752542"
---
# <a name="getitem-operation-contact"></a><span data-ttu-id="ce045-103">Operação GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="ce045-103">GetItem operation (contact)</span></span>

<span data-ttu-id="ce045-104">A operação GetItem é usada para obter os itens de contato do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce045-104">The GetItem operation is used to get contact items from the Exchange store.</span></span>
  
## <a name="getitem-contact-request-example"></a><span data-ttu-id="ce045-105">Exemplo de solicitação de GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="ce045-105">GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="ce045-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce045-106">Description</span></span>

<span data-ttu-id="ce045-107">O exemplo a seguir mostra como obter um item do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce045-107">The following example shows how to get an item from the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce045-108">Código</span><span class="sxs-lookup"><span data-stu-id="ce045-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABY" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce045-109">Comments</span><span class="sxs-lookup"><span data-stu-id="ce045-109">Comments</span></span>

<span data-ttu-id="ce045-110">A solicitação para obter um item de armazenamento do Exchange assume o mesmo formato para todos os tipos de item.</span><span class="sxs-lookup"><span data-stu-id="ce045-110">The request to get an item from the Exchange store takes the same form for all item types.</span></span> <span data-ttu-id="ce045-111">As respostas às solicitações de itens diferentes serão diferentes porque itens diferentes retornam informações diferentes com base nas formas de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce045-111">The responses to requests for different items will be different because different items return different information based on the response shapes.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ce045-112">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce045-112">The item identifier has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ce045-113">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce045-113">Request elements</span></span>

<span data-ttu-id="ce045-114">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="ce045-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce045-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="ce045-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="ce045-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="ce045-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="ce045-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="ce045-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="ce045-118">ItemIds</span><span class="sxs-lookup"><span data-stu-id="ce045-118">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="ce045-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="ce045-119">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-contact-response"></a><span data-ttu-id="ce045-120">Resposta bem-sucedida GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="ce045-120">Successful GetItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="ce045-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce045-121">Description</span></span>

<span data-ttu-id="ce045-122">O exemplo de código a seguir mostra uma resposta bem-sucedida do GetItem para o **AllProperties**[BaseShape](baseshape.md).</span><span class="sxs-lookup"><span data-stu-id="ce045-122">The following code example shows a successful GetItem response for the **AllProperties**[BaseShape](baseshape.md).</span></span>
  
### <a name="code"></a><span data-ttu-id="ce045-123">Código</span><span class="sxs-lookup"><span data-stu-id="ce045-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EQAAABYq" />
              <t:ParentFolderId Id="AQAtAEFk==" ChangeKey="AQAAAA==" />
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text" />
              <t:DateTimeReceived>2006-08-18T17:31:18Z</t:DateTimeReceived>
              <t:Size>382</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-08-18T17:31:18Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-08-18T17:31:18Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en</t:Culture>
              <t:FileAs>SampleContact</t:FileAs>
              <t:FileAsMapping>None</t:FileAsMapping>
              <t:DisplayName>Tanja Plate</t:DisplayName>
              <t:GivenName>Tanja</t:GivenName>
              <t:Initials>T.P.</t:Initials>
              <t:CompleteName>
                <t:FirstName>Tanja</t:FirstName>
                <t:LastName>Plate</t:LastName>
                <t:Initials>T.P.</t:Initials>
                <t:FullName>Tanja Plate</t:FullName>
              </t:CompleteName>
              <t:CompanyName>Northwind Traders</t:CompanyName>
              <t:EmailAddresses>
                <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
                <t:Entry Key="EmailAddress2">tplate@example.com</t:Entry>
              </t:EmailAddresses>
              <t:PhysicalAddresses>
                <t:Entry Key="Business">
                  <t:Street>12345 67th Ave</t:Street>
                  <t:City>Whittier</t:City>
                  <t:State>CA</t:State>
                  <t:Country>USA</t:Country>
                </t:Entry>
              </t:PhysicalAddresses>
              <t:PhoneNumbers>
                <t:Entry Key="BusinessPhone">5625550199</t:Entry>
              </t:PhoneNumbers>
              <t:JobTitle>Project Manager</t:JobTitle>
              <t:Surname>Plate</t:Surname>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce045-124">Comments</span><span class="sxs-lookup"><span data-stu-id="ce045-124">Comments</span></span>

<span data-ttu-id="ce045-125">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce045-125">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="ce045-126">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ce045-126">Successful response elements</span></span>

<span data-ttu-id="ce045-127">Os seguintes elementos são usados na resposta para uma solicitação de GetItem com uma forma de resposta de **AllProperties** para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="ce045-127">The following elements are used in the response for a GetItem request with a response shape of **AllProperties** for a contact item.</span></span> 
  
- [<span data-ttu-id="ce045-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce045-128">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce045-129">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="ce045-129">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="ce045-130">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce045-130">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ce045-131">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce045-131">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="ce045-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce045-132">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ce045-133">Items</span><span class="sxs-lookup"><span data-stu-id="ce045-133">Items</span></span>](items.md)
    
- [<span data-ttu-id="ce045-134">Contato</span><span class="sxs-lookup"><span data-stu-id="ce045-134">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="ce045-135">ItemId</span><span class="sxs-lookup"><span data-stu-id="ce045-135">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ce045-136">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ce045-136">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="ce045-137">ItemClass</span><span class="sxs-lookup"><span data-stu-id="ce045-137">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="ce045-138">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ce045-138">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="ce045-139">Corpo</span><span class="sxs-lookup"><span data-stu-id="ce045-139">Body</span></span>](body.md)
    
- [<span data-ttu-id="ce045-140">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="ce045-140">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="ce045-141">Size</span><span class="sxs-lookup"><span data-stu-id="ce045-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="ce045-142">Importância</span><span class="sxs-lookup"><span data-stu-id="ce045-142">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="ce045-143">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="ce045-143">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="ce045-144">IsDraft</span><span class="sxs-lookup"><span data-stu-id="ce045-144">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="ce045-145">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="ce045-145">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="ce045-146">IsResend</span><span class="sxs-lookup"><span data-stu-id="ce045-146">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="ce045-147">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="ce045-147">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="ce045-148">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="ce045-148">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="ce045-149">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ce045-149">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="ce045-150">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ce045-150">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="ce045-151">Cultura</span><span class="sxs-lookup"><span data-stu-id="ce045-151">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="ce045-152">FileAs</span><span class="sxs-lookup"><span data-stu-id="ce045-152">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="ce045-153">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="ce045-153">FileAsMapping</span></span>](fileasmapping.md)
    
- [<span data-ttu-id="ce045-154">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="ce045-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="ce045-155">GivenName</span><span class="sxs-lookup"><span data-stu-id="ce045-155">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="ce045-156">Iniciais</span><span class="sxs-lookup"><span data-stu-id="ce045-156">Initials</span></span>](initials.md)
    
- [<span data-ttu-id="ce045-157">CompleteName</span><span class="sxs-lookup"><span data-stu-id="ce045-157">CompleteName</span></span>](completename.md)
    
- [<span data-ttu-id="ce045-158">FirstName</span><span class="sxs-lookup"><span data-stu-id="ce045-158">FirstName</span></span>](firstname.md)
    
- [<span data-ttu-id="ce045-159">LastName</span><span class="sxs-lookup"><span data-stu-id="ce045-159">LastName</span></span>](lastname.md)
    
- [<span data-ttu-id="ce045-160">FullName</span><span class="sxs-lookup"><span data-stu-id="ce045-160">FullName</span></span>](fullname.md)
    
- [<span data-ttu-id="ce045-161">CompanyName</span><span class="sxs-lookup"><span data-stu-id="ce045-161">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="ce045-162">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="ce045-162">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="ce045-163">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ce045-163">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="ce045-164">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="ce045-164">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="ce045-165">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="ce045-165">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="ce045-166">Rua</span><span class="sxs-lookup"><span data-stu-id="ce045-166">Street</span></span>](street.md)
    
- [<span data-ttu-id="ce045-167">Cidade</span><span class="sxs-lookup"><span data-stu-id="ce045-167">City</span></span>](city.md)
    
- [<span data-ttu-id="ce045-168">Estado</span><span class="sxs-lookup"><span data-stu-id="ce045-168">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ce045-169">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ce045-169">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="ce045-170">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="ce045-170">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="ce045-171">Entrada (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="ce045-171">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="ce045-172">JobTitle</span><span class="sxs-lookup"><span data-stu-id="ce045-172">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="ce045-173">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="ce045-173">Surname</span></span>](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a><span data-ttu-id="ce045-174">Exemplo de solicitação inválido GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="ce045-174">Invalid GetItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="ce045-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce045-175">Description</span></span>

<span data-ttu-id="ce045-176">O exemplo de código a seguir mostra uma solicitação inválida.</span><span class="sxs-lookup"><span data-stu-id="ce045-176">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce045-177">Código</span><span class="sxs-lookup"><span data-stu-id="ce045-177">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABq" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce045-178">Comments</span><span class="sxs-lookup"><span data-stu-id="ce045-178">Comments</span></span>

<span data-ttu-id="ce045-179">Identificadores de item tem sido reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce045-179">Item identifiers have been shortened to preserve readability.</span></span>
  
## <a name="getitem-contact-error-response"></a><span data-ttu-id="ce045-180">Resposta de erro GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="ce045-180">GetItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="ce045-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce045-181">Description</span></span>

<span data-ttu-id="ce045-182">O exemplo de código a seguir mostra uma resposta de erro a uma solicitação de GetItem (contato).</span><span class="sxs-lookup"><span data-stu-id="ce045-182">The following code example shows an error response to a GetItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce045-183">Código</span><span class="sxs-lookup"><span data-stu-id="ce045-183">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Mime conversion is not supported for this item type.</m:MessageText>
          <m:ResponseCode>ErrorUnsupportedMimeConversion</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="ce045-184">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="ce045-184">Error response elements</span></span>

<span data-ttu-id="ce045-185">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="ce045-185">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ce045-186">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce045-186">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce045-187">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="ce045-187">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="ce045-188">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce045-188">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ce045-189">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce045-189">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="ce045-190">MessageText</span><span class="sxs-lookup"><span data-stu-id="ce045-190">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ce045-191">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce045-191">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ce045-192">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ce045-192">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ce045-193">Items</span><span class="sxs-lookup"><span data-stu-id="ce045-193">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="ce045-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="ce045-194">See also</span></span>



[<span data-ttu-id="ce045-195">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="ce045-195">GetItem operation</span></span>](getitem-operation.md)


- [<span data-ttu-id="ce045-196">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce045-196">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

