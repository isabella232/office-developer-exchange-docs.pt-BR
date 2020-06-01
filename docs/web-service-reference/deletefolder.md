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
description: O elemento DeleteFolder define uma solicitação para excluir pastas de uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: eb705a47b78b19c79b2e87561ba3696ed40e09cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458765"
---
# <a name="deletefolder"></a><span data-ttu-id="63182-103">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="63182-103">DeleteFolder</span></span>

<span data-ttu-id="63182-104">O elemento **DeleteFolder** define uma solicitação para excluir pastas de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="63182-104">The **DeleteFolder** element defines a request to delete folders from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 <span data-ttu-id="63182-105">**DeleteFolderType**</span><span class="sxs-lookup"><span data-stu-id="63182-105">**DeleteFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63182-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="63182-106">Attributes and elements</span></span>

<span data-ttu-id="63182-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="63182-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63182-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="63182-108">Attributes</span></span>

|<span data-ttu-id="63182-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="63182-109">**Attribute**</span></span>|<span data-ttu-id="63182-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="63182-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63182-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="63182-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="63182-112">Descreve como uma pasta é excluída.</span><span class="sxs-lookup"><span data-stu-id="63182-112">Describes how a folder is deleted.</span></span> <span data-ttu-id="63182-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="63182-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="63182-114">Atributo DeleteType</span><span class="sxs-lookup"><span data-stu-id="63182-114">DeleteType attribute</span></span>

|<span data-ttu-id="63182-115">**Valor**</span><span class="sxs-lookup"><span data-stu-id="63182-115">**Value**</span></span>|<span data-ttu-id="63182-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="63182-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63182-117">HardDelete</span><span class="sxs-lookup"><span data-stu-id="63182-117">HardDelete</span></span>  <br/> |<span data-ttu-id="63182-118">Uma pasta é removida permanentemente da loja.</span><span class="sxs-lookup"><span data-stu-id="63182-118">A folder is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="63182-119">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="63182-119">SoftDelete</span></span>  <br/> |<span data-ttu-id="63182-120">Uma pasta será movida para o dumpster se o dumpster estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="63182-120">A folder is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="63182-121">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="63182-121">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="63182-122">Uma pasta é movida para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="63182-122">A folder is moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="63182-123">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="63182-123">Child elements</span></span>

|<span data-ttu-id="63182-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="63182-124">**Element**</span></span>|<span data-ttu-id="63182-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="63182-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63182-126">FolderIds</span><span class="sxs-lookup"><span data-stu-id="63182-126">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="63182-127">Contém uma matriz de identificadores de pasta que são usados para identificar pastas a serem excluídas.</span><span class="sxs-lookup"><span data-stu-id="63182-127">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63182-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="63182-128">Parent elements</span></span>

<span data-ttu-id="63182-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63182-129">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="63182-130">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="63182-130">Text value</span></span>

<span data-ttu-id="63182-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="63182-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63182-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="63182-132">Remarks</span></span>

<span data-ttu-id="63182-133">As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que, quando uma chamada de serviço Web é concluída, o banco de dados moveu o item para a pasta itens excluídos ou removeu permanentemente o item do banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="63182-133">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="63182-134">Esse comportamento é o mesmo para o MicrosoftExchange Server 2007 e o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="63182-134">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="63182-135">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="63182-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63182-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="63182-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63182-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="63182-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63182-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="63182-138">Schema Name</span></span>  <br/> |<span data-ttu-id="63182-139">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="63182-139">Message schema</span></span>  <br/> |
|<span data-ttu-id="63182-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="63182-140">Validation File</span></span>  <br/> |<span data-ttu-id="63182-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="63182-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63182-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="63182-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="63182-143">False</span><span class="sxs-lookup"><span data-stu-id="63182-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63182-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="63182-144">See also</span></span>

- [<span data-ttu-id="63182-145">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="63182-145">DeleteFolder operation</span></span>](deletefolder-operation.md)

