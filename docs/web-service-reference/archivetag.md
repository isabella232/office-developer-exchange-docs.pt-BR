---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: O elemento ArchiveTag Especifica o identificador de retenção da marca archive definir em um item ou pasta.
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751203"
---
# <a name="archivetag"></a><span data-ttu-id="2686f-103">ArchiveTag</span><span class="sxs-lookup"><span data-stu-id="2686f-103">ArchiveTag</span></span>

<span data-ttu-id="2686f-104">O elemento **ArchiveTag** Especifica o identificador de retenção da marca archive definir em um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="2686f-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="2686f-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="2686f-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2686f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2686f-106">Attributes and elements</span></span>

<span data-ttu-id="2686f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2686f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2686f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2686f-108">Attributes</span></span>

|<span data-ttu-id="2686f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="2686f-109">**Attribute**</span></span>|<span data-ttu-id="2686f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2686f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2686f-111">**IsExplicit**</span><span class="sxs-lookup"><span data-stu-id="2686f-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="2686f-112">Especifica se a política de retenção é definida explicitamente em uma pasta ou um item ou se ela é herdada da pasta pai.</span><span class="sxs-lookup"><span data-stu-id="2686f-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2686f-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2686f-113">Child elements</span></span>

<span data-ttu-id="2686f-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2686f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2686f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2686f-115">Parent elements</span></span>

|<span data-ttu-id="2686f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2686f-116">**Element**</span></span>|<span data-ttu-id="2686f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2686f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2686f-118">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="2686f-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="2686f-119">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="2686f-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="2686f-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2686f-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2686f-121">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-121">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2686f-122">Contato</span><span class="sxs-lookup"><span data-stu-id="2686f-122">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2686f-123">Representa um item de contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2686f-124">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="2686f-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="2686f-125">Representa uma pasta de contatos que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2686f-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2686f-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="2686f-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="2686f-127">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="2686f-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="2686f-128">Folder</span><span class="sxs-lookup"><span data-stu-id="2686f-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="2686f-129">Define uma pasta para criar, obter, encontre, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="2686f-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="2686f-130">1.1</span><span class="sxs-lookup"><span data-stu-id="2686f-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="2686f-131">Representa um item genérico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2686f-132">Mensagem</span><span class="sxs-lookup"><span data-stu-id="2686f-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2686f-133">Representa uma mensagem de email do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="2686f-134">PostItem</span><span class="sxs-lookup"><span data-stu-id="2686f-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="2686f-135">Representa um item de postagem no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2686f-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="2686f-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="2686f-137">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2686f-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2686f-138">Task</span><span class="sxs-lookup"><span data-stu-id="2686f-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="2686f-139">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2686f-140">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="2686f-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="2686f-141">Representa uma pasta de tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2686f-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2686f-142">Text value</span><span class="sxs-lookup"><span data-stu-id="2686f-142">Text value</span></span>

<span data-ttu-id="2686f-143">O valor de texto do elemento **ArchiveTag** é um GUID que identifica a política de retenção.</span><span class="sxs-lookup"><span data-stu-id="2686f-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2686f-144">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2686f-144">Remarks</span></span>

<span data-ttu-id="2686f-145">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2686f-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2686f-146">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2686f-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2686f-147">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2686f-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2686f-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="2686f-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2686f-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2686f-149">Schema Name</span></span>  <br/> |<span data-ttu-id="2686f-150">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2686f-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="2686f-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2686f-151">Validation File</span></span>  <br/> |<span data-ttu-id="2686f-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2686f-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2686f-153">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2686f-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2686f-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="2686f-154">See also</span></span>

- [<span data-ttu-id="2686f-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2686f-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

