---
title: Criar (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: 6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1
description: O elemento Create identifica uma única pasta a ser criada no armazenamento do cliente local.
ms.openlocfilehash: 43f6a6b3c084c8ecae767c512181bbdf50c7e786
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458373"
---
# <a name="create-foldersync"></a><span data-ttu-id="c191d-103">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c191d-103">Create (FolderSync)</span></span>

<span data-ttu-id="c191d-104">O elemento **Create** identifica uma única pasta a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="c191d-104">The **Create** element identifies a single folder to create in the local client store.</span></span> 
  
[<span data-ttu-id="c191d-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c191d-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="c191d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c191d-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c191d-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c191d-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="c191d-108">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="c191d-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="c191d-109">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c191d-109">Create (FolderSync)</span></span>](create-foldersync.md)
  
```xml
<Create>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</Create>
```

 <span data-ttu-id="c191d-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="c191d-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c191d-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c191d-111">Attributes and elements</span></span>

<span data-ttu-id="c191d-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c191d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c191d-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="c191d-113">Attributes</span></span>

<span data-ttu-id="c191d-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c191d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c191d-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c191d-115">Child elements</span></span>

|<span data-ttu-id="c191d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c191d-116">**Element**</span></span>|<span data-ttu-id="c191d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c191d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c191d-118">Folder</span><span class="sxs-lookup"><span data-stu-id="c191d-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="c191d-119">Define a pasta a ser criada, obtida, localizar, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="c191d-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="c191d-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="c191d-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="c191d-121">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="c191d-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="c191d-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="c191d-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="c191d-123">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c191d-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c191d-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="c191d-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="c191d-125">Representa uma pasta de pesquisa contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c191d-125">Represents a search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c191d-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="c191d-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="c191d-127">Representa uma pasta de tarefas contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c191d-127">Represents a task folder contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c191d-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c191d-128">Parent elements</span></span>

|<span data-ttu-id="c191d-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c191d-129">**Element**</span></span>|<span data-ttu-id="c191d-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c191d-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c191d-131">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="c191d-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="c191d-132">Contém uma matriz de sequência de tipos de alteração que representam o tipo de diferença entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="c191d-132">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c191d-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="c191d-133">Remarks</span></span>

<span data-ttu-id="c191d-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c191d-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c191d-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c191d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c191d-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="c191d-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c191d-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c191d-137">Schema name</span></span>  <br/> |<span data-ttu-id="c191d-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c191d-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="c191d-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c191d-139">Validation file</span></span>  <br/> |<span data-ttu-id="c191d-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c191d-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c191d-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c191d-141">Can be empty</span></span>  <br/> |<span data-ttu-id="c191d-142">False</span><span class="sxs-lookup"><span data-stu-id="c191d-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c191d-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="c191d-143">See also</span></span>



[<span data-ttu-id="c191d-144">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c191d-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="c191d-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c191d-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

