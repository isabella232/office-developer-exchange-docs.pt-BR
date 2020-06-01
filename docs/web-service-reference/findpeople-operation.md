---
title: Operação FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Encontre informações sobre a operação do EWS do FindPeople.
ms.openlocfilehash: ab5edc3f140e34123ce1f009c401ddd61a0e2598
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462905"
---
# <a name="findpeople-operation"></a><span data-ttu-id="91a3b-103">Operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="91a3b-103">FindPeople operation</span></span>

<span data-ttu-id="91a3b-104">Encontre informações sobre a operação do EWS do **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="91a3b-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="91a3b-105">A operação **FindPeople** retorna todos os objetos persona de uma pasta de contatos especificada ou recupera contatos que correspondem a uma cadeia de caracteres de consulta especificada.</span><span class="sxs-lookup"><span data-stu-id="91a3b-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="91a3b-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91a3b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="91a3b-107">Usando a operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="91a3b-107">Using the FindPeople operation</span></span>

<span data-ttu-id="91a3b-108">A operação **FindPeople** retorna informações de contato agregadas.</span><span class="sxs-lookup"><span data-stu-id="91a3b-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="91a3b-109">A operação **FindPeople** cria a funcionalidade existente dos tipos complexos [Restriction](restriction.md) e [BaseShape](baseshape.md) adicionando uma restrição de agregação e a capacidade de retornar propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="91a3b-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="91a3b-110">Usando uma restrição, um cliente pode especificar filtros, como "somente resultados de retorno que têm um endereço de mensagens instantâneas".</span><span class="sxs-lookup"><span data-stu-id="91a3b-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="91a3b-111">O comportamento de pesquisa padrão é direcionado para a caixa de correio pessoal e a lista de endereços global (GAL) do usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="91a3b-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="91a3b-112">Ao pesquisar a GAL como a pasta de pesquisa principal, você deve especificar uma cadeia de caracteres de consulta em vez de uma restrição, porque essa operação não permite a navegação da GAL.</span><span class="sxs-lookup"><span data-stu-id="91a3b-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="91a3b-113">Cabeçalhos SOAP de operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="91a3b-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="91a3b-114">A operação **FindPeople** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="91a3b-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="91a3b-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="91a3b-115">**Header name**</span></span>|<span data-ttu-id="91a3b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="91a3b-116">**Element**</span></span>|<span data-ttu-id="91a3b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91a3b-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="91a3b-118">**Representação**</span><span class="sxs-lookup"><span data-stu-id="91a3b-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="91a3b-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="91a3b-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="91a3b-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="91a3b-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="91a3b-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="91a3b-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="91a3b-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="91a3b-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="91a3b-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="91a3b-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="91a3b-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="91a3b-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="91a3b-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="91a3b-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="91a3b-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="91a3b-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="91a3b-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="91a3b-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="91a3b-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="91a3b-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="91a3b-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="91a3b-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="91a3b-130">Exemplo de solicitação de operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="91a3b-130">FindPeople operation request example</span></span>

<span data-ttu-id="91a3b-131">O exemplo a seguir de uma solicitação de operação **FindPeople** mostra como retornar os primeiros 100 contatos da pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="91a3b-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:FindPeople>
         <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="contacts"/>
         </m:ParentFolderId>
      </m:FindPeople>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="91a3b-132">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="91a3b-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="91a3b-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="91a3b-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="91a3b-134">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="91a3b-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="91a3b-135">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="91a3b-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="91a3b-136">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="91a3b-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="91a3b-137">O exemplo a seguir de uma solicitação de operação **FindPeople** mostra como retornar os primeiros 100 contatos da GAL usando uma cadeia de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="91a3b-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="91a3b-138">A configuração do **DistinguishedFolderId** como "Directory" pesquisará a GAL como a principal fonte de personas.</span><span class="sxs-lookup"><span data-stu-id="91a3b-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
    <m:FindPeople>
      <m:PersonaShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="persona:DisplayName"/>
          <t:FieldURI FieldURI="persona:Title"/>
        </t:AdditionalProperties>
      </m:PersonaShape>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="directory"/>
      </m:ParentFolderId>
      <m:QueryString>adams</m:QueryString>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="91a3b-139">Resposta de operação FindPeople bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="91a3b-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="91a3b-140">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="91a3b-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAOjFqObcLmtOlzlRnHdXQjo=" />
          <CreationTime>2012-01-11T22:25:37Z</CreationTime>
          <DisplayName>Terry Adams</DisplayName>
          <DisplayNameFirstLast>Terry Adams</DisplayNameFirstLast>
          <DisplayNameLastFirst>Adams Terry</DisplayNameLastFirst>
          <FileAs>Adams, Terry</FileAs>
          <GivenName>Terry</GivenName>
          <Surname>Adams</Surname>
          <EmailAddress>
            <Name>terry@litwareinc.com</Name>
            <EmailAddress>terry@litwareinc.com</EmailAddress>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
          <EmailAddresses>
            <EmailAddress>
              <Name>terry@litwareinc.com</Name>
              <EmailAddress>terry@litwareinc.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
            <EmailAddress>
              <Name>tadams@contoso.com</Name>
              <EmailAddress>tadams@contoso.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
          </EmailAddresses>
          <RelevanceScore>2147483647</RelevanceScore>
        </Persona>
      </People>
      <TotalNumberOfPeopleInView>1</TotalNumberOfPeopleInView>
    </FindPeopleResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="91a3b-141">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="91a3b-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="91a3b-142">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="91a3b-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="91a3b-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="91a3b-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="91a3b-144">Pessoas</span><span class="sxs-lookup"><span data-stu-id="91a3b-144">People</span></span>](people.md)
    
- [<span data-ttu-id="91a3b-145">Pessoal</span><span class="sxs-lookup"><span data-stu-id="91a3b-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="91a3b-146">Personaid</span><span class="sxs-lookup"><span data-stu-id="91a3b-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="91a3b-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="91a3b-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="91a3b-148">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="91a3b-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="91a3b-149">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="91a3b-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="91a3b-150">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="91a3b-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="91a3b-151">FileAs</span><span class="sxs-lookup"><span data-stu-id="91a3b-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="91a3b-152">GivenName</span><span class="sxs-lookup"><span data-stu-id="91a3b-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="91a3b-153">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="91a3b-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="91a3b-154">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="91a3b-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="91a3b-155">EmailAddress (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="91a3b-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="91a3b-156">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="91a3b-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="91a3b-157">EmailAddress (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="91a3b-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="91a3b-158">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="91a3b-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="91a3b-159">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="91a3b-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="91a3b-160">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="91a3b-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="91a3b-161">Resposta de erro de operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="91a3b-161">FindPeople operation error response</span></span>

<span data-ttu-id="91a3b-162">Para códigos de erro genéricos para EWS, confira [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="91a3b-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="91a3b-163">Também consulte</span><span class="sxs-lookup"><span data-stu-id="91a3b-163">See also</span></span>

- [<span data-ttu-id="91a3b-164">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="91a3b-164">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="91a3b-165">Operação getpersona</span><span class="sxs-lookup"><span data-stu-id="91a3b-165">GetPersona operation</span></span>](getpersona-operation.md)
    

