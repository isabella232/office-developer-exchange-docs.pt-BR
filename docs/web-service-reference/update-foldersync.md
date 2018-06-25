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
description: O elemento de atualização identifica uma única pasta ao atualizar no repositório de cliente local.
ms.openlocfilehash: 6d4a6233df41ea95e1fd9b394502bfb2728bddb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837873"
---
# <a name="update-foldersync"></a><span data-ttu-id="89355-103">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="89355-103">Update (FolderSync)</span></span>

<span data-ttu-id="89355-104">O elemento **Atualizar** identifica uma única pasta ao atualizar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="89355-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
[<span data-ttu-id="89355-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="89355-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="89355-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="89355-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="89355-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="89355-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="89355-108">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="89355-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="89355-109">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="89355-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

 <span data-ttu-id="89355-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="89355-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89355-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="89355-111">Attributes and elements</span></span>

<span data-ttu-id="89355-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="89355-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89355-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="89355-113">Attributes</span></span>

<span data-ttu-id="89355-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89355-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89355-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="89355-115">Child elements</span></span>

|<span data-ttu-id="89355-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89355-116">**Element**</span></span>|<span data-ttu-id="89355-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89355-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89355-118">Folder</span><span class="sxs-lookup"><span data-stu-id="89355-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="89355-119">Define a pasta para criar, obter, encontre, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="89355-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="89355-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="89355-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="89355-121">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="89355-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="89355-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="89355-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="89355-123">Representa uma pasta de contato em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="89355-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="89355-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="89355-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="89355-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="89355-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="89355-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="89355-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="89355-127">Representa uma tarefa pasta t é thcontained em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="89355-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89355-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="89355-128">Parent elements</span></span>

|<span data-ttu-id="89355-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89355-129">**Element**</span></span>|<span data-ttu-id="89355-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89355-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89355-131">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="89355-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="89355-132">Contém uma matriz sequenciada dos tipos de alteração que representam o tipo das diferenças entre as pastas no cliente e as pastas do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="89355-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89355-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="89355-133">Remarks</span></span>

<span data-ttu-id="89355-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="89355-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89355-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="89355-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89355-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="89355-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89355-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="89355-137">Schema name</span></span>  <br/> |<span data-ttu-id="89355-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="89355-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="89355-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="89355-139">Validation file</span></span>  <br/> |<span data-ttu-id="89355-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89355-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89355-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="89355-141">Can be empty</span></span>  <br/> |<span data-ttu-id="89355-142">False</span><span class="sxs-lookup"><span data-stu-id="89355-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89355-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="89355-143">See also</span></span>



[<span data-ttu-id="89355-144">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="89355-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="89355-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="89355-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

