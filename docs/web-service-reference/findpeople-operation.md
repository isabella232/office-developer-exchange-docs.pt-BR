---
title: Operação FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Encontre informações sobre o EWS FindPeople operação.
ms.openlocfilehash: 97c34d7df590d20513e8f1ad476d62f16815a42b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752300"
---
# <a name="findpeople-operation"></a><span data-ttu-id="2e6e5-103">Operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="2e6e5-103">FindPeople operation</span></span>

<span data-ttu-id="2e6e5-104">Encontre informações sobre a operação de EWS **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="2e6e5-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="2e6e5-105">A operação **FindPeople** retorna todos os objetos de pessoa de uma pasta de contatos especificada ou recupera contatos que correspondem a uma cadeia de caracteres de consulta especificada.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="2e6e5-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="2e6e5-107">Usando a operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="2e6e5-107">Using the FindPeople operation</span></span>

<span data-ttu-id="2e6e5-108">A operação **FindPeople** retorna informações de contato agregadas.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="2e6e5-109">A operação **FindPeople** aproveita as funções existentes dos tipos complexos [BaseShape](baseshape.md) e [restrição](restriction.md) adicionando uma restrição de agregação de lista segura e a capacidade de retornar as propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="2e6e5-110">Usando uma restrição, um cliente pode especificar filtros, como "retornar apenas resultados que têm um endereço de mensagens Instantâneas".</span><span class="sxs-lookup"><span data-stu-id="2e6e5-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="2e6e5-111">O comportamento de pesquisa padrão refere-se a caixa de correio pessoal do usuário especificado e a lista de endereços global (GAL).</span><span class="sxs-lookup"><span data-stu-id="2e6e5-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="2e6e5-112">Ao pesquisar a GAL como a pasta de pesquisa primário, você deve especificar uma cadeia de caracteres de consulta, em vez de uma restrição, porque não permite esta operação para navegação da GAL.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="2e6e5-113">Cabeçalhos SOAP FindPeople operação</span><span class="sxs-lookup"><span data-stu-id="2e6e5-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="2e6e5-114">A operação **FindPeople** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="2e6e5-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="2e6e5-115">**Header name**</span></span>|<span data-ttu-id="2e6e5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e6e5-116">**Element**</span></span>|<span data-ttu-id="2e6e5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e6e5-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2e6e5-118">**Representação**</span><span class="sxs-lookup"><span data-stu-id="2e6e5-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="2e6e5-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="2e6e5-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2e6e5-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="2e6e5-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2e6e5-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="2e6e5-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="2e6e5-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="2e6e5-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2e6e5-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="2e6e5-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2e6e5-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="2e6e5-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="2e6e5-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2e6e5-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2e6e5-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="2e6e5-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="2e6e5-130">Exemplo de solicitação de operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="2e6e5-130">FindPeople operation request example</span></span>

<span data-ttu-id="2e6e5-131">O exemplo a seguir de uma solicitação de operação **FindPeople** mostra como retornar os primeiros 100 contatos da pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="2e6e5-132">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="2e6e5-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2e6e5-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="2e6e5-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="2e6e5-134">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="2e6e5-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="2e6e5-135">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="2e6e5-136">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="2e6e5-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="2e6e5-137">O exemplo a seguir de uma solicitação de operação **FindPeople** mostra como retornar os primeiros 100 contatos da GAL usando-se uma cadeia de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="2e6e5-138">Definir o **DistinguishedFolderId** "diretório" pesquisará GAL como a principal fonte de personagens.</span><span class="sxs-lookup"><span data-stu-id="2e6e5-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="2e6e5-139">Resposta de operação FindPeople bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="2e6e5-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="2e6e5-140">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="2e6e5-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="2e6e5-141">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="2e6e5-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="2e6e5-142">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="2e6e5-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="2e6e5-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2e6e5-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2e6e5-144">Pessoas</span><span class="sxs-lookup"><span data-stu-id="2e6e5-144">People</span></span>](people.md)
    
- [<span data-ttu-id="2e6e5-145">Pessoa</span><span class="sxs-lookup"><span data-stu-id="2e6e5-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="2e6e5-146">PersonaId</span><span class="sxs-lookup"><span data-stu-id="2e6e5-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="2e6e5-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="2e6e5-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="2e6e5-148">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="2e6e5-149">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="2e6e5-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="2e6e5-150">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="2e6e5-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="2e6e5-151">FileAs</span><span class="sxs-lookup"><span data-stu-id="2e6e5-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="2e6e5-152">GivenName</span><span class="sxs-lookup"><span data-stu-id="2e6e5-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="2e6e5-153">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="2e6e5-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="2e6e5-154">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="2e6e5-155">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="2e6e5-156">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="2e6e5-157">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="2e6e5-158">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2e6e5-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="2e6e5-159">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="2e6e5-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="2e6e5-160">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="2e6e5-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="2e6e5-161">Resposta de erro de operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="2e6e5-161">FindPeople operation error response</span></span>

<span data-ttu-id="2e6e5-162">Para códigos de erro que são genéricos para EWS, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="2e6e5-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="2e6e5-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="2e6e5-163">See also</span></span>

- [<span data-ttu-id="2e6e5-164">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2e6e5-164">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="2e6e5-165">Operação GetPersona</span><span class="sxs-lookup"><span data-stu-id="2e6e5-165">GetPersona operation</span></span>](getpersona-operation.md)
    

