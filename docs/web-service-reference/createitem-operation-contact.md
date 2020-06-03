---
title: Operação CreateItem (contato)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 417e994b-0a17-4c24-9527-04796b80b029
description: A operação CreateItem é usada para criar contatos no repositório do Exchange.
ms.openlocfilehash: e1d78392b94d328cf687655cd93e6c9568f6274f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457120"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="db3a0-103">Operação CreateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="db3a0-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="db3a0-104">A operação CreateItem é usada para criar contatos no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="db3a0-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db3a0-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="db3a0-105">Remarks</span></span>

<span data-ttu-id="db3a0-106">A criação de listas de distribuição particulares não é suportada.</span><span class="sxs-lookup"><span data-stu-id="db3a0-106">The creation of private distribution lists is not supported.</span></span> <span data-ttu-id="db3a0-107">Todas as propriedades dentro do contêiner [CompleteName](completename.md) são somente leitura e não podem ser definidas em um item de contato.</span><span class="sxs-lookup"><span data-stu-id="db3a0-107">All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="db3a0-108">Exemplo de solicitação CreateItem</span><span class="sxs-lookup"><span data-stu-id="db3a0-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="db3a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db3a0-109">Description</span></span>

<span data-ttu-id="db3a0-110">O exemplo a seguir de uma solicitação CreateItem SOAP válida mostra como criar um contato na pasta contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="db3a0-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="db3a0-111">Código</span><span class="sxs-lookup"><span data-stu-id="db3a0-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts"/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:FileAs>SampleContact</t:FileAs>
          <t:GivenName>Tanja</t:GivenName>
          <t:CompanyName>Blue Yonder Airlines</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
          </t:EmailAddresses>
          <t:PhysicalAddresses>
            <t:Entry Key="Business">
              <t:Street>1234 56th Ave</t:Street>
              <t:City>La Habra</t:City>
              <t:State>CA</t:State>
              <t: CountryOrRegion>USA</t: CountryOrRegion>
            </t:Entry>
          </t:PhysicalAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">4255550199</t:Entry>
          </t:PhoneNumbers>
          <t:JobTitle>Manager</t:JobTitle>
          <t:Surname>Plate</t:Surname>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="db3a0-112">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="db3a0-112">Request elements</span></span>

<span data-ttu-id="db3a0-113">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="db3a0-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="db3a0-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="db3a0-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="db3a0-115">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="db3a0-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="db3a0-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="db3a0-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="db3a0-117">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="db3a0-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="db3a0-118">Contato</span><span class="sxs-lookup"><span data-stu-id="db3a0-118">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="db3a0-119">FileAs</span><span class="sxs-lookup"><span data-stu-id="db3a0-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="db3a0-120">GivenName</span><span class="sxs-lookup"><span data-stu-id="db3a0-120">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="db3a0-121">CompanyName</span><span class="sxs-lookup"><span data-stu-id="db3a0-121">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="db3a0-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="db3a0-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="db3a0-123">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="db3a0-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="db3a0-124">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="db3a0-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="db3a0-125">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="db3a0-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="db3a0-126">123</span><span class="sxs-lookup"><span data-stu-id="db3a0-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="db3a0-127">Cidade</span><span class="sxs-lookup"><span data-stu-id="db3a0-127">City</span></span>](city.md)
    
- [<span data-ttu-id="db3a0-128">State</span><span class="sxs-lookup"><span data-stu-id="db3a0-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="db3a0-129">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="db3a0-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="db3a0-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="db3a0-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="db3a0-131">Entrada (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="db3a0-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="db3a0-132">JobTitle</span><span class="sxs-lookup"><span data-stu-id="db3a0-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="db3a0-133">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="db3a0-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="db3a0-134">Solicitação CreateItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="db3a0-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="db3a0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="db3a0-135">Description</span></span>

<span data-ttu-id="db3a0-136">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateItem que criou um contato.</span><span class="sxs-lookup"><span data-stu-id="db3a0-136">The following example shows a successful response to the CreateItem request that created a contact.</span></span> <span data-ttu-id="db3a0-137">Neste exemplo, a resposta contém o identificador do item recém-criado.</span><span class="sxs-lookup"><span data-stu-id="db3a0-137">In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="db3a0-138">Código</span><span class="sxs-lookup"><span data-stu-id="db3a0-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtA=" ChangeKey="EQAAAB" />
            </t:Contact>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="db3a0-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="db3a0-139">Comments</span></span>

<span data-ttu-id="db3a0-140">O identificador de item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="db3a0-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="db3a0-141">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="db3a0-141">Successful response elements</span></span>

<span data-ttu-id="db3a0-142">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="db3a0-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="db3a0-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="db3a0-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="db3a0-144">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="db3a0-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="db3a0-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="db3a0-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="db3a0-146">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="db3a0-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="db3a0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db3a0-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="db3a0-148">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="db3a0-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="db3a0-149">Contato</span><span class="sxs-lookup"><span data-stu-id="db3a0-149">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="db3a0-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="db3a0-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="db3a0-151">Exemplo de solicitação CreateItem inválida</span><span class="sxs-lookup"><span data-stu-id="db3a0-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="db3a0-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="db3a0-152">Description</span></span>

<span data-ttu-id="db3a0-153">O exemplo a seguir mostra uma solicitação que contém um XML válido, mas instruções incompatíveis.</span><span class="sxs-lookup"><span data-stu-id="db3a0-153">The following example shows a request that contains valid XML but incompatible instructions.</span></span> <span data-ttu-id="db3a0-154">Não é possível criar um contato em uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="db3a0-154">A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="db3a0-155">Código</span><span class="sxs-lookup"><span data-stu-id="db3a0-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id='searchfolders'/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:ItemClass>IPM.Contact</t:ItemClass>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="createitem-contact-error-response"></a><span data-ttu-id="db3a0-156">Resposta de erro CreateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="db3a0-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="db3a0-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="db3a0-157">Description</span></span>

<span data-ttu-id="db3a0-158">O exemplo a seguir mostra uma resposta de erro a uma solicitação CreateItem (contato).</span><span class="sxs-lookup"><span data-stu-id="db3a0-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="db3a0-159">Código</span><span class="sxs-lookup"><span data-stu-id="db3a0-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot create a contact in a non-contact Folder.</m:MessageText>
          <m:ResponseCode>ErrorCannotCreateContactInNonContactFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="db3a0-160">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="db3a0-160">Error response elements</span></span>

<span data-ttu-id="db3a0-161">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="db3a0-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="db3a0-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="db3a0-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="db3a0-163">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="db3a0-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="db3a0-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="db3a0-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="db3a0-165">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="db3a0-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="db3a0-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="db3a0-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="db3a0-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db3a0-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="db3a0-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="db3a0-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="db3a0-169">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="db3a0-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="db3a0-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="db3a0-170">See also</span></span>



[<span data-ttu-id="db3a0-171">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="db3a0-171">CreateItem operation</span></span>](createitem-operation.md)

