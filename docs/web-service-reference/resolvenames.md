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
description: O elemento de ResolveNames define uma solicitação para resolver nomes de ambíguos.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825172"
---
# <a name="resolvenames"></a><span data-ttu-id="16169-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="16169-103">ResolveNames</span></span>

<span data-ttu-id="16169-104">O elemento de **ResolveNames** define uma solicitação para resolver nomes de ambíguos.</span><span class="sxs-lookup"><span data-stu-id="16169-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="16169-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="16169-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16169-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="16169-106">Attributes and elements</span></span>

<span data-ttu-id="16169-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="16169-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16169-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="16169-108">Attributes</span></span>

|<span data-ttu-id="16169-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="16169-109">**Attribute**</span></span>|<span data-ttu-id="16169-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16169-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16169-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="16169-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="16169-112">Descreve se os detalhes de contato completo para Contatos públicos para um nome resolvido são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="16169-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="16169-113">Este atributo é necessário para Contatos públicos.</span><span class="sxs-lookup"><span data-stu-id="16169-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="16169-114">Este valor não afeta privados contatos e listas de distribuição privada, para o qual [ItemId](itemid.md) sempre será retornado.</span><span class="sxs-lookup"><span data-stu-id="16169-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="16169-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="16169-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="16169-116">Identifica o escopo para uma pesquisa ResolveNames e ordem.</span><span class="sxs-lookup"><span data-stu-id="16169-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="16169-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="16169-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="16169-118">Identifica a propriedade definida retornada para contatos.</span><span class="sxs-lookup"><span data-stu-id="16169-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="16169-119">Este atributo foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="16169-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="16169-120">Valores de atributo ReturnFullContactData</span><span class="sxs-lookup"><span data-stu-id="16169-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="16169-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="16169-121">**Value**</span></span>|<span data-ttu-id="16169-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16169-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16169-123">True</span><span class="sxs-lookup"><span data-stu-id="16169-123">True</span></span>  <br/> |<span data-ttu-id="16169-124">Detalhes do contato completa para Contatos públicos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="16169-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="16169-125">False</span><span class="sxs-lookup"><span data-stu-id="16169-125">False</span></span>  <br/> |<span data-ttu-id="16169-126">Detalhes do contato completa para Contatos públicos não são retornados.</span><span class="sxs-lookup"><span data-stu-id="16169-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="16169-127">Valores de atributo SearchScope</span><span class="sxs-lookup"><span data-stu-id="16169-127">SearchScope attribute values</span></span>

|<span data-ttu-id="16169-128">**Valor**</span><span class="sxs-lookup"><span data-stu-id="16169-128">**Value**</span></span>|<span data-ttu-id="16169-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16169-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16169-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="16169-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="16169-131">O serviço de diretório do Active Directory é pesquisado.</span><span class="sxs-lookup"><span data-stu-id="16169-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="16169-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="16169-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="16169-133">Active Directory é pesquisado primeiro e, em seguida, as pastas de contato que são especificadas na propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="16169-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="16169-134">Contatos</span><span class="sxs-lookup"><span data-stu-id="16169-134">Contacts</span></span>  <br/> |<span data-ttu-id="16169-135">Somente as pastas de contato que são identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="16169-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="16169-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="16169-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="16169-137">Pastas de contatos são identificadas pela propriedade [ParentFolderIds](parentfolderids.md) são pesquisadas primeiro e, em seguida, o Active Directory é pesquisado.</span><span class="sxs-lookup"><span data-stu-id="16169-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="16169-138">Valores de atributo ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="16169-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="16169-139">**Valor**</span><span class="sxs-lookup"><span data-stu-id="16169-139">**Value**</span></span>|<span data-ttu-id="16169-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16169-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16169-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="16169-141">IdOnly</span></span>  <br/> |<span data-ttu-id="16169-142">A propriedade do identificador de item de contato é retornada.</span><span class="sxs-lookup"><span data-stu-id="16169-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="16169-143">Default</span><span class="sxs-lookup"><span data-stu-id="16169-143">Default</span></span>  <br/> |<span data-ttu-id="16169-144">O conjunto de propriedades de item de contato padrão será retornado.</span><span class="sxs-lookup"><span data-stu-id="16169-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="16169-145">Para obter mais informações, consulte [as formas de resposta no EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="16169-145">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="16169-146">AllProperties</span><span class="sxs-lookup"><span data-stu-id="16169-146">AllProperties</span></span>  <br/> |<span data-ttu-id="16169-147">O conjunto de AllProperties de propriedades de item de contato são retornadas.</span><span class="sxs-lookup"><span data-stu-id="16169-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="16169-148">Para obter mais informações, consulte [as formas de resposta no EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="16169-148">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="16169-149">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="16169-149">Child elements</span></span>

|<span data-ttu-id="16169-150">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="16169-150">**Element**</span></span>|<span data-ttu-id="16169-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16169-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16169-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="16169-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="16169-153">Contém uma matriz de identificadores de pasta de contato que seria ser pesquisada se o atributo **SearchScope** estiver definido como ActiveDirectoryContacts, contatos ou ContactsActiveDirectory.</span><span class="sxs-lookup"><span data-stu-id="16169-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="16169-154">A matriz ParentFolderIds só pode conter um identificador único de pasta de contato.</span><span class="sxs-lookup"><span data-stu-id="16169-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="16169-155">Se o elemento **ParentFolderIds** não estiver presente, a pasta padrão Contatos é pesquisada.</span><span class="sxs-lookup"><span data-stu-id="16169-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="16169-156">O identificador de pasta pode ser usado para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="16169-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="16169-157">Pesquisas do Active Directory são realizadas usando listas de controle de acesso (ACLs).</span><span class="sxs-lookup"><span data-stu-id="16169-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="16169-158">Alguns usuários talvez não tenha os direitos para ver alguns objetos do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16169-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="16169-159">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="16169-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="16169-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="16169-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="16169-161">Contém o nome de uma lista de contatos ou de distribuição para resolver.</span><span class="sxs-lookup"><span data-stu-id="16169-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="16169-162">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="16169-162">Parent elements</span></span>

<span data-ttu-id="16169-163">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16169-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="16169-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="16169-164">Remarks</span></span>

<span data-ttu-id="16169-165">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="16169-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16169-166">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="16169-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16169-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="16169-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="16169-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="16169-168">Schema name</span></span>  <br/> |<span data-ttu-id="16169-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="16169-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="16169-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="16169-170">Validation file</span></span>  <br/> |<span data-ttu-id="16169-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="16169-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="16169-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="16169-172">Can be empty</span></span>  <br/> |<span data-ttu-id="16169-173">False</span><span class="sxs-lookup"><span data-stu-id="16169-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16169-174">Ver também</span><span class="sxs-lookup"><span data-stu-id="16169-174">See also</span></span>



[<span data-ttu-id="16169-175">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="16169-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="16169-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="16169-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="16169-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="16169-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="16169-178">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="16169-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="16169-179">Usando a resolução de nome</span><span class="sxs-lookup"><span data-stu-id="16169-179">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

