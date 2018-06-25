---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: O elemento EffectiveRights contém direitos do cliente com base nas configurações de permissão para o item ou a pasta. Este elemento é somente leitura.
ms.openlocfilehash: 610d9e214a8de648ece667799bb5e67dfcc358f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751972"
---
# <a name="effectiverights"></a><span data-ttu-id="c75e8-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c75e8-104">EffectiveRights</span></span>

<span data-ttu-id="c75e8-105">O elemento **EffectiveRights** contém direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="c75e8-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c75e8-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c75e8-106">This element is read-only.</span></span> 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 <span data-ttu-id="c75e8-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="c75e8-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c75e8-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c75e8-108">Attributes and elements</span></span>

<span data-ttu-id="c75e8-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c75e8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c75e8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c75e8-110">Attributes</span></span>

<span data-ttu-id="c75e8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c75e8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c75e8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c75e8-112">Child elements</span></span>

|<span data-ttu-id="c75e8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c75e8-113">**Element**</span></span>|<span data-ttu-id="c75e8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c75e8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c75e8-115">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="c75e8-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="c75e8-116">Indica se um cliente pode criar um índice de conteúdo associado.</span><span class="sxs-lookup"><span data-stu-id="c75e8-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="c75e8-117">Essa propriedade é usada somente em objetos de pasta.</span><span class="sxs-lookup"><span data-stu-id="c75e8-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-118">CreateContents</span><span class="sxs-lookup"><span data-stu-id="c75e8-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="c75e8-119">Indica se um cliente pode criar uma tabela de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c75e8-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="c75e8-120">Essa propriedade é usada somente em objetos de pasta.</span><span class="sxs-lookup"><span data-stu-id="c75e8-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-121">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="c75e8-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="c75e8-122">Indica se um cliente pode criar uma tabela de hierarquia.</span><span class="sxs-lookup"><span data-stu-id="c75e8-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="c75e8-123">Essa propriedade é usada somente em objetos de pasta.</span><span class="sxs-lookup"><span data-stu-id="c75e8-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-124">Delete</span><span class="sxs-lookup"><span data-stu-id="c75e8-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="c75e8-125">Indica se um cliente pode excluir uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c75e8-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-126">Modificar</span><span class="sxs-lookup"><span data-stu-id="c75e8-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="c75e8-127">Indica se um cliente pode modificar uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c75e8-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-128">Read</span><span class="sxs-lookup"><span data-stu-id="c75e8-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="c75e8-129">Indica se um cliente pode ler uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c75e8-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="c75e8-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="c75e8-131">Indica se um item particular pode ser exibido.</span><span class="sxs-lookup"><span data-stu-id="c75e8-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c75e8-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c75e8-132">Parent elements</span></span>

|<span data-ttu-id="c75e8-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c75e8-133">**Element**</span></span>|<span data-ttu-id="c75e8-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c75e8-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c75e8-135">Folder</span><span class="sxs-lookup"><span data-stu-id="c75e8-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="c75e8-136">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c75e8-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="c75e8-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="c75e8-138">Representa uma pasta de tarefas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c75e8-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="c75e8-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="c75e8-140">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c75e8-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="c75e8-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="c75e8-142">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c75e8-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="c75e8-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="c75e8-144">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c75e8-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-145">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c75e8-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c75e8-146">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-147">Contato</span><span class="sxs-lookup"><span data-stu-id="c75e8-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c75e8-148">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c75e8-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c75e8-150">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c75e8-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-151">1.1</span><span class="sxs-lookup"><span data-stu-id="c75e8-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="c75e8-152">Representa um item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c75e8-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c75e8-154">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c75e8-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c75e8-156">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c75e8-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c75e8-158">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c75e8-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c75e8-160">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-161">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c75e8-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c75e8-162">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-163">Task</span><span class="sxs-lookup"><span data-stu-id="c75e8-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="c75e8-164">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c75e8-165">PostItem</span><span class="sxs-lookup"><span data-stu-id="c75e8-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="c75e8-166">Representa um item de postagem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c75e8-167">Text value</span><span class="sxs-lookup"><span data-stu-id="c75e8-167">Text value</span></span>

<span data-ttu-id="c75e8-168">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c75e8-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c75e8-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="c75e8-169">Remarks</span></span>

<span data-ttu-id="c75e8-170">**EffectiveRights** é suportado nas respostas GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy e SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="c75e8-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="c75e8-171">A propriedade **EffectiveRights** é exposta na forma **AllProperties** para pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="c75e8-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="c75e8-172">Essa propriedade **EffectiveRights** fornece acesso às mesmas informações que são fornecidos na propriedade de **MAPI PR_ACCESS** .</span><span class="sxs-lookup"><span data-stu-id="c75e8-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="c75e8-173">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c75e8-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c75e8-174">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c75e8-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c75e8-175">Namespace</span><span class="sxs-lookup"><span data-stu-id="c75e8-175">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c75e8-176">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c75e8-176">Schema Name</span></span>  <br/> |<span data-ttu-id="c75e8-177">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c75e8-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="c75e8-178">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c75e8-178">Validation File</span></span>  <br/> |<span data-ttu-id="c75e8-179">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c75e8-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c75e8-180">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c75e8-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="c75e8-181">False</span><span class="sxs-lookup"><span data-stu-id="c75e8-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c75e8-182">Ver também</span><span class="sxs-lookup"><span data-stu-id="c75e8-182">See also</span></span>

- [<span data-ttu-id="c75e8-183">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c75e8-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c75e8-184">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="c75e8-184">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

