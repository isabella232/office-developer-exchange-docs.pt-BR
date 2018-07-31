---
title: Update (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: O elemento de atualização identifica uma única pasta ao atualizar no repositório de cliente local.
ms.openlocfilehash: bf49741b2478edff450f114dc1464a0528072bea
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353501"
---
# <a name="update-foldersync"></a><span data-ttu-id="9aaf9-103">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9aaf9-103">Update (FolderSync)</span></span>

<span data-ttu-id="9aaf9-104">O elemento **Atualizar** identifica uma única pasta ao atualizar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
- [<span data-ttu-id="9aaf9-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="9aaf9-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="9aaf9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9aaf9-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="9aaf9-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9aaf9-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="9aaf9-108">Changes (Hierarchy)</span><span class="sxs-lookup"><span data-stu-id="9aaf9-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md) 
- [<span data-ttu-id="9aaf9-109">Update (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9aaf9-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

```xml
<Update>
   <CalendarFolder/>
</Update>
```

```xml
<Update>
   <ContactsFolder/>
</Update>
```

```xml
<Update>
   <TasksFolder/>
</Update>
```

```xml
<Update>
   <SearchFolder/>
</Update>
```

<span data-ttu-id="9aaf9-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="9aaf9-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9aaf9-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9aaf9-111">Attributes and elements</span></span>

<span data-ttu-id="9aaf9-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9aaf9-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="9aaf9-113">Attributes</span></span>

<span data-ttu-id="9aaf9-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9aaf9-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9aaf9-115">Child elements</span></span>

|<span data-ttu-id="9aaf9-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9aaf9-116">**Element**</span></span>|<span data-ttu-id="9aaf9-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9aaf9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9aaf9-118">Folder</span><span class="sxs-lookup"><span data-stu-id="9aaf9-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9aaf9-119">Define a pasta para criar, obter, encontre, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="9aaf9-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="9aaf9-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="9aaf9-121">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="9aaf9-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="9aaf9-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9aaf9-123">Representa uma pasta de contato em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9aaf9-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9aaf9-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9aaf9-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9aaf9-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="9aaf9-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9aaf9-127">Representa uma tarefa pasta t é thcontained em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9aaf9-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9aaf9-128">Parent elements</span></span>

|<span data-ttu-id="9aaf9-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9aaf9-129">**Element**</span></span>|<span data-ttu-id="9aaf9-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9aaf9-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9aaf9-131">Changes (Hierarchy)</span><span class="sxs-lookup"><span data-stu-id="9aaf9-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="9aaf9-132">Contém uma matriz sequenciada dos tipos de alteração que representam o tipo das diferenças entre as pastas no cliente e as pastas do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9aaf9-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="9aaf9-133">Remarks</span></span>

<span data-ttu-id="9aaf9-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9aaf9-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9aaf9-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9aaf9-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9aaf9-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="9aaf9-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9aaf9-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9aaf9-137">Schema name</span></span>  <br/> |<span data-ttu-id="9aaf9-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9aaf9-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="9aaf9-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9aaf9-139">Validation file</span></span>  <br/> |<span data-ttu-id="9aaf9-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9aaf9-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9aaf9-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9aaf9-141">Can be empty</span></span>  <br/> |<span data-ttu-id="9aaf9-142">False</span><span class="sxs-lookup"><span data-stu-id="9aaf9-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9aaf9-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="9aaf9-143">See also</span></span>

- [<span data-ttu-id="9aaf9-144">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9aaf9-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="9aaf9-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9aaf9-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

