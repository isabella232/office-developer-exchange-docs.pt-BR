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
description: A operação CreateItem é usada para criar contatos no armazenamento do Exchange.
ms.openlocfilehash: 05e4715f3c6675401ae7afac852395f7459c02c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751602"
---
# <a name="createitem-operation-contact"></a><span data-ttu-id="a8674-103">Operação CreateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="a8674-103">CreateItem operation (contact)</span></span>

<span data-ttu-id="a8674-104">A operação CreateItem é usada para criar contatos no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8674-104">The CreateItem operation is used to create contacts in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8674-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="a8674-105">Remarks</span></span>

<span data-ttu-id="a8674-106">Não há suporte para a criação de listas de distribuição privada.</span><span class="sxs-lookup"><span data-stu-id="a8674-106">The creation of private distribution lists is not supported.</span></span> <span data-ttu-id="a8674-107">Todas as propriedades dentro do contêiner [CompleteName](completename.md) são somente leitura e não podem ser definidas em um item de contato.</span><span class="sxs-lookup"><span data-stu-id="a8674-107">All properties within the [CompleteName](completename.md) container are read-only and cannot be set on a contact item.</span></span> 
  
## <a name="createitem-request-example"></a><span data-ttu-id="a8674-108">Exemplo de solicitação CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8674-108">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="a8674-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8674-109">Description</span></span>

<span data-ttu-id="a8674-110">O exemplo a seguir de uma solicitação SOAP CreateItem válida mostra como criar um contato na pasta padrão Contatos.</span><span class="sxs-lookup"><span data-stu-id="a8674-110">The following example of a valid CreateItem SOAP request shows how to create a contact in the default Contacts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8674-111">Código</span><span class="sxs-lookup"><span data-stu-id="a8674-111">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" >
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

### <a name="request-elements"></a><span data-ttu-id="a8674-112">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8674-112">Request elements</span></span>

<span data-ttu-id="a8674-113">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="a8674-113">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a8674-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8674-114">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="a8674-115">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="a8674-115">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="a8674-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a8674-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="a8674-117">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a8674-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="a8674-118">Contato</span><span class="sxs-lookup"><span data-stu-id="a8674-118">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="a8674-119">FileAs</span><span class="sxs-lookup"><span data-stu-id="a8674-119">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="a8674-120">GivenName</span><span class="sxs-lookup"><span data-stu-id="a8674-120">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="a8674-121">CompanyName</span><span class="sxs-lookup"><span data-stu-id="a8674-121">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="a8674-122">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a8674-122">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="a8674-123">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a8674-123">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="a8674-124">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="a8674-124">PhysicalAddresses</span></span>](physicaladdresses.md)
    
- [<span data-ttu-id="a8674-125">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="a8674-125">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md)
    
- [<span data-ttu-id="a8674-126">Rua</span><span class="sxs-lookup"><span data-stu-id="a8674-126">Street</span></span>](street.md)
    
- [<span data-ttu-id="a8674-127">Cidade</span><span class="sxs-lookup"><span data-stu-id="a8674-127">City</span></span>](city.md)
    
- [<span data-ttu-id="a8674-128">Estado</span><span class="sxs-lookup"><span data-stu-id="a8674-128">State</span></span>](state-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a8674-129">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a8674-129">CountryOrRegion</span></span>](countryorregion.md)
    
- [<span data-ttu-id="a8674-130">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="a8674-130">PhoneNumbers</span></span>](phonenumbers.md)
    
- [<span data-ttu-id="a8674-131">Entrada (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="a8674-131">Entry (PhoneNumber)</span></span>](entry-phonenumber.md)
    
- [<span data-ttu-id="a8674-132">JobTitle</span><span class="sxs-lookup"><span data-stu-id="a8674-132">JobTitle</span></span>](jobtitle.md)
    
- [<span data-ttu-id="a8674-133">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="a8674-133">Surname</span></span>](surname.md)
    
## <a name="successful-createitem-request"></a><span data-ttu-id="a8674-134">Solicitação de CreateItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a8674-134">Successful CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="a8674-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8674-135">Description</span></span>

<span data-ttu-id="a8674-136">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de CreateItem que criou um contato.</span><span class="sxs-lookup"><span data-stu-id="a8674-136">The following example shows a successful response to the CreateItem request that created a contact.</span></span> <span data-ttu-id="a8674-137">Neste exemplo, a resposta conterá o identificador do item recém-criado.</span><span class="sxs-lookup"><span data-stu-id="a8674-137">In this example, the response contains the identifier of the newly created item.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8674-138">Código</span><span class="sxs-lookup"><span data-stu-id="a8674-138">Code</span></span>

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="a8674-139">Comments</span><span class="sxs-lookup"><span data-stu-id="a8674-139">Comments</span></span>

<span data-ttu-id="a8674-140">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8674-140">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="a8674-141">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a8674-141">Successful response elements</span></span>

<span data-ttu-id="a8674-142">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="a8674-142">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a8674-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a8674-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a8674-144">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="a8674-144">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="a8674-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a8674-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a8674-146">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a8674-146">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="a8674-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8674-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a8674-148">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a8674-148">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="a8674-149">Contato</span><span class="sxs-lookup"><span data-stu-id="a8674-149">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="a8674-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="a8674-150">ItemId</span></span>](itemid.md)
    
## <a name="invalid-createitem-request-example"></a><span data-ttu-id="a8674-151">Exemplo de solicitação inválido CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8674-151">Invalid CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="a8674-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8674-152">Description</span></span>

<span data-ttu-id="a8674-153">O exemplo a seguir mostra uma solicitação que contém o XML válido, mas as instruções incompatíveis.</span><span class="sxs-lookup"><span data-stu-id="a8674-153">The following example shows a request that contains valid XML but incompatible instructions.</span></span> <span data-ttu-id="a8674-154">Não é possível criar um contato em uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a8674-154">A contact cannot be created in a search folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8674-155">Código</span><span class="sxs-lookup"><span data-stu-id="a8674-155">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
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

## <a name="createitem-contact-error-response"></a><span data-ttu-id="a8674-156">Resposta de erro CreateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="a8674-156">CreateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="a8674-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8674-157">Description</span></span>

<span data-ttu-id="a8674-158">O exemplo a seguir mostra uma resposta de erro a uma solicitação de CreateItem (contato).</span><span class="sxs-lookup"><span data-stu-id="a8674-158">The following example shows an error response to a CreateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="a8674-159">Código</span><span class="sxs-lookup"><span data-stu-id="a8674-159">Code</span></span>

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="a8674-160">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="a8674-160">Error response elements</span></span>

<span data-ttu-id="a8674-161">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="a8674-161">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="a8674-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a8674-162">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a8674-163">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="a8674-163">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="a8674-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a8674-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a8674-165">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a8674-165">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="a8674-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="a8674-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a8674-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a8674-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a8674-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a8674-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a8674-169">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="a8674-169">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a><span data-ttu-id="a8674-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="a8674-170">See also</span></span>



[<span data-ttu-id="a8674-171">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="a8674-171">CreateItem operation</span></span>](createitem-operation.md)

