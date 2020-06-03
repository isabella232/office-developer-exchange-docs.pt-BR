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
description: O elemento BaseShape identifica o conjunto de propriedades a ser retornado em uma resposta de item ou pasta.
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464487"
---
# <a name="baseshape"></a><span data-ttu-id="1f414-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="1f414-103">BaseShape</span></span>

<span data-ttu-id="1f414-104">O elemento **BaseShape** identifica o conjunto de propriedades a ser retornado em uma resposta de item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1f414-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="1f414-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="1f414-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f414-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1f414-106">Attributes and elements</span></span>

<span data-ttu-id="1f414-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1f414-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f414-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1f414-108">Attributes</span></span>

<span data-ttu-id="1f414-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f414-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f414-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1f414-110">Child elements</span></span>

<span data-ttu-id="1f414-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f414-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f414-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1f414-112">Parent elements</span></span>

|<span data-ttu-id="1f414-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1f414-113">**Element**</span></span>|<span data-ttu-id="1f414-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1f414-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f414-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="1f414-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="1f414-116">Identifica as propriedades da pasta a serem incluídas na resposta GetFolder, FindFolder ou SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="1f414-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="1f414-117">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="1f414-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="1f414-118">Shape</span><span class="sxs-lookup"><span data-stu-id="1f414-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="1f414-119">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="1f414-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="1f414-120">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="1f414-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f414-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1f414-121">Text value</span></span>

<span data-ttu-id="1f414-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f414-122">A text value is required.</span></span> <span data-ttu-id="1f414-123">A tabela a seguir lista os possíveis valores de texto.</span><span class="sxs-lookup"><span data-stu-id="1f414-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="1f414-124">**Valores de texto para o elemento BaseShape**</span><span class="sxs-lookup"><span data-stu-id="1f414-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="1f414-125">**Valor**</span><span class="sxs-lookup"><span data-stu-id="1f414-125">**Value**</span></span>|<span data-ttu-id="1f414-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1f414-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f414-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="1f414-127">IdOnly</span></span>  <br/> |<span data-ttu-id="1f414-128">Retorna somente a ID do item ou da pasta.</span><span class="sxs-lookup"><span data-stu-id="1f414-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="1f414-129">Padrão</span><span class="sxs-lookup"><span data-stu-id="1f414-129">Default</span></span>  <br/> |<span data-ttu-id="1f414-130">Retorna um conjunto de propriedades que são definidas como o padrão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1f414-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="1f414-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f414-131">AllProperties</span></span>  <br/> |<span data-ttu-id="1f414-132">Retorna todas as propriedades usadas pela camada de lógica de negócios do Exchange para criar uma pasta.</span><span class="sxs-lookup"><span data-stu-id="1f414-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="1f414-133">A tabela a seguir lista as propriedades padrão que são retornadas para uma solicitação FindFolder.</span><span class="sxs-lookup"><span data-stu-id="1f414-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="1f414-134">Todas as subpastas de uma determinada pasta são retornadas em ordem por nome.</span><span class="sxs-lookup"><span data-stu-id="1f414-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="1f414-135">**Propriedades padrão**</span><span class="sxs-lookup"><span data-stu-id="1f414-135">**Default properties**</span></span>

|<span data-ttu-id="1f414-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="1f414-136">**Folder**</span></span>|<span data-ttu-id="1f414-137">**Propriedades padrão**</span><span class="sxs-lookup"><span data-stu-id="1f414-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f414-138">Caixa de Entrada</span><span class="sxs-lookup"><span data-stu-id="1f414-138">Inbox</span></span>  <br/> |<span data-ttu-id="1f414-139">FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-140">Contatos</span><span class="sxs-lookup"><span data-stu-id="1f414-140">Contacts</span></span>  <br/> |<span data-ttu-id="1f414-141">FolderId, nome para exibição, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-142">Calendário</span><span class="sxs-lookup"><span data-stu-id="1f414-142">Calendar</span></span>  <br/> |<span data-ttu-id="1f414-143">FolderId, nome para exibição, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-144">Rascunhos</span><span class="sxs-lookup"><span data-stu-id="1f414-144">Drafts</span></span>  <br/> |<span data-ttu-id="1f414-145">FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-146">Itens excluídos</span><span class="sxs-lookup"><span data-stu-id="1f414-146">Deleted items</span></span>  <br/> |<span data-ttu-id="1f414-147">FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-148">Outras pastas</span><span class="sxs-lookup"><span data-stu-id="1f414-148">Other folders</span></span>  <br/> |<span data-ttu-id="1f414-149">FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-150">Enviada</span><span class="sxs-lookup"><span data-stu-id="1f414-150">Outbox</span></span>  <br/> |<span data-ttu-id="1f414-151">FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-152">Tarefas</span><span class="sxs-lookup"><span data-stu-id="1f414-152">Tasks</span></span>  <br/> |<span data-ttu-id="1f414-153">FolderId, nome de exibição, contagem atrasada, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="1f414-154">Observações</span><span class="sxs-lookup"><span data-stu-id="1f414-154">Notes</span></span>  <br/> |<span data-ttu-id="1f414-155">FolderId, nome para exibição, contagem total, contagem de subpastas</span><span class="sxs-lookup"><span data-stu-id="1f414-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f414-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="1f414-156">Remarks</span></span>

<span data-ttu-id="1f414-157">Para retornar propriedades além daquelas identificadas pelo elemento [BaseShape](baseshape.md) , use o elemento Properties [adicionais](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="1f414-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="1f414-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f414-158">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="1f414-159">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1f414-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f414-160">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f414-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f414-161">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1f414-161">Schema Name</span></span>  <br/> |<span data-ttu-id="1f414-162">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1f414-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f414-163">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1f414-163">Validation File</span></span>  <br/> |<span data-ttu-id="1f414-164">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1f414-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f414-165">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1f414-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f414-166">False</span><span class="sxs-lookup"><span data-stu-id="1f414-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f414-167">Confira também</span><span class="sxs-lookup"><span data-stu-id="1f414-167">See also</span></span>

- [<span data-ttu-id="1f414-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="1f414-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="1f414-169">Shape</span><span class="sxs-lookup"><span data-stu-id="1f414-169">ItemShape</span></span>](itemshape.md)

