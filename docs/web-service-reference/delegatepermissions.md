---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: O elemento DelegatePermissions contém as configurações de nível de permissão do representante de um usuário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751718"
---
# <a name="delegatepermissions"></a><span data-ttu-id="addd0-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="addd0-104">DelegatePermissions</span></span>

<span data-ttu-id="addd0-105">O elemento **DelegatePermissions** contém as configurações de nível de permissão do representante de um usuário.</span><span class="sxs-lookup"><span data-stu-id="addd0-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="addd0-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="addd0-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

<span data-ttu-id="addd0-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="addd0-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="addd0-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="addd0-108">Attributes and elements</span></span>

<span data-ttu-id="addd0-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="addd0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="addd0-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="addd0-110">Attributes</span></span>

<span data-ttu-id="addd0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="addd0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="addd0-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="addd0-112">Child elements</span></span>

|<span data-ttu-id="addd0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="addd0-113">**Element**</span></span>|<span data-ttu-id="addd0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="addd0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="addd0-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="addd0-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="addd0-116">Contém as permissões para a pasta de calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="addd0-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="addd0-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="addd0-118">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="addd0-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="addd0-119">Contém as permissões para a pasta de tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="addd0-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="addd0-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="addd0-121">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="addd0-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="addd0-122">Contém as permissões para a pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="addd0-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="addd0-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="addd0-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="addd0-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="addd0-125">Contém as permissões para a pasta padrão Contatos.</span><span class="sxs-lookup"><span data-stu-id="addd0-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="addd0-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="addd0-127">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="addd0-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="addd0-128">Contém as permissões para a pasta de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="addd0-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="addd0-129">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="addd0-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="addd0-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="addd0-131">Contém as permissões para a pasta de diário padrão.</span><span class="sxs-lookup"><span data-stu-id="addd0-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="addd0-132">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="addd0-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="addd0-133">Parent elements</span></span>

|<span data-ttu-id="addd0-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="addd0-134">**Element**</span></span>|<span data-ttu-id="addd0-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="addd0-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="addd0-136">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="addd0-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="addd0-137">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="addd0-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="addd0-138">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="addd0-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="addd0-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="addd0-139">Remarks</span></span>

<span data-ttu-id="addd0-140">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="addd0-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="addd0-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="addd0-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="addd0-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="addd0-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="addd0-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="addd0-143">Schema Name</span></span>  <br/> |<span data-ttu-id="addd0-144">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="addd0-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="addd0-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="addd0-145">Validation File</span></span>  <br/> |<span data-ttu-id="addd0-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="addd0-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="addd0-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="addd0-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="addd0-148">False</span><span class="sxs-lookup"><span data-stu-id="addd0-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="addd0-149">Ver também</span><span class="sxs-lookup"><span data-stu-id="addd0-149">See also</span></span>

- [<span data-ttu-id="addd0-150">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="addd0-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="addd0-151">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="addd0-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="addd0-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="addd0-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="addd0-153">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="addd0-153">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

