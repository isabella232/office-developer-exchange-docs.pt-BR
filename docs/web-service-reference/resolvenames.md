---
title: ResolveNames
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
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: O elemento ResolveNames define uma solicitação para resolver nomes ambíguos.
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467946"
---
# <a name="resolvenames"></a><span data-ttu-id="10205-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="10205-103">ResolveNames</span></span>

<span data-ttu-id="10205-104">O elemento **ResolveNames** define uma solicitação para resolver nomes ambíguos.</span><span class="sxs-lookup"><span data-stu-id="10205-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="10205-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="10205-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10205-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="10205-106">Attributes and elements</span></span>

<span data-ttu-id="10205-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="10205-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10205-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="10205-108">Attributes</span></span>

|<span data-ttu-id="10205-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="10205-109">**Attribute**</span></span>|<span data-ttu-id="10205-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10205-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10205-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="10205-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="10205-112">Descreve se os detalhes do contato completo para contatos públicos para um nome resolvido são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="10205-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="10205-113">Este atributo é necessário para contatos públicos.</span><span class="sxs-lookup"><span data-stu-id="10205-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="10205-114">Esse valor não afeta contatos privados e listas de distribuição privada, para os quais o [ItemId](itemid.md) sempre é retornado.</span><span class="sxs-lookup"><span data-stu-id="10205-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="10205-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="10205-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="10205-116">Identifica a ordem e o escopo de uma pesquisa ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="10205-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="10205-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="10205-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="10205-118">Identifica o conjunto de propriedades retornado para os contatos.</span><span class="sxs-lookup"><span data-stu-id="10205-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="10205-119">Este atributo foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="10205-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="10205-120">Valores de atributo ReturnFullContactData</span><span class="sxs-lookup"><span data-stu-id="10205-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="10205-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="10205-121">**Value**</span></span>|<span data-ttu-id="10205-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10205-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10205-123">True</span><span class="sxs-lookup"><span data-stu-id="10205-123">True</span></span>  <br/> |<span data-ttu-id="10205-124">Detalhes de contato completo para contatos públicos são retornados.</span><span class="sxs-lookup"><span data-stu-id="10205-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="10205-125">Falso</span><span class="sxs-lookup"><span data-stu-id="10205-125">False</span></span>  <br/> |<span data-ttu-id="10205-126">Detalhes de contato completo para contatos públicos não são retornados.</span><span class="sxs-lookup"><span data-stu-id="10205-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="10205-127">Valores de atributo SearchScope</span><span class="sxs-lookup"><span data-stu-id="10205-127">SearchScope attribute values</span></span>

|<span data-ttu-id="10205-128">**Valor**</span><span class="sxs-lookup"><span data-stu-id="10205-128">**Value**</span></span>|<span data-ttu-id="10205-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10205-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10205-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="10205-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="10205-131">Somente o serviço de diretório do Active Directory é pesquisado.</span><span class="sxs-lookup"><span data-stu-id="10205-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="10205-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="10205-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="10205-133">O Active Directory é pesquisado primeiro e, em seguida, as pastas de contatos especificadas na propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="10205-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="10205-134">Contatos</span><span class="sxs-lookup"><span data-stu-id="10205-134">Contacts</span></span>  <br/> |<span data-ttu-id="10205-135">Somente as pastas de contatos identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="10205-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="10205-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="10205-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="10205-137">As pastas de contatos identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas primeiro e, em seguida, o Active Directory é pesquisado.</span><span class="sxs-lookup"><span data-stu-id="10205-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="10205-138">Valores de atributo ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="10205-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="10205-139">**Valor**</span><span class="sxs-lookup"><span data-stu-id="10205-139">**Value**</span></span>|<span data-ttu-id="10205-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10205-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10205-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="10205-141">IdOnly</span></span>  <br/> |<span data-ttu-id="10205-142">A propriedade de identificador de item de contato é retornada.</span><span class="sxs-lookup"><span data-stu-id="10205-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="10205-143">Padrão</span><span class="sxs-lookup"><span data-stu-id="10205-143">Default</span></span>  <br/> |<span data-ttu-id="10205-144">O conjunto padrão de propriedades de item de contato é retornado.</span><span class="sxs-lookup"><span data-stu-id="10205-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="10205-145">Para obter mais informações, consulte [as formas de resposta no EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="10205-145">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="10205-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10205-146">AllProperties</span></span>  <br/> |<span data-ttu-id="10205-147">O conjunto de propriedades de item de contato Propriedades é retornado.</span><span class="sxs-lookup"><span data-stu-id="10205-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="10205-148">Para obter mais informações, consulte [as formas de resposta no EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="10205-148">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="10205-149">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="10205-149">Child elements</span></span>

|<span data-ttu-id="10205-150">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="10205-150">**Element**</span></span>|<span data-ttu-id="10205-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10205-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10205-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="10205-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="10205-153">Contém uma matriz de identificadores de pasta de contato que seriam pesquisados se o atributo **SearchScope** estiver definido como ActiveDirectoryContacts, contatos ou ContactsActiveDirectory.</span><span class="sxs-lookup"><span data-stu-id="10205-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="10205-154">A matriz ParentFolderIds só pode conter um único identificador de pasta de contato.</span><span class="sxs-lookup"><span data-stu-id="10205-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="10205-155">Se o elemento **ParentFolderIds** não estiver presente, a pasta de contatos padrão será pesquisada.</span><span class="sxs-lookup"><span data-stu-id="10205-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="10205-156">O identificador de pasta pode ser usado para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="10205-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="10205-157">As pesquisas do Active Directory são realizadas usando ACLs (listas de controle de acesso).</span><span class="sxs-lookup"><span data-stu-id="10205-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="10205-158">Alguns usuários podem não ter os direitos para ver alguns objetos do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="10205-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="10205-159">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="10205-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="10205-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="10205-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="10205-161">Contém o nome de um contato ou de uma lista de distribuição a ser resolvido.</span><span class="sxs-lookup"><span data-stu-id="10205-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10205-162">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="10205-162">Parent elements</span></span>

<span data-ttu-id="10205-163">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10205-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="10205-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="10205-164">Remarks</span></span>

<span data-ttu-id="10205-165">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="10205-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10205-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="10205-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10205-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="10205-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="10205-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="10205-168">Schema name</span></span>  <br/> |<span data-ttu-id="10205-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="10205-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="10205-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="10205-170">Validation file</span></span>  <br/> |<span data-ttu-id="10205-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="10205-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="10205-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="10205-172">Can be empty</span></span>  <br/> |<span data-ttu-id="10205-173">False</span><span class="sxs-lookup"><span data-stu-id="10205-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10205-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="10205-174">See also</span></span>



[<span data-ttu-id="10205-175">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="10205-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="10205-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="10205-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="10205-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="10205-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="10205-178">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10205-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="10205-179">Usando a resolução de nome</span><span class="sxs-lookup"><span data-stu-id="10205-179">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

