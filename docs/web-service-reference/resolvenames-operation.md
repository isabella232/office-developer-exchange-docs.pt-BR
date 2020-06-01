---
title: Operação ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: A operação ResolveNames resolve endereços de email e nomes de exibição ambíguos.
ms.openlocfilehash: 51728addddd2bfb9d35b874ae8c11e83a4c8629b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468275"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="0cbba-103">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0cbba-103">ResolveNames operation</span></span>

<span data-ttu-id="0cbba-104">A operação **ResolveNames** resolve endereços de email e nomes de exibição ambíguos.</span><span class="sxs-lookup"><span data-stu-id="0cbba-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="0cbba-105">Usando a operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0cbba-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="0cbba-106">Essa operação pode ser usada para verificar aliases e resolver nomes de exibição para o usuário de caixa de correio apropriado.</span><span class="sxs-lookup"><span data-stu-id="0cbba-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="0cbba-107">Se houver nomes ambíguos, a resposta de operação **ResolveNames** fornecerá informações sobre cada usuário de caixa de correio para que o aplicativo cliente possa resolver os nomes.</span><span class="sxs-lookup"><span data-stu-id="0cbba-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0cbba-108">Comentários</span><span class="sxs-lookup"><span data-stu-id="0cbba-108">Remarks</span></span>

<span data-ttu-id="0cbba-109">A resposta ResolveNames retorna um máximo de 100 candidatos.</span><span class="sxs-lookup"><span data-stu-id="0cbba-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="0cbba-110">Os candidatos 100 retornados são os primeiros 100 encontrados na operação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0cbba-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="0cbba-111">Os endereços de email com tipos de roteamento prefixos, como SMTP ou SIP, são salvos em uma matriz de vários valores.</span><span class="sxs-lookup"><span data-stu-id="0cbba-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="0cbba-112">A operação **ResolveNames** executa uma correspondência parcial em relação a cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "SIP:User1@Contoso.com".</span><span class="sxs-lookup"><span data-stu-id="0cbba-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="0cbba-113">Se você não especificar um tipo de roteamento, **ResolveNames** usará como padrão o tipo de roteamento do SMTP, o corresponderá a uma propriedade de endereço SMTP primária e não pesquisará a matriz de vários valores.</span><span class="sxs-lookup"><span data-stu-id="0cbba-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="0cbba-114">Apenas um nome ambíguo pode ser especificado em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cbba-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="0cbba-115">O Active Directory é pesquisado primeiro e, em seguida, a pasta de contatos do usuário é pesquisada.</span><span class="sxs-lookup"><span data-stu-id="0cbba-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="0cbba-116">As entradas resolvidas da pasta de contatos de um usuário têm uma propriedade **ItemId** não nula, que pode ser usada em uma solicitação GetItem.</span><span class="sxs-lookup"><span data-stu-id="0cbba-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="0cbba-117">Se for a ID de uma lista de distribuição privada, ela poderá ser usada em uma [operação ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0cbba-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="0cbba-118">Se o atributo **ReturnFullContactData** for definido como **true**, as entradas do Active Directory localizadas com a operação **ResolveNames** retornarão propriedades adicionais que descrevem um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="0cbba-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="0cbba-119">O atributo **ReturnFullContactData** não afeta os dados retornados para contatos e listas de distribuição privada da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="0cbba-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="0cbba-120">Exemplo de solicitação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0cbba-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="0cbba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cbba-121">Description</span></span>

<span data-ttu-id="0cbba-122">O exemplo a seguir de uma solicitação **ResolveNames** mostra como resolver a entrada de User.</span><span class="sxs-lookup"><span data-stu-id="0cbba-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="0cbba-123">Código</span><span class="sxs-lookup"><span data-stu-id="0cbba-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="0cbba-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="0cbba-124">Comments</span></span>

<span data-ttu-id="0cbba-125">A resposta a essa solicitação retornará todas as entradas que começam com "Jo" ou "mi".</span><span class="sxs-lookup"><span data-stu-id="0cbba-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="0cbba-126">Os itens retornados são caixas de correio públicas, listas de distribuição pública e privada e contatos.</span><span class="sxs-lookup"><span data-stu-id="0cbba-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0cbba-127">Somente os contatos na pasta contatos pessoais padrão são pesquisados.</span><span class="sxs-lookup"><span data-stu-id="0cbba-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="0cbba-128">Estes são os resultados possíveis para uma solicitação **ResolveNames** :</span><span class="sxs-lookup"><span data-stu-id="0cbba-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="0cbba-129">As respostas que não contiverem uma entidade resolvida retornarão um valor de atributo **ResponseClass** igual a **erro**.</span><span class="sxs-lookup"><span data-stu-id="0cbba-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="0cbba-130">O elemento **MessageText** conterá " **nenhum resultado encontrado**."</span><span class="sxs-lookup"><span data-stu-id="0cbba-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="0cbba-131">As respostas que contenham uma única entidade resolvida retornarão um valor de atributo **ResponseClass** igual a **Success**.</span><span class="sxs-lookup"><span data-stu-id="0cbba-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="0cbba-132">As respostas que contêm várias entidades possíveis retornarão um valor de atributo **ResponseClass** igual a **Warning**.</span><span class="sxs-lookup"><span data-stu-id="0cbba-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="0cbba-133">Nesse caso, a entidade não pôde ser resolvida para uma identidade exclusiva.</span><span class="sxs-lookup"><span data-stu-id="0cbba-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="0cbba-134">O elemento **MessageText** conterá "vários resultados encontrados."</span><span class="sxs-lookup"><span data-stu-id="0cbba-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="0cbba-135">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="0cbba-135">Request elements</span></span>

<span data-ttu-id="0cbba-136">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="0cbba-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0cbba-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0cbba-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="0cbba-138">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="0cbba-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="0cbba-139">Exemplo de resposta de operação ResolveNames com êxito</span><span class="sxs-lookup"><span data-stu-id="0cbba-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="0cbba-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cbba-140">Description</span></span>

<span data-ttu-id="0cbba-141">O exemplo a seguir mostra uma resposta bem-sucedida para uma solicitação **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="0cbba-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0cbba-142">Código</span><span class="sxs-lookup"><span data-stu-id="0cbba-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="0cbba-143">Elementos de resposta resolvedos com êxito</span><span class="sxs-lookup"><span data-stu-id="0cbba-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="0cbba-144">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="0cbba-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0cbba-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0cbba-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0cbba-146">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="0cbba-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="0cbba-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0cbba-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0cbba-148">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0cbba-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="0cbba-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0cbba-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0cbba-150">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="0cbba-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="0cbba-151">Resolução</span><span class="sxs-lookup"><span data-stu-id="0cbba-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="0cbba-152">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="0cbba-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="0cbba-153">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="0cbba-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="0cbba-154">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="0cbba-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="0cbba-155">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="0cbba-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="0cbba-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="0cbba-156">MailboxType</span></span>](mailboxtype.md)
    
- [<span data-ttu-id="0cbba-157">Contato</span><span class="sxs-lookup"><span data-stu-id="0cbba-157">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="0cbba-158">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="0cbba-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="0cbba-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="0cbba-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="0cbba-160">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="0cbba-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="0cbba-161">Contato</span><span class="sxs-lookup"><span data-stu-id="0cbba-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="0cbba-162">Resposta de erro de operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0cbba-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="0cbba-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cbba-163">Description</span></span>

<span data-ttu-id="0cbba-164">O exemplo a seguir mostra uma resposta de erro para uma solicitação **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="0cbba-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="0cbba-165">O erro é causado pela tentativa de resolver um nome que não pode ser resolvido.</span><span class="sxs-lookup"><span data-stu-id="0cbba-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0cbba-166">Código</span><span class="sxs-lookup"><span data-stu-id="0cbba-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="0cbba-167">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="0cbba-167">Error response elements</span></span>

<span data-ttu-id="0cbba-168">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="0cbba-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="0cbba-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0cbba-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0cbba-170">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="0cbba-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="0cbba-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0cbba-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0cbba-172">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0cbba-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="0cbba-173">MessageText</span><span class="sxs-lookup"><span data-stu-id="0cbba-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0cbba-174">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0cbba-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0cbba-175">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0cbba-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="0cbba-176">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0cbba-176">See also</span></span>



[<span data-ttu-id="0cbba-177">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="0cbba-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="0cbba-178">Usando a resolução de nome</span><span class="sxs-lookup"><span data-stu-id="0cbba-178">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

