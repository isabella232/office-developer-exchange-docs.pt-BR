---
title: Operação ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: A operação ExpandDL expõe a associação completa de listas de distribuição.
ms.openlocfilehash: 8edaf057538e2c1136465f0ff7937c14477b2c47
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454047"
---
# <a name="expanddl-operation"></a><span data-ttu-id="8f1be-103">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8f1be-103">ExpandDL operation</span></span>

<span data-ttu-id="8f1be-104">A operação ExpandDL expõe a associação completa de listas de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8f1be-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="8f1be-105">Usando o método Web ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8f1be-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="8f1be-106">A operação ExpandDL usa o serviço Web localizado no Exchange. asmx.</span><span class="sxs-lookup"><span data-stu-id="8f1be-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="8f1be-107">Este método de serviço Web aceita um elemento de [caixa de correio](mailbox.md) que pode conter um elemento filho [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) para uma expansão de uma lista de distribuição pública ou um elemento filho [ItemId](itemid.md) para a expansão de uma lista de distribuição privada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="8f1be-108">As listas de distribuição pública podem ser expandidas usando um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="8f1be-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="8f1be-109">Alias da lista de distribuição</span><span class="sxs-lookup"><span data-stu-id="8f1be-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="8f1be-110">O endereço do Protocolo SMTP Seguro</span><span class="sxs-lookup"><span data-stu-id="8f1be-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="8f1be-111">X400</span><span class="sxs-lookup"><span data-stu-id="8f1be-111">X400</span></span>
    
4. <span data-ttu-id="8f1be-112">X500</span><span class="sxs-lookup"><span data-stu-id="8f1be-112">X500</span></span>
    
5. <span data-ttu-id="8f1be-113">Endereço herdado do Exchange</span><span class="sxs-lookup"><span data-stu-id="8f1be-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="8f1be-114">O nome da lista de distribuição</span><span class="sxs-lookup"><span data-stu-id="8f1be-114">The distribution list name</span></span>
    
7. <span data-ttu-id="8f1be-115">O nome de exibição</span><span class="sxs-lookup"><span data-stu-id="8f1be-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="8f1be-116">Os nomes de exibição não são exclusivos.</span><span class="sxs-lookup"><span data-stu-id="8f1be-116">Display names are not unique.</span></span> <span data-ttu-id="8f1be-117">Várias contas podem compartilhar o mesmo nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="8f1be-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8f1be-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f1be-118">Remarks</span></span>

<span data-ttu-id="8f1be-119">A expansão recursiva não é suportada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="8f1be-120">Apenas uma lista de distribuição pode ser expandida em uma única chamada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="8f1be-121">Se mais de uma lista de distribuição corresponder aos critérios, o serviço Web relatará um erro.</span><span class="sxs-lookup"><span data-stu-id="8f1be-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="8f1be-122">Um aplicativo cliente pode usar a ANR (resolução de nomes ambíguos) para localizar listas de distribuição ambíguas e, em seguida, escolher o endereço de email correto da lista de distribuição necessária como um parâmetro para a [operação ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8f1be-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="8f1be-123">Para obter mais informações, consulte [ResolveNames Operation](resolvenames-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8f1be-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="8f1be-124">As listas de distribuição pública estão localizadas no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8f1be-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="8f1be-125">Eles podem ser qualquer grupo de distribuição dinâmico ou habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="8f1be-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="8f1be-126">O grupo não deve ser oculto na lista de endereços e cada membro deve ter um endereço de email não vazio.</span><span class="sxs-lookup"><span data-stu-id="8f1be-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="8f1be-127">Os membros da lista de distribuição podem ser usuários e contatos habilitados para email, pastas públicas e listas de distribuição habilitadas para email e grupos dinâmicos.</span><span class="sxs-lookup"><span data-stu-id="8f1be-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="8f1be-128">As listas de distribuição privadas estão localizadas na pasta contatos da caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8f1be-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="8f1be-129">As listas de distribuição privada não têm endereços de email para que seus identificadores de item de repositório sejam usados em uma solicitação ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="8f1be-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="8f1be-130">Os membros de uma lista de distribuição privada podem ser qualquer usuário habilitado para email, contatos ou listas de distribuição do Active Directory ou de contatos ou listas de distribuição privada da pasta contatos de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8f1be-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="8f1be-131">Para contatos ou listas de distribuição privadas, os identificadores de item são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f1be-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="8f1be-132">Isso pode ser usado para obter informações sobre o objeto ou para expandir a associação em uma lista de distribuição privada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="8f1be-133">Exemplo de solicitação de lista de distribuição privada ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8f1be-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="8f1be-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1be-134">Description</span></span>

<span data-ttu-id="8f1be-135">O exemplo a seguir de uma solicitação ExpandDL mostra como formar uma solicitação para expandir uma lista de distribuição privada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="8f1be-136">Código</span><span class="sxs-lookup"><span data-stu-id="8f1be-136">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="8f1be-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f1be-137">Comments</span></span>

<span data-ttu-id="8f1be-138">Para expandir uma lista de distribuição privada, o elemento [Mailbox](mailbox.md) conterá o elemento [ItemId](itemid.md) que identifica uma lista de distribuição privada na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8f1be-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="8f1be-139">Exemplo de solicitação de lista de distribuição pública do ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8f1be-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="8f1be-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1be-140">Description</span></span>

<span data-ttu-id="8f1be-141">O exemplo a seguir de uma solicitação ExpandDL mostra como formar uma solicitação para expandir uma lista de distribuição pública.</span><span class="sxs-lookup"><span data-stu-id="8f1be-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="8f1be-142">O exemplo mostra o uso de um nome de exibição para expandir uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8f1be-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="8f1be-143">Código</span><span class="sxs-lookup"><span data-stu-id="8f1be-143">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="8f1be-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f1be-144">Comments</span></span>

<span data-ttu-id="8f1be-145">A resposta a essa solicitação conterá elementos de **caixa de correio** que identificam cada caixa de correio na lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8f1be-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="8f1be-146">Se uma lista de distribuição estiver contida em uma lista de distribuição, uma expansão de lista de distribuição separada deverá ser executada na lista de distribuição incorporada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="8f1be-147">Se a lista de distribuição não tiver membros ou a lista de distribuição solicitada não existir, o atributo **ResponseClass** conterá um valor igual a Success.</span><span class="sxs-lookup"><span data-stu-id="8f1be-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="8f1be-148">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="8f1be-148">Request elements</span></span>

<span data-ttu-id="8f1be-149">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="8f1be-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8f1be-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8f1be-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="8f1be-151">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="8f1be-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="8f1be-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é usado para identificar listas de distribuição públicas.</span><span class="sxs-lookup"><span data-stu-id="8f1be-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="8f1be-153">O elemento [ItemId](itemid.md) é usado para identificar listas de distribuição privadas.</span><span class="sxs-lookup"><span data-stu-id="8f1be-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8f1be-154">O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8f1be-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="8f1be-155">Exemplo de resposta ExpandDL bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="8f1be-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="8f1be-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1be-156">Description</span></span>

<span data-ttu-id="8f1be-157">O exemplo a seguir de uma resposta ExpandDL mostra uma resposta à solicitação descrita acima.</span><span class="sxs-lookup"><span data-stu-id="8f1be-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="8f1be-158">A expansão da lista de distribuição descreve o seguinte:</span><span class="sxs-lookup"><span data-stu-id="8f1be-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="8f1be-159">O número de membros da lista de distribuição que são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f1be-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="8f1be-160">Se a resposta contém todos os membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="8f1be-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="8f1be-161">O nome da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8f1be-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="8f1be-162">O endereço de email da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8f1be-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="8f1be-163">O tipo de roteamento para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8f1be-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="8f1be-164">O tipo de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8f1be-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="8f1be-165">O nome da lista de distribuição não está incluído na resposta; Portanto, você deve acompanhar o nome da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f1be-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8f1be-166">Código</span><span class="sxs-lookup"><span data-stu-id="8f1be-166">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="8f1be-167">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="8f1be-167">Successful response elements</span></span>

<span data-ttu-id="8f1be-168">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="8f1be-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="8f1be-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8f1be-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8f1be-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="8f1be-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="8f1be-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8f1be-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8f1be-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8f1be-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="8f1be-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8f1be-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8f1be-174">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="8f1be-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="8f1be-175">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="8f1be-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="8f1be-176">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="8f1be-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="8f1be-177">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="8f1be-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="8f1be-178">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="8f1be-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="8f1be-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="8f1be-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="8f1be-180">Para encontrar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="8f1be-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8f1be-181">Inicie no elemento [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="8f1be-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="8f1be-182">Resposta de erro ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8f1be-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="8f1be-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1be-183">Description</span></span>

<span data-ttu-id="8f1be-184">O exemplo a seguir mostra uma resposta de erro a uma solicitação ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="8f1be-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8f1be-185">Código</span><span class="sxs-lookup"><span data-stu-id="8f1be-185">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="8f1be-186">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="8f1be-186">Error response elements</span></span>

<span data-ttu-id="8f1be-187">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="8f1be-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="8f1be-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8f1be-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8f1be-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="8f1be-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="8f1be-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8f1be-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8f1be-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8f1be-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="8f1be-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="8f1be-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8f1be-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8f1be-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8f1be-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8f1be-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="8f1be-195">Para encontrar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="8f1be-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="8f1be-196">Inicie no elemento [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="8f1be-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8f1be-197">Também consulte</span><span class="sxs-lookup"><span data-stu-id="8f1be-197">See also</span></span>

- [<span data-ttu-id="8f1be-198">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8f1be-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="8f1be-199">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f1be-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

