---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: O elemento ReadItems indica se um usuário tem permissão para ler itens dentro de uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824964"
---
# <a name="readitems-calendarpermissiontype"></a><span data-ttu-id="37167-104">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="37167-104">ReadItems (CalendarPermissionType)</span></span>

<span data-ttu-id="37167-105">O elemento **ReadItems** indica se um usuário tem permissão para ler itens dentro de uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="37167-105">The **ReadItems** element indicates whether a user has permission to read items within a Calendar folder.</span></span> <span data-ttu-id="37167-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="37167-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 <span data-ttu-id="37167-107">**CalendarPermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="37167-107">**CalendarPermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37167-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="37167-108">Attributes and elements</span></span>

<span data-ttu-id="37167-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="37167-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37167-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="37167-110">Attributes</span></span>

<span data-ttu-id="37167-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="37167-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37167-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="37167-112">Child elements</span></span>

<span data-ttu-id="37167-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="37167-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37167-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="37167-114">Parent elements</span></span>

|<span data-ttu-id="37167-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37167-115">**Element**</span></span>|<span data-ttu-id="37167-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37167-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37167-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="37167-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="37167-118">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="37167-118">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="37167-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="37167-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37167-120">Text value</span><span class="sxs-lookup"><span data-stu-id="37167-120">Text value</span></span>

<span data-ttu-id="37167-121">A tabela a seguir lista os valores possíveis para o elemento **ReadItems** .</span><span class="sxs-lookup"><span data-stu-id="37167-121">The following table lists the possible values for the **ReadItems** element.</span></span> 
  
<span data-ttu-id="37167-122">**Valores de texto do elemento ReadItems**</span><span class="sxs-lookup"><span data-stu-id="37167-122">**ReadItems element text values**</span></span>

|<span data-ttu-id="37167-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="37167-123">**Value**</span></span>|<span data-ttu-id="37167-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37167-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="37167-125">None</span><span class="sxs-lookup"><span data-stu-id="37167-125">None</span></span>  <br/> |<span data-ttu-id="37167-126">Indica que o usuário não tem permissão para exibir itens do calendário.</span><span class="sxs-lookup"><span data-stu-id="37167-126">Indicates that the user does not have permission to view items in the calendar.</span></span>  <br/> |
|<span data-ttu-id="37167-127">TimeOnly</span><span class="sxs-lookup"><span data-stu-id="37167-127">TimeOnly</span></span>  <br/> |<span data-ttu-id="37167-128">Indica que o usuário tem permissão para exibir o tempo de disponibilidade apenas no calendário.</span><span class="sxs-lookup"><span data-stu-id="37167-128">Indicates that the user has permission to view only free/busy time in the calendar.</span></span>  <br/> |
|<span data-ttu-id="37167-129">TimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="37167-129">TimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="37167-130">Indica que o usuário tem permissão para exibir o tempo de disponibilidade no calendário e o assunto e o local de compromissos.</span><span class="sxs-lookup"><span data-stu-id="37167-130">Indicates that the user has permission to view free/busy time in the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="37167-131">FullDetails</span><span class="sxs-lookup"><span data-stu-id="37167-131">FullDetails</span></span>  <br/> |<span data-ttu-id="37167-132">Indica que o usuário tem permissão para exibir todos os itens do calendário, incluindo o tempo de livre/ocupado e assunto, local e detalhes dos compromissos.</span><span class="sxs-lookup"><span data-stu-id="37167-132">Indicates that the user has permission to view all items in the calendar, including free/busy time and subject, location, and details of appointments.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="37167-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="37167-133">Remarks</span></span>

<span data-ttu-id="37167-134">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="37167-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37167-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="37167-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37167-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="37167-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37167-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="37167-137">Schema Name</span></span>  <br/> |<span data-ttu-id="37167-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="37167-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="37167-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="37167-139">Validation File</span></span>  <br/> |<span data-ttu-id="37167-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37167-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37167-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="37167-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="37167-142">False</span><span class="sxs-lookup"><span data-stu-id="37167-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37167-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="37167-143">See also</span></span>



- [<span data-ttu-id="37167-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="37167-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="37167-145">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="37167-145">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

