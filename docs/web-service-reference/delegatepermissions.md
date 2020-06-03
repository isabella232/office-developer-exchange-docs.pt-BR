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
description: O elemento DelegatePermissions contém as configurações de delegação de nível de permissão para um usuário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 2cf8c9a8d3c5db8e13d43c207df173c12fca5acb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457407"
---
# <a name="delegatepermissions"></a><span data-ttu-id="05729-104">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="05729-104">DelegatePermissions</span></span>

<span data-ttu-id="05729-105">O elemento **DelegatePermissions** contém as configurações de delegação de nível de permissão para um usuário.</span><span class="sxs-lookup"><span data-stu-id="05729-105">The **DelegatePermissions** element contains the delegate permission-level settings for a user.</span></span> <span data-ttu-id="05729-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="05729-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
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

<span data-ttu-id="05729-107">**DelegatePermissionsType**</span><span class="sxs-lookup"><span data-stu-id="05729-107">**DelegatePermissionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="05729-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="05729-108">Attributes and elements</span></span>

<span data-ttu-id="05729-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="05729-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05729-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="05729-110">Attributes</span></span>

<span data-ttu-id="05729-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05729-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05729-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="05729-112">Child elements</span></span>

|<span data-ttu-id="05729-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="05729-113">**Element**</span></span>|<span data-ttu-id="05729-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="05729-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05729-115">CalendarFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="05729-115">CalendarFolderPermissionLevel</span></span>](calendarfolderpermissionlevel.md) <br/> |<span data-ttu-id="05729-116">Contém as permissões para a pasta de calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="05729-116">Contains the permissions for the default Calendar folder.</span></span> <span data-ttu-id="05729-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="05729-118">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="05729-118">TasksFolderPermissionLevel</span></span>](tasksfolderpermissionlevel.md) <br/> |<span data-ttu-id="05729-119">Contém as permissões para a pasta de tarefas padrão.</span><span class="sxs-lookup"><span data-stu-id="05729-119">Contains the permissions for the default Task folder.</span></span> <span data-ttu-id="05729-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="05729-121">InboxFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="05729-121">InboxFolderPermissionLevel</span></span>](inboxfolderpermissionlevel.md) <br/> |<span data-ttu-id="05729-122">Contém as permissões para a pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="05729-122">Contains the permissions for the default Inbox folder.</span></span> <span data-ttu-id="05729-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="05729-124">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="05729-124">ContactsFolderPermissionLevel</span></span>](contactsfolderpermissionlevel.md) <br/> |<span data-ttu-id="05729-125">Contém as permissões para a pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="05729-125">Contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="05729-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="05729-127">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="05729-127">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md) <br/> |<span data-ttu-id="05729-128">Contém as permissões para a pasta padrão de anotações.</span><span class="sxs-lookup"><span data-stu-id="05729-128">Contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="05729-129">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="05729-130">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="05729-130">JournalFolderPermissionLevel</span></span>](journalfolderpermissionlevel.md) <br/> |<span data-ttu-id="05729-131">Contém as permissões para a pasta de diário padrão.</span><span class="sxs-lookup"><span data-stu-id="05729-131">Contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="05729-132">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05729-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="05729-133">Parent elements</span></span>

|<span data-ttu-id="05729-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="05729-134">**Element**</span></span>|<span data-ttu-id="05729-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="05729-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05729-136">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="05729-136">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="05729-137">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05729-137">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="05729-138">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="05729-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="05729-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="05729-139">Remarks</span></span>

<span data-ttu-id="05729-140">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="05729-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05729-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="05729-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05729-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="05729-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05729-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="05729-143">Schema Name</span></span>  <br/> |<span data-ttu-id="05729-144">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="05729-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="05729-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="05729-145">Validation File</span></span>  <br/> |<span data-ttu-id="05729-146">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="05729-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05729-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="05729-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="05729-148">False</span><span class="sxs-lookup"><span data-stu-id="05729-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05729-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="05729-149">See also</span></span>

- [<span data-ttu-id="05729-150">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="05729-150">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="05729-151">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="05729-151">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="05729-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="05729-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="05729-153">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="05729-153">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

