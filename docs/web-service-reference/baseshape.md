---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: O elemento BaseShape identifica o conjunto de propriedades para retornar em uma resposta de item ou uma pasta.
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751265"
---
# <a name="baseshape"></a><span data-ttu-id="4ff1f-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="4ff1f-103">BaseShape</span></span>

<span data-ttu-id="4ff1f-104">O elemento **BaseShape** identifica o conjunto de propriedades para retornar em uma resposta de item ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="4ff1f-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ff1f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4ff1f-106">Attributes and elements</span></span>

<span data-ttu-id="4ff1f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ff1f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ff1f-108">Attributes</span></span>

<span data-ttu-id="4ff1f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ff1f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ff1f-110">Child elements</span></span>

<span data-ttu-id="4ff1f-111">None</span><span class="sxs-lookup"><span data-stu-id="4ff1f-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ff1f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ff1f-112">Parent elements</span></span>

|<span data-ttu-id="4ff1f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-113">**Element**</span></span>|<span data-ttu-id="4ff1f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ff1f-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="4ff1f-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="4ff1f-116">Identifica as propriedades de pasta para incluir na resposta GetFolder, FindFolder ou SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="4ff1f-117">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="4ff1f-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="4ff1f-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="4ff1f-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="4ff1f-119">Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="4ff1f-120">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="4ff1f-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ff1f-121">Text value</span><span class="sxs-lookup"><span data-stu-id="4ff1f-121">Text value</span></span>

<span data-ttu-id="4ff1f-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-122">A text value is required.</span></span> <span data-ttu-id="4ff1f-123">A tabela a seguir lista os valores de texto possíveis.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="4ff1f-124">**Valores de texto para o elemento BaseShape**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="4ff1f-125">**Valor**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-125">**Value**</span></span>|<span data-ttu-id="4ff1f-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ff1f-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="4ff1f-127">IdOnly</span></span>  <br/> |<span data-ttu-id="4ff1f-128">Retorna apenas o ID de item ou uma pasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="4ff1f-129">Default</span><span class="sxs-lookup"><span data-stu-id="4ff1f-129">Default</span></span>  <br/> |<span data-ttu-id="4ff1f-130">Retorna um conjunto de propriedades que são definidas como padrão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="4ff1f-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="4ff1f-131">AllProperties</span></span>  <br/> |<span data-ttu-id="4ff1f-132">Retorna todas as propriedades utilizadas pela camada de lógica de negócios do Exchange para construir uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="4ff1f-133">A tabela a seguir lista as propriedades padrão que são retornadas para uma solicitação de FindFolder.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="4ff1f-134">Todas as subpastas de uma determinada pasta são retornadas em ordem pelo nome.</span><span class="sxs-lookup"><span data-stu-id="4ff1f-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="4ff1f-135">**Propriedades padrão**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-135">**Default properties**</span></span>

|<span data-ttu-id="4ff1f-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-136">**Folder**</span></span>|<span data-ttu-id="4ff1f-137">**Propriedades padrão**</span><span class="sxs-lookup"><span data-stu-id="4ff1f-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ff1f-138">Caixa de Entrada</span><span class="sxs-lookup"><span data-stu-id="4ff1f-138">Inbox</span></span>  <br/> |<span data-ttu-id="4ff1f-139">FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-140">Contatos</span><span class="sxs-lookup"><span data-stu-id="4ff1f-140">Contacts</span></span>  <br/> |<span data-ttu-id="4ff1f-141">FolderId, nome para exibição, a contagem total, a contagem de subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-142">Calendário</span><span class="sxs-lookup"><span data-stu-id="4ff1f-142">Calendar</span></span>  <br/> |<span data-ttu-id="4ff1f-143">FolderId, nome para exibição, contagem da subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-144">Rascunhos</span><span class="sxs-lookup"><span data-stu-id="4ff1f-144">Drafts</span></span>  <br/> |<span data-ttu-id="4ff1f-145">FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-146">Itens excluídos</span><span class="sxs-lookup"><span data-stu-id="4ff1f-146">Deleted items</span></span>  <br/> |<span data-ttu-id="4ff1f-147">FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-148">Outras pastas</span><span class="sxs-lookup"><span data-stu-id="4ff1f-148">Other folders</span></span>  <br/> |<span data-ttu-id="4ff1f-149">FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-150">Caixa de saída</span><span class="sxs-lookup"><span data-stu-id="4ff1f-150">Outbox</span></span>  <br/> |<span data-ttu-id="4ff1f-151">FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-152">Tarefas</span><span class="sxs-lookup"><span data-stu-id="4ff1f-152">Tasks</span></span>  <br/> |<span data-ttu-id="4ff1f-153">FolderId, nome para exibição, vencidos contagem, a contagem total, a contagem de subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="4ff1f-154">Observações</span><span class="sxs-lookup"><span data-stu-id="4ff1f-154">Notes</span></span>  <br/> |<span data-ttu-id="4ff1f-155">FolderId, nome para exibição, a contagem total, a contagem de subpasta</span><span class="sxs-lookup"><span data-stu-id="4ff1f-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ff1f-156">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4ff1f-156">Remarks</span></span>

<span data-ttu-id="4ff1f-157">Para retornar propriedades além daquelas identificado pelo elemento [BaseShape](baseshape.md) , use o elemento [AdditionalProperties](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="4ff1f-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="4ff1f-158">Example</span><span class="sxs-lookup"><span data-stu-id="4ff1f-158">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="4ff1f-159">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4ff1f-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ff1f-160">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ff1f-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ff1f-161">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ff1f-161">Schema Name</span></span>  <br/> |<span data-ttu-id="4ff1f-162">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4ff1f-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ff1f-163">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ff1f-163">Validation File</span></span>  <br/> |<span data-ttu-id="4ff1f-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ff1f-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ff1f-165">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4ff1f-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ff1f-166">False</span><span class="sxs-lookup"><span data-stu-id="4ff1f-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ff1f-167">Ver também</span><span class="sxs-lookup"><span data-stu-id="4ff1f-167">See also</span></span>

- [<span data-ttu-id="4ff1f-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="4ff1f-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="4ff1f-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="4ff1f-169">ItemShape</span></span>](itemshape.md)

