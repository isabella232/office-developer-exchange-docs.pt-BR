---
title: Alterações (itens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: O elemento de alterações contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.
ms.openlocfilehash: 8e38597276e3e3051a5c1494619d3220280e401f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751387"
---
# <a name="changes-items"></a><span data-ttu-id="ae387-103">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="ae387-103">Changes (Items)</span></span>

<span data-ttu-id="ae387-104">O elemento de **alterações** contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae387-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="ae387-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="ae387-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="ae387-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ae387-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="ae387-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ae387-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="ae387-108">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="ae387-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="ae387-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="ae387-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae387-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ae387-110">Attributes and elements</span></span>

<span data-ttu-id="ae387-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ae387-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae387-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="ae387-112">Attributes</span></span>

<span data-ttu-id="ae387-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ae387-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae387-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ae387-114">Child elements</span></span>

|<span data-ttu-id="ae387-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae387-115">**Element**</span></span>|<span data-ttu-id="ae387-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae387-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae387-117">Criar (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ae387-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="ae387-118">Identifica um único item para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="ae387-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ae387-119">Atualização (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ae387-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="ae387-120">Identifica um único item a ser atualizado no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="ae387-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ae387-121">Excluir (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ae387-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="ae387-122">Identifica um único item a ser excluído no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="ae387-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ae387-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="ae387-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="ae387-124">Retornados em [operação SyncFolderItems](syncfolderitems-operation.md) respostas quando um item foi lido.</span><span class="sxs-lookup"><span data-stu-id="ae387-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="ae387-125">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae387-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae387-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ae387-126">Parent elements</span></span>

|<span data-ttu-id="ae387-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae387-127">**Element**</span></span>|<span data-ttu-id="ae387-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae387-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae387-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ae387-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="ae387-130">Contém o status e o resultado de uma solicitação de [operação SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ae387-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae387-131">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ae387-131">Remarks</span></span>

<span data-ttu-id="ae387-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ae387-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae387-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ae387-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae387-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae387-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae387-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ae387-135">Schema name</span></span>  <br/> |<span data-ttu-id="ae387-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ae387-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae387-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ae387-137">Validation file</span></span>  <br/> |<span data-ttu-id="ae387-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ae387-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae387-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ae387-139">Can be empty</span></span>  <br/> |<span data-ttu-id="ae387-140">False</span><span class="sxs-lookup"><span data-stu-id="ae387-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae387-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="ae387-141">See also</span></span>



[<span data-ttu-id="ae387-142">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ae387-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="ae387-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ae387-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

