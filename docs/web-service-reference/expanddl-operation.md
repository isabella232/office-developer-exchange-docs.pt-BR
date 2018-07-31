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
description: A operação ExpandDL expõe a participação completa das listas de distribuição.
ms.openlocfilehash: 4af6198ff15407b7fb71cdb4010ff6ce035460d0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353739"
---
# <a name="expanddl-operation"></a><span data-ttu-id="4105e-103">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="4105e-103">ExpandDL operation</span></span>

<span data-ttu-id="4105e-104">A operação ExpandDL expõe a participação completa das listas de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4105e-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="4105e-105">Usando o método ExpandDL da Web</span><span class="sxs-lookup"><span data-stu-id="4105e-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="4105e-106">A operação ExpandDL usa o serviço Web que está localizado em Exchange.asmx.</span><span class="sxs-lookup"><span data-stu-id="4105e-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="4105e-107">Este método de serviço Web aceita um elemento de [caixa de correio](mailbox.md) que pode conter um elemento filho de [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) uma expansão de uma lista de distribuição pública ou um elemento filho de [ItemId](itemid.md) para a expansão de uma privada lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4105e-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="4105e-108">Listas de distribuição pública podem ser expandidas usando um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="4105e-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="4105e-109">Alias de lista de distribuição</span><span class="sxs-lookup"><span data-stu-id="4105e-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="4105e-110">O endereço de Simple Mail Transfer Protocol (SMTP)</span><span class="sxs-lookup"><span data-stu-id="4105e-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="4105e-111">X400</span><span class="sxs-lookup"><span data-stu-id="4105e-111">X400</span></span>
    
4. <span data-ttu-id="4105e-112">X500</span><span class="sxs-lookup"><span data-stu-id="4105e-112">X500</span></span>
    
5. <span data-ttu-id="4105e-113">Endereço herdado do Exchange</span><span class="sxs-lookup"><span data-stu-id="4105e-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="4105e-114">O nome da lista de distribuição</span><span class="sxs-lookup"><span data-stu-id="4105e-114">The distribution list name</span></span>
    
7. <span data-ttu-id="4105e-115">O nome para exibição</span><span class="sxs-lookup"><span data-stu-id="4105e-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="4105e-116">Nomes de exibição não são exclusivos.</span><span class="sxs-lookup"><span data-stu-id="4105e-116">Display names are not unique.</span></span> <span data-ttu-id="4105e-117">Várias contas podem compartilhar o mesmo nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4105e-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4105e-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="4105e-118">Remarks</span></span>

<span data-ttu-id="4105e-119">Expansão recursiva não é suportado.</span><span class="sxs-lookup"><span data-stu-id="4105e-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="4105e-120">Lista de distribuição apenas um pode ser expandida em uma única chamada.</span><span class="sxs-lookup"><span data-stu-id="4105e-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="4105e-121">Se mais de uma lista de distribuição corresponde aos critérios, o serviço Web relata um erro.</span><span class="sxs-lookup"><span data-stu-id="4105e-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="4105e-122">Um aplicativo cliente pode usar a resolução de nome ambígua (ANR) para localizar a lista de distribuição ambígua e, em seguida, escolher o endereço de email correto da lista de distribuição necessários como um parâmetro para a [operação ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4105e-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="4105e-123">Para obter mais informações, consulte [ResolveNames operação](resolvenames-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4105e-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="4105e-124">Listas de distribuição pública estão localizadas no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4105e-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="4105e-125">Eles podem ser qualquer grupo de distribuição dinâmico ou habilitados para email.</span><span class="sxs-lookup"><span data-stu-id="4105e-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="4105e-126">O grupo não deve ser ocultado da lista de endereços e cada membro deve ter um endereço de email não vazias.</span><span class="sxs-lookup"><span data-stu-id="4105e-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="4105e-127">Membros da lista de distribuição podem ser habilitado para email usuários e contatos, pastas públicas e listas de distribuição habilitado para email e grupos dinâmicos.</span><span class="sxs-lookup"><span data-stu-id="4105e-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="4105e-128">Listas de distribuição privada estão localizadas na pasta de contatos da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4105e-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="4105e-129">Listas de distribuição privada não têm endereços de email para que seus identificadores de item do repositório que são usados em uma solicitação de ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="4105e-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="4105e-130">Membros de uma lista de distribuição privada podem ser qualquer usuário habilitado para email, contatos ou listas de distribuição do Active Directory, ou listas de contatos ou distribuição particular da pasta de contatos do usuário.</span><span class="sxs-lookup"><span data-stu-id="4105e-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="4105e-131">Para os contatos ou listas de distribuição privada, os identificadores de item são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="4105e-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="4105e-132">Isso pode ser usado para obter informações sobre o objeto ou para expandir a associação em uma lista de distribuição particular.</span><span class="sxs-lookup"><span data-stu-id="4105e-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="4105e-133">Exemplo de solicitação da lista de distribuição particular ExpandDL</span><span class="sxs-lookup"><span data-stu-id="4105e-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="4105e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4105e-134">Description</span></span>

<span data-ttu-id="4105e-135">O exemplo a seguir de uma solicitação de ExpandDL mostra como uma solicitação para expandir uma lista de distribuição particular de formulário.</span><span class="sxs-lookup"><span data-stu-id="4105e-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="4105e-136">Código</span><span class="sxs-lookup"><span data-stu-id="4105e-136">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

### <a name="comments"></a><span data-ttu-id="4105e-137">Comments</span><span class="sxs-lookup"><span data-stu-id="4105e-137">Comments</span></span>

<span data-ttu-id="4105e-138">Para expandir uma lista de distribuição particular, o elemento de [caixa de correio](mailbox.md) conterá o elemento [ItemId](itemid.md) que identifica uma lista de distribuição particular na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4105e-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="4105e-139">Exemplo de solicitação da lista de distribuição pública ExpandDL</span><span class="sxs-lookup"><span data-stu-id="4105e-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="4105e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="4105e-140">Description</span></span>

<span data-ttu-id="4105e-141">O exemplo a seguir de uma solicitação de ExpandDL mostra como uma solicitação para expandir uma lista de distribuição pública de formulário.</span><span class="sxs-lookup"><span data-stu-id="4105e-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="4105e-142">O exemplo mostra o uso de um nome de exibição para expandir uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4105e-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="4105e-143">Código</span><span class="sxs-lookup"><span data-stu-id="4105e-143">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="4105e-144">Comments</span><span class="sxs-lookup"><span data-stu-id="4105e-144">Comments</span></span>

<span data-ttu-id="4105e-145">A resposta à solicitação conterá elementos de **caixa de correio** que identificam cada caixa de correio na lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4105e-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="4105e-146">Se uma lista de distribuição está contida em uma lista de distribuição, uma expansão de lista de distribuição separado deve ser executada na lista de distribuição incorporadas.</span><span class="sxs-lookup"><span data-stu-id="4105e-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="4105e-147">Se a lista de distribuição não tem membros ou lista de distribuição solicitado não existir, o atributo **ResponseClass** conterá um valor igual ao sucesso.</span><span class="sxs-lookup"><span data-stu-id="4105e-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="4105e-148">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4105e-148">Request elements</span></span>

<span data-ttu-id="4105e-149">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="4105e-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4105e-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="4105e-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="4105e-151">Mailbox</span><span class="sxs-lookup"><span data-stu-id="4105e-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="4105e-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é usado para identificar as listas de distribuição pública.</span><span class="sxs-lookup"><span data-stu-id="4105e-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="4105e-153">O elemento [ItemId](itemid.md) é usado para identificar as listas de distribuição particular.</span><span class="sxs-lookup"><span data-stu-id="4105e-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4105e-154">O esquema que descreve esses elementos está localizado no diretório virtual EWS do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4105e-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="4105e-155">Exemplo de resposta bem-sucedida ExpandDL</span><span class="sxs-lookup"><span data-stu-id="4105e-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="4105e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="4105e-156">Description</span></span>

<span data-ttu-id="4105e-157">O exemplo a seguir de uma resposta ExpandDL mostra uma resposta à solicitação de descrito acima.</span><span class="sxs-lookup"><span data-stu-id="4105e-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="4105e-158">A expansão de lista de distribuição descreve o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4105e-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="4105e-159">O número de membros da lista de distribuição que são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="4105e-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="4105e-160">Se a resposta conterá todos os membros da lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="4105e-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="4105e-161">O nome da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4105e-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="4105e-162">O endereço de email da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4105e-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="4105e-163">O tipo de roteamento da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4105e-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="4105e-164">O tipo de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4105e-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="4105e-165">O nome da lista de distribuição não está incluído na resposta; Portanto, você deve ficar atento ao nome da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4105e-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4105e-166">Código</span><span class="sxs-lookup"><span data-stu-id="4105e-166">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="4105e-167">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="4105e-167">Successful response elements</span></span>

<span data-ttu-id="4105e-168">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="4105e-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4105e-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4105e-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4105e-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="4105e-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="4105e-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4105e-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4105e-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4105e-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="4105e-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4105e-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4105e-174">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="4105e-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="4105e-175">Mailbox</span><span class="sxs-lookup"><span data-stu-id="4105e-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="4105e-176">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4105e-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="4105e-177">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="4105e-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="4105e-178">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4105e-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="4105e-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="4105e-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="4105e-180">Para localizar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="4105e-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="4105e-181">Inicie o elemento [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="4105e-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="4105e-182">Resposta de erro ExpandDL</span><span class="sxs-lookup"><span data-stu-id="4105e-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="4105e-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="4105e-183">Description</span></span>

<span data-ttu-id="4105e-184">O exemplo a seguir mostra uma resposta de erro a uma solicitação de ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="4105e-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="4105e-185">Código</span><span class="sxs-lookup"><span data-stu-id="4105e-185">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="4105e-186">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="4105e-186">Error response elements</span></span>

<span data-ttu-id="4105e-187">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="4105e-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="4105e-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4105e-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4105e-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="4105e-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="4105e-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4105e-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4105e-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4105e-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="4105e-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="4105e-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4105e-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4105e-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4105e-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4105e-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="4105e-195">Para localizar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="4105e-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="4105e-196">Inicie o elemento [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="4105e-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4105e-197">Confira também</span><span class="sxs-lookup"><span data-stu-id="4105e-197">See also</span></span>

- [<span data-ttu-id="4105e-198">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="4105e-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="4105e-199">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4105e-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

