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
description: O elemento changes contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.
ms.openlocfilehash: 6fda7b5602f172bae84ad7b211db2811def4f883
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463262"
---
# <a name="changes-items"></a><span data-ttu-id="5df27-103">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="5df27-103">Changes (Items)</span></span>

<span data-ttu-id="5df27-104">O elemento **Changes** contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5df27-104">The **Changes** element contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span> 
  
[<span data-ttu-id="5df27-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="5df27-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="5df27-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5df27-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="5df27-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5df27-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="5df27-108">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="5df27-108">Changes (Items)</span></span>](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="5df27-109">**SyncFolderItemsChangesType**</span><span class="sxs-lookup"><span data-stu-id="5df27-109">**SyncFolderItemsChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5df27-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5df27-110">Attributes and elements</span></span>

<span data-ttu-id="5df27-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5df27-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5df27-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="5df27-112">Attributes</span></span>

<span data-ttu-id="5df27-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5df27-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5df27-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5df27-114">Child elements</span></span>

|<span data-ttu-id="5df27-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5df27-115">**Element**</span></span>|<span data-ttu-id="5df27-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5df27-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5df27-117">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="5df27-117">Create (ItemSync)</span></span>](create-itemsync.md) <br/> |<span data-ttu-id="5df27-118">Identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="5df27-118">Identifies a single item to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5df27-119">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="5df27-119">Update (ItemSync)</span></span>](update-itemsync.md) <br/> |<span data-ttu-id="5df27-120">Identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="5df27-120">Identifies a single item to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5df27-121">Excluir (issync)</span><span class="sxs-lookup"><span data-stu-id="5df27-121">Delete (ItemSync)</span></span>](delete-itemsync.md) <br/> |<span data-ttu-id="5df27-122">Identifica um único item a ser excluído no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="5df27-122">Identifies a single item to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="5df27-123">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="5df27-123">ReadFlagChange</span></span>](readflagchange.md) <br/> |<span data-ttu-id="5df27-124">Retornado nas respostas da [operação SyncFolderItems](syncfolderitems-operation.md) quando um item foi lido.</span><span class="sxs-lookup"><span data-stu-id="5df27-124">Returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="5df27-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5df27-125">This property is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5df27-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5df27-126">Parent elements</span></span>

|<span data-ttu-id="5df27-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5df27-127">**Element**</span></span>|<span data-ttu-id="5df27-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5df27-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5df27-129">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5df27-129">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="5df27-130">Contém o status e o resultado de uma solicitação de [operação SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5df27-130">Contains the status and result of a [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5df27-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="5df27-131">Remarks</span></span>

<span data-ttu-id="5df27-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5df27-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5df27-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5df27-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5df27-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="5df27-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5df27-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5df27-135">Schema name</span></span>  <br/> |<span data-ttu-id="5df27-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5df27-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5df27-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5df27-137">Validation file</span></span>  <br/> |<span data-ttu-id="5df27-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5df27-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5df27-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5df27-139">Can be empty</span></span>  <br/> |<span data-ttu-id="5df27-140">False</span><span class="sxs-lookup"><span data-stu-id="5df27-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5df27-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="5df27-141">See also</span></span>



[<span data-ttu-id="5df27-142">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5df27-142">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="5df27-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5df27-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

