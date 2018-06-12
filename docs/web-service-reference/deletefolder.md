---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: O elemento de DeleteFolder define uma solicitação para excluir pastas de uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751746"
---
# <a name="deletefolder"></a><span data-ttu-id="7498b-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="7498b-103">DeleteFolder</span></span>

<span data-ttu-id="7498b-104">O elemento de **DeleteFolder** define uma solicitação para excluir pastas de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7498b-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="7498b-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="7498b-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7498b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7498b-106">Attributes and elements</span></span>

<span data-ttu-id="7498b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7498b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7498b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7498b-108">Attributes</span></span>

|<span data-ttu-id="7498b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7498b-109">**Attribute**</span></span>|<span data-ttu-id="7498b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7498b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7498b-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="7498b-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="7498b-112">Descreve como uma pasta é excluída.</span><span class="sxs-lookup"><span data-stu-id="7498b-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="7498b-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="7498b-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="7498b-114">Atributo DeleteType</span><span class="sxs-lookup"><span data-stu-id="7498b-114">DeleteType attribute</span></span>

|<span data-ttu-id="7498b-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7498b-115">**Value**</span></span>|<span data-ttu-id="7498b-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7498b-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7498b-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="7498b-117">HardDelete</span></span>  <br/> |<span data-ttu-id="7498b-118">Uma pasta é removida permanentemente do repositório.</span><span class="sxs-lookup"><span data-stu-id="7498b-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="7498b-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="7498b-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="7498b-120">Uma pasta é movida para o dumpster se o dumpster está habilitado.</span><span class="sxs-lookup"><span data-stu-id="7498b-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="7498b-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="7498b-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="7498b-122">Uma pasta é movida para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="7498b-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7498b-123">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7498b-123">Child elements</span></span>

|<span data-ttu-id="7498b-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7498b-124">**Element**</span></span>|<span data-ttu-id="7498b-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7498b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7498b-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="7498b-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="7498b-127">Contém uma matriz de identificadores de pasta que são usados para identificar pastas para excluir.</span><span class="sxs-lookup"><span data-stu-id="7498b-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7498b-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7498b-128">Parent elements</span></span>

<span data-ttu-id="7498b-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7498b-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7498b-130">Text value</span><span class="sxs-lookup"><span data-stu-id="7498b-130">Text value</span></span>

<span data-ttu-id="7498b-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7498b-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7498b-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="7498b-132">Remarks</span></span>

<span data-ttu-id="7498b-133">As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que no momento em uma chamada de serviço da Web for concluído, o banco de dados tiver movido o item para a pasta Itens excluídos ou removido permanentemente o item do banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7498b-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="7498b-134">Esse comportamento é o mesmo para MicrosoftExchange Server 2007 e o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="7498b-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="7498b-135">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7498b-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7498b-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7498b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7498b-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="7498b-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7498b-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7498b-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7498b-139">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="7498b-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="7498b-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7498b-140">Validation File</span></span>  <br/> |<span data-ttu-id="7498b-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7498b-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7498b-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7498b-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7498b-143">False</span><span class="sxs-lookup"><span data-stu-id="7498b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7498b-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="7498b-144">See also</span></span>

- [<span data-ttu-id="7498b-145">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="7498b-145">DeleteFolder operation</span></span>](deletefolder-operation.md)

