---
title: Atualização (FolderSync)
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
description: O elemento Update identifica uma única pasta a ser atualizada no repositório do cliente local.
ms.openlocfilehash: 5c1b5b1fd87e4651125293eac431c56f732c6c02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467134"
---
# <a name="update-foldersync"></a><span data-ttu-id="48313-103">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="48313-103">Update (FolderSync)</span></span>

<span data-ttu-id="48313-104">O elemento **Update** identifica uma única pasta a ser atualizada no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="48313-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
- [<span data-ttu-id="48313-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="48313-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="48313-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="48313-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="48313-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="48313-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="48313-108">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="48313-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md) 
- [<span data-ttu-id="48313-109">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="48313-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
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

<span data-ttu-id="48313-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="48313-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="48313-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="48313-111">Attributes and elements</span></span>

<span data-ttu-id="48313-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="48313-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48313-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="48313-113">Attributes</span></span>

<span data-ttu-id="48313-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48313-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48313-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="48313-115">Child elements</span></span>

|<span data-ttu-id="48313-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="48313-116">**Element**</span></span>|<span data-ttu-id="48313-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48313-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48313-118">Folder</span><span class="sxs-lookup"><span data-stu-id="48313-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="48313-119">Define a pasta a ser criada, obtida, localizar, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="48313-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="48313-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="48313-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="48313-121">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="48313-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="48313-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="48313-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="48313-123">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="48313-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="48313-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="48313-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="48313-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="48313-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="48313-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="48313-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="48313-127">Representa uma pasta de tarefas t é thcontained em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="48313-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48313-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="48313-128">Parent elements</span></span>

|<span data-ttu-id="48313-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="48313-129">**Element**</span></span>|<span data-ttu-id="48313-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48313-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48313-131">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="48313-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="48313-132">Contém uma matriz em sequência de tipos de alteração que representam o tipo de diferença entre as pastas no cliente e as pastas no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="48313-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="48313-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="48313-133">Remarks</span></span>

<span data-ttu-id="48313-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="48313-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48313-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="48313-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48313-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="48313-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="48313-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="48313-137">Schema name</span></span>  <br/> |<span data-ttu-id="48313-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="48313-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="48313-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="48313-139">Validation file</span></span>  <br/> |<span data-ttu-id="48313-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="48313-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="48313-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="48313-141">Can be empty</span></span>  <br/> |<span data-ttu-id="48313-142">False</span><span class="sxs-lookup"><span data-stu-id="48313-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48313-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="48313-143">See also</span></span>

- [<span data-ttu-id="48313-144">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="48313-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="48313-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="48313-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

