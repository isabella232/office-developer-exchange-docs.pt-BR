---
title: Setfolderfield
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
description: O elemento setfolderfield representa uma atualização que define o valor de uma única propriedade em uma pasta em uma operação UpdateFolder.
ms.openlocfilehash: ab75a3862801b9a7b3369d9a4116c653b461781c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530314"
---
# <a name="setfolderfield"></a><span data-ttu-id="2a4ba-103">Setfolderfield</span><span class="sxs-lookup"><span data-stu-id="2a4ba-103">SetFolderField</span></span>

<span data-ttu-id="2a4ba-104">O elemento **Setfolderfield** representa uma atualização que define o valor de uma única propriedade em uma pasta em uma operação UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

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


<span data-ttu-id="2a4ba-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="2a4ba-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2a4ba-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2a4ba-106">Attributes and elements</span></span>

<span data-ttu-id="2a4ba-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a4ba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2a4ba-108">Attributes</span></span>

<span data-ttu-id="2a4ba-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a4ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a4ba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2a4ba-110">Child elements</span></span>

|<span data-ttu-id="2a4ba-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2a4ba-111">**Element**</span></span>|<span data-ttu-id="2a4ba-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2a4ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a4ba-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="2a4ba-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="2a4ba-114">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2a4ba-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="2a4ba-116">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2a4ba-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="2a4ba-118">Identifica as propriedades de MAPI estendidas.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-119">Folder</span><span class="sxs-lookup"><span data-stu-id="2a4ba-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="2a4ba-120">Identifica uma pasta a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="2a4ba-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="2a4ba-122">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="2a4ba-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="2a4ba-124">Representa uma pasta contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="2a4ba-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="2a4ba-126">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a4ba-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="2a4ba-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="2a4ba-128">Representa uma pasta tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a4ba-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2a4ba-129">Parent elements</span></span>

|<span data-ttu-id="2a4ba-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2a4ba-130">**Element**</span></span>|<span data-ttu-id="2a4ba-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2a4ba-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a4ba-132">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="2a4ba-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="2a4ba-133">Contém um conjunto de elementos que define Append, set e Delete alterações nas propriedades da pasta.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2a4ba-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="2a4ba-134">Remarks</span></span>

<span data-ttu-id="2a4ba-135">Se a propriedade existir, o valor da propriedade será definido como o valor especificado.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="2a4ba-136">Se a propriedade não existir, a propriedade será criada com o valor especificado.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="2a4ba-137">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2a4ba-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a4ba-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2a4ba-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a4ba-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a4ba-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a4ba-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2a4ba-140">Schema Name</span></span>  <br/> |<span data-ttu-id="2a4ba-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2a4ba-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="2a4ba-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2a4ba-142">Validation File</span></span>  <br/> |<span data-ttu-id="2a4ba-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2a4ba-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a4ba-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2a4ba-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a4ba-145">False</span><span class="sxs-lookup"><span data-stu-id="2a4ba-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a4ba-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="2a4ba-146">See also</span></span>

- [<span data-ttu-id="2a4ba-147">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="2a4ba-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="2a4ba-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2a4ba-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

