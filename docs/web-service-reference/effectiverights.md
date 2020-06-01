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
description: O elemento EffectiveRights contém os direitos do cliente com base nas configurações de permissão para o item ou pasta. Este elemento é somente leitura.
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459241"
---
# <a name="effectiverights"></a><span data-ttu-id="c945c-104">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="c945c-104">EffectiveRights</span></span>

<span data-ttu-id="c945c-105">O elemento **EffectiveRights** contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="c945c-105">The **EffectiveRights** element contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="c945c-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c945c-106">This element is read-only.</span></span> 
  
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

 <span data-ttu-id="c945c-107">**EffectiveRightsType**</span><span class="sxs-lookup"><span data-stu-id="c945c-107">**EffectiveRightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c945c-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c945c-108">Attributes and elements</span></span>

<span data-ttu-id="c945c-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c945c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c945c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c945c-110">Attributes</span></span>

<span data-ttu-id="c945c-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c945c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c945c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c945c-112">Child elements</span></span>

|<span data-ttu-id="c945c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c945c-113">**Element**</span></span>|<span data-ttu-id="c945c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c945c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c945c-115">Createassociado</span><span class="sxs-lookup"><span data-stu-id="c945c-115">CreateAssociated</span></span>](createassociated.md) <br/> |<span data-ttu-id="c945c-116">Indica se um cliente pode criar uma tabela de conteúdo associado.</span><span class="sxs-lookup"><span data-stu-id="c945c-116">Indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="c945c-117">Esta propriedade só é usada em objetos Folder.</span><span class="sxs-lookup"><span data-stu-id="c945c-117">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="c945c-118">Createcontents</span><span class="sxs-lookup"><span data-stu-id="c945c-118">CreateContents</span></span>](createcontents.md) <br/> |<span data-ttu-id="c945c-119">Indica se um cliente pode criar uma tabela de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c945c-119">Indicates whether a client can create a contents table.</span></span> <span data-ttu-id="c945c-120">Esta propriedade só é usada em objetos Folder.</span><span class="sxs-lookup"><span data-stu-id="c945c-120">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="c945c-121">Createhierarchy</span><span class="sxs-lookup"><span data-stu-id="c945c-121">CreateHierarchy</span></span>](createhierarchy.md) <br/> |<span data-ttu-id="c945c-122">Indica se um cliente pode criar uma tabela de hierarquia.</span><span class="sxs-lookup"><span data-stu-id="c945c-122">Indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="c945c-123">Esta propriedade só é usada em objetos Folder.</span><span class="sxs-lookup"><span data-stu-id="c945c-123">This property is only used on folder objects.</span></span>  <br/> |
|[<span data-ttu-id="c945c-124">Delete</span><span class="sxs-lookup"><span data-stu-id="c945c-124">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="c945c-125">Indica se um cliente pode excluir uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c945c-125">Indicates whether a client can delete a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="c945c-126">Modificar</span><span class="sxs-lookup"><span data-stu-id="c945c-126">Modify</span></span>](modify.md) <br/> |<span data-ttu-id="c945c-127">Indica se um cliente pode modificar uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c945c-127">Indicates whether a client can modify a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="c945c-128">Leitura</span><span class="sxs-lookup"><span data-stu-id="c945c-128">Read</span></span>](read.md) <br/> |<span data-ttu-id="c945c-129">Indica se um cliente pode ler uma pasta ou item.</span><span class="sxs-lookup"><span data-stu-id="c945c-129">Indicates whether a client can read a folder or item.</span></span>  <br/> |
|[<span data-ttu-id="c945c-130">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="c945c-130">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="c945c-131">Indica se um item particular pode ser exibido.</span><span class="sxs-lookup"><span data-stu-id="c945c-131">Indicates whether a private item can be viewed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c945c-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c945c-132">Parent elements</span></span>

|<span data-ttu-id="c945c-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c945c-133">**Element**</span></span>|<span data-ttu-id="c945c-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c945c-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c945c-135">Folder</span><span class="sxs-lookup"><span data-stu-id="c945c-135">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="c945c-136">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c945c-136">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c945c-137">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="c945c-137">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="c945c-138">Representa uma pasta tarefas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c945c-138">Represents a tasks folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c945c-139">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="c945c-139">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="c945c-140">Representa uma pasta contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c945c-140">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c945c-141">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="c945c-141">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="c945c-142">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c945c-142">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c945c-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="c945c-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="c945c-144">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c945c-144">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c945c-145">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c945c-145">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c945c-146">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-146">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c945c-147">Contato</span><span class="sxs-lookup"><span data-stu-id="c945c-147">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c945c-148">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-148">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="c945c-149">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c945c-149">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c945c-150">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c945c-150">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c945c-151">Item</span><span class="sxs-lookup"><span data-stu-id="c945c-151">Item</span></span>](item.md) <br/> |<span data-ttu-id="c945c-152">Representa um item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-152">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c945c-153">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c945c-153">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c945c-154">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-154">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c945c-155">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c945c-155">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c945c-156">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-156">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c945c-157">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c945c-157">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c945c-158">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-158">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c945c-159">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c945c-159">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c945c-160">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-160">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c945c-161">Message</span><span class="sxs-lookup"><span data-stu-id="c945c-161">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c945c-162">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-162">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="c945c-163">Tarefa</span><span class="sxs-lookup"><span data-stu-id="c945c-163">Task</span></span>](task.md) <br/> |<span data-ttu-id="c945c-164">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-164">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c945c-165">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="c945c-165">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="c945c-166">Representa um item de postagem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-166">Represents a post item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c945c-167">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c945c-167">Text value</span></span>

<span data-ttu-id="c945c-168">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c945c-168">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c945c-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="c945c-169">Remarks</span></span>

<span data-ttu-id="c945c-170">**EffectiveRights** é suportado nas respostas GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy e SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="c945c-170">**EffectiveRights** is supported in the GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy, and SyncFolderItems responses.</span></span> <span data-ttu-id="c945c-171">A propriedade **EffectiveRights** é exposta na forma de **Propriedades** para pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="c945c-171">The **EffectiveRights** property is exposed in the **AllProperties** shape for folders and items.</span></span> 
  
<span data-ttu-id="c945c-172">Esta propriedade **EffectiveRights** fornece acesso às mesmas informações fornecidas na propriedade **PR_ACCESS MAPI** .</span><span class="sxs-lookup"><span data-stu-id="c945c-172">This **EffectiveRights** property provides access to the same information that is provided in the **PR_ACCESS MAPI** property.</span></span> 
  
<span data-ttu-id="c945c-173">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c945c-173">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c945c-174">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c945c-174">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c945c-175">Namespace</span><span class="sxs-lookup"><span data-stu-id="c945c-175">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c945c-176">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c945c-176">Schema Name</span></span>  <br/> |<span data-ttu-id="c945c-177">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c945c-177">Types schema</span></span>  <br/> |
|<span data-ttu-id="c945c-178">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c945c-178">Validation File</span></span>  <br/> |<span data-ttu-id="c945c-179">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c945c-179">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c945c-180">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c945c-180">Can be Empty</span></span>  <br/> |<span data-ttu-id="c945c-181">False</span><span class="sxs-lookup"><span data-stu-id="c945c-181">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c945c-182">Confira também</span><span class="sxs-lookup"><span data-stu-id="c945c-182">See also</span></span>

- [<span data-ttu-id="c945c-183">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c945c-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c945c-184">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="c945c-184">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

