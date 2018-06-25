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
description: Os endereços de email ambíguo ResolveNames operação resolve e nomes para exibição.
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825162"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="a7dfd-103">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-103">ResolveNames operation</span></span>

<span data-ttu-id="a7dfd-104">Os endereços de email ambíguo **ResolveNames** operação resolve e nomes para exibição.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="a7dfd-105">Usando a operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="a7dfd-106">Esta operação pode ser usada para verificar aliases e resolver nomes para exibição para o usuário de caixa de correio apropriado.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="a7dfd-107">Se nomes ambíguos existirem, a resposta de operação **ResolveNames** fornece informações sobre cada usuário de caixa de correio para que o aplicativo cliente possa resolver os nomes.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a7dfd-108">Comentários</span><span class="sxs-lookup"><span data-stu-id="a7dfd-108">Remarks</span></span>

<span data-ttu-id="a7dfd-109">A resposta ResolveNames retorna um máximo de 100 candidatos.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="a7dfd-110">Os 100 candidatos que são retornados são os primeiros 100 encontradas na operação de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="a7dfd-111">Endereços de email com tipos de roteamento de prefixados, como smtp ou sip, são salvas em uma matriz de valores múltiplos.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="a7dfd-112">A operação **ResolveNames** realiza uma correspondência parcial contra cada valor dessa matriz, quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1@Contoso.com".</span><span class="sxs-lookup"><span data-stu-id="a7dfd-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="a7dfd-113">Se você não especificar um tipo de roteamento, **ResolveNames** será o padrão para o tipo de roteamento de smtp, associá-lo a uma propriedade de endereço smtp principal e não pesquisar a matriz de valores múltiplos.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="a7dfd-114">Apenas um nome ambíguo pode ser especificado em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="a7dfd-115">Active Directory é pesquisado primeiro e, em seguida, a pasta de contato do usuário é pesquisada.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="a7dfd-116">Resolvido entradas da pasta de contato de um usuário tem uma propriedade de **ItemId** não-nulo, que pode ser usada em uma solicitação de GetItem.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="a7dfd-117">Se for a ID de uma lista de distribuição particular, pode ser usada em uma [operação ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a7dfd-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="a7dfd-118">Se o atributo **ReturnFullContactData** for definido como **true**, entradas do Active Directory encontradas com a operação **ResolveNames** retornará propriedades adicionais que descrevem um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="a7dfd-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="a7dfd-119">O atributo **ReturnFullContactData** não afeta os dados que são retornados para contatos e privadas listas de distribuição da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="a7dfd-120">Exemplo de solicitação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="a7dfd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7dfd-121">Description</span></span>

<span data-ttu-id="a7dfd-122">O exemplo a seguir de uma solicitação de **ResolveNames** mostra como resolver a entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="a7dfd-123">Código</span><span class="sxs-lookup"><span data-stu-id="a7dfd-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a7dfd-124">Comments</span><span class="sxs-lookup"><span data-stu-id="a7dfd-124">Comments</span></span>

<span data-ttu-id="a7dfd-125">A resposta à solicitação retornará todas as entradas que começam com "Joana" ou "Mi".</span><span class="sxs-lookup"><span data-stu-id="a7dfd-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="a7dfd-126">Os itens retornados são caixas de correio públicas, listas de distribuição pública e privada e contatos.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a7dfd-127">Somente os contatos da pasta Contatos pessoal padrão são pesquisados.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="a7dfd-128">Estes são os resultados possíveis para uma solicitação de **ResolveNames** :</span><span class="sxs-lookup"><span data-stu-id="a7dfd-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="a7dfd-129">Respostas que não contêm uma entidade resolvida retornará um valor de atributo **ResponseClass** igual a **erro**.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="a7dfd-130">O elemento **MessageText** conterá " **Nenhum resultado é encontrado**."</span><span class="sxs-lookup"><span data-stu-id="a7dfd-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="a7dfd-131">As respostas que contêm uma única entidade resolvida retornará um valor de atributo **ResponseClass** igual ao **sucesso**.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="a7dfd-132">As respostas que contêm várias entidades possíveis retornará um valor de atributo **ResponseClass** igual a **Aviso**.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="a7dfd-133">Nesse caso, a entidade não pôde ser resolvida para uma identidade exclusiva.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="a7dfd-134">O elemento **MessageText** conterá "vários resultados encontrados."</span><span class="sxs-lookup"><span data-stu-id="a7dfd-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="a7dfd-135">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7dfd-135">Request elements</span></span>

<span data-ttu-id="a7dfd-136">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="a7dfd-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a7dfd-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="a7dfd-138">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="a7dfd-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="a7dfd-139">Exemplo de resposta bem-sucedida da operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="a7dfd-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7dfd-140">Description</span></span>

<span data-ttu-id="a7dfd-141">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="a7dfd-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a7dfd-142">Código</span><span class="sxs-lookup"><span data-stu-id="a7dfd-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="a7dfd-143">Elementos de resposta bem-sucedida ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="a7dfd-144">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="a7dfd-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a7dfd-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a7dfd-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a7dfd-146">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="a7dfd-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="a7dfd-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a7dfd-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a7dfd-148">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a7dfd-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="a7dfd-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a7dfd-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a7dfd-150">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="a7dfd-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="a7dfd-151">Resolução</span><span class="sxs-lookup"><span data-stu-id="a7dfd-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="a7dfd-152">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="a7dfd-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="a7dfd-153">Nome (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a7dfd-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="a7dfd-154">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a7dfd-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="a7dfd-155">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a7dfd-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="a7dfd-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="a7dfd-156">MailboxType</span></span>](mailboxtype.md)
    
- [<span data-ttu-id="a7dfd-157">Contato</span><span class="sxs-lookup"><span data-stu-id="a7dfd-157">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="a7dfd-158">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="a7dfd-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="a7dfd-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a7dfd-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="a7dfd-160">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a7dfd-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="a7dfd-161">ContactSource</span><span class="sxs-lookup"><span data-stu-id="a7dfd-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="a7dfd-162">Resposta de erro de operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a7dfd-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="a7dfd-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7dfd-163">Description</span></span>

<span data-ttu-id="a7dfd-164">O exemplo a seguir mostra uma resposta de erro a uma solicitação de **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="a7dfd-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="a7dfd-165">O erro é causado por tentar resolver um nome que não pode ser resolvido.</span><span class="sxs-lookup"><span data-stu-id="a7dfd-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a7dfd-166">Código</span><span class="sxs-lookup"><span data-stu-id="a7dfd-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="a7dfd-167">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="a7dfd-167">Error response elements</span></span>

<span data-ttu-id="a7dfd-168">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="a7dfd-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="a7dfd-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a7dfd-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a7dfd-170">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="a7dfd-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="a7dfd-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a7dfd-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a7dfd-172">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a7dfd-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="a7dfd-173">MessageText</span><span class="sxs-lookup"><span data-stu-id="a7dfd-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a7dfd-174">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a7dfd-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a7dfd-175">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a7dfd-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="a7dfd-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="a7dfd-176">See also</span></span>



[<span data-ttu-id="a7dfd-177">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a7dfd-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="a7dfd-178">Usando a resolução de nome</span><span class="sxs-lookup"><span data-stu-id="a7dfd-178">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

