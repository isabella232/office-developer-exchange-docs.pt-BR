---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: O elemento SearchFolder representa uma pasta de pesquisa que está contida em uma caixa de correio.
ms.openlocfilehash: d842c54dab7950c68e26804b676834c2d95debad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825302"
---
# <a name="searchfolder"></a><span data-ttu-id="299a1-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="299a1-103">SearchFolder</span></span>

<span data-ttu-id="299a1-104">O elemento **SearchFolder** representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="299a1-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
```xml
<SearchFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <SearchParameters/>
   <PermissionSet/>
      <EffectiveRights/>
</SearchFolder>
```

 <span data-ttu-id="299a1-105">**SearchFolderType**</span><span class="sxs-lookup"><span data-stu-id="299a1-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="299a1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="299a1-106">Attributes and elements</span></span>

<span data-ttu-id="299a1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="299a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="299a1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="299a1-108">Attributes</span></span>

<span data-ttu-id="299a1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="299a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="299a1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="299a1-110">Child elements</span></span>

|<span data-ttu-id="299a1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="299a1-111">**Element**</span></span>|<span data-ttu-id="299a1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="299a1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="299a1-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="299a1-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="299a1-114">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="299a1-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="299a1-116">Representa o identificador da pasta pai que contém a pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="299a1-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="299a1-118">Representa a classe de pasta para uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-119">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="299a1-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="299a1-120">Contém o nome de exibição de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="299a1-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="299a1-122">Representa a contagem total de itens dentro de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="299a1-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="299a1-124">Representa o número de pastas filho contida em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="299a1-125">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="299a1-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="299a1-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="299a1-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="299a1-127">Identifica as propriedades estendidas de pastas.</span><span class="sxs-lookup"><span data-stu-id="299a1-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="299a1-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="299a1-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="299a1-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="299a1-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="299a1-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="299a1-131">Representa a contagem de itens não lidos dentro de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-132">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="299a1-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="299a1-133">Contém os parâmetros que definem a uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="299a1-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="299a1-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="299a1-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="299a1-135">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="299a1-136">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="299a1-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="299a1-137">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="299a1-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="299a1-138">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="299a1-139">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="299a1-139">This element is read-only.</span></span> <span data-ttu-id="299a1-140">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="299a1-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="299a1-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="299a1-141">Parent elements</span></span>

|<span data-ttu-id="299a1-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="299a1-142">**Element**</span></span>|<span data-ttu-id="299a1-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="299a1-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="299a1-144">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="299a1-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="299a1-145">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="299a1-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="299a1-146">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="299a1-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="299a1-147">Identifica uma única pasta para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="299a1-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="299a1-148">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="299a1-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="299a1-149">Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="299a1-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="299a1-150">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="299a1-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="299a1-151">Identifica uma única pasta ao atualizar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="299a1-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="299a1-152">Pastas</span><span class="sxs-lookup"><span data-stu-id="299a1-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="299a1-153">Contém uma matriz de pastas usados nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="299a1-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="299a1-154">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="299a1-154">Remarks</span></span>

 <span data-ttu-id="299a1-155">**SearchFolder** é usado para as pastas de pesquisa comum e MicrosoftOfficeOutlook e Outlook Web Access visível pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="299a1-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="299a1-156">Para uma pasta de pesquisa fiquem visíveis para o Outlook e Outlook Web Access, a pasta deve ser criada na pasta diferenciada SearchFolders.</span><span class="sxs-lookup"><span data-stu-id="299a1-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="299a1-157">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="299a1-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="299a1-158">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="299a1-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="299a1-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="299a1-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="299a1-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="299a1-160">Schema Name</span></span>  <br/> |<span data-ttu-id="299a1-161">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="299a1-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="299a1-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="299a1-162">Validation File</span></span>  <br/> |<span data-ttu-id="299a1-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="299a1-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="299a1-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="299a1-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="299a1-165">False</span><span class="sxs-lookup"><span data-stu-id="299a1-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="299a1-166">Ver também</span><span class="sxs-lookup"><span data-stu-id="299a1-166">See also</span></span>



- [<span data-ttu-id="299a1-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="299a1-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

