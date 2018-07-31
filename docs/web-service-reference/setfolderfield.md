---
title: SetFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetFolderField
api_type:
- schema
ms.assetid: 8c69db7b-54b5-4ae2-abca-4d6e0937a790
description: O elemento SetFolderField representa uma atualização que define o valor para uma única propriedade em uma pasta em uma operação UpdateFolder.
ms.openlocfilehash: ed5c055c697865d5eb728d269c6f4c7ce60f4b5c
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353284"
---
# <a name="setfolderfield"></a><span data-ttu-id="37c6f-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="37c6f-103">SetFolderField</span></span>

<span data-ttu-id="37c6f-104">O elemento **SetFolderField** representa uma atualização que define o valor para uma única propriedade em uma pasta em uma operação UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="37c6f-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```
  
```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <SearchFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <Folder/> 
</SetFolderField>
```

```xml
<SetFolderField>
    <IndexedFieldURI/> 
    <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <TasksFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <Folder/>
</SetFolderField>
```

```xml
<SetFolderField>
    <FieldURI/> 
    <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <ContactsFolder/> 
</SetFolderField>
```


<span data-ttu-id="37c6f-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="37c6f-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="37c6f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="37c6f-106">Attributes and elements</span></span>

<span data-ttu-id="37c6f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="37c6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37c6f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="37c6f-108">Attributes</span></span>

<span data-ttu-id="37c6f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="37c6f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37c6f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="37c6f-110">Child elements</span></span>

|<span data-ttu-id="37c6f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37c6f-111">**Element**</span></span>|<span data-ttu-id="37c6f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37c6f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37c6f-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="37c6f-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="37c6f-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="37c6f-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="37c6f-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="37c6f-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="37c6f-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="37c6f-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="37c6f-118">Identifica as propriedades estendidas de MAPI.</span><span class="sxs-lookup"><span data-stu-id="37c6f-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-119">Folder</span><span class="sxs-lookup"><span data-stu-id="37c6f-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="37c6f-120">Identifica uma pasta a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="37c6f-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="37c6f-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="37c6f-122">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="37c6f-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="37c6f-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="37c6f-124">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="37c6f-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="37c6f-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="37c6f-126">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="37c6f-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="37c6f-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="37c6f-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="37c6f-128">Representa uma pasta de tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="37c6f-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37c6f-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="37c6f-129">Parent elements</span></span>

|<span data-ttu-id="37c6f-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37c6f-130">**Element**</span></span>|<span data-ttu-id="37c6f-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37c6f-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37c6f-132">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="37c6f-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="37c6f-133">Contém um conjunto de elementos que define append, definir e excluir as alterações nas propriedades da pasta.</span><span class="sxs-lookup"><span data-stu-id="37c6f-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="37c6f-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="37c6f-134">Remarks</span></span>

<span data-ttu-id="37c6f-135">Se a propriedade existir, o valor da propriedade é definido como o valor especificado.</span><span class="sxs-lookup"><span data-stu-id="37c6f-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="37c6f-136">Se a propriedade não existir, a propriedade é criada com o valor especificado.</span><span class="sxs-lookup"><span data-stu-id="37c6f-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="37c6f-137">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="37c6f-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37c6f-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="37c6f-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37c6f-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="37c6f-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37c6f-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="37c6f-140">Schema Name</span></span>  <br/> |<span data-ttu-id="37c6f-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="37c6f-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="37c6f-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="37c6f-142">Validation File</span></span>  <br/> |<span data-ttu-id="37c6f-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37c6f-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37c6f-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="37c6f-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="37c6f-145">False</span><span class="sxs-lookup"><span data-stu-id="37c6f-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37c6f-146">Ver também</span><span class="sxs-lookup"><span data-stu-id="37c6f-146">See also</span></span>

- [<span data-ttu-id="37c6f-147">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="37c6f-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="37c6f-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="37c6f-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

