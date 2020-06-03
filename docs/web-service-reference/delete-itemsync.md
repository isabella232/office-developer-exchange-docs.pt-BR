---
title: Excluir (issync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: O elemento delete identifica um único item a ser excluído no repositório do cliente local.
ms.openlocfilehash: 6e30ddc7f7248fe7ff7136e19ba58c7d5d8a800f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454677"
---
# <a name="delete-itemsync"></a><span data-ttu-id="c1fe4-103">Excluir (issync)</span><span class="sxs-lookup"><span data-stu-id="c1fe4-103">Delete (ItemSync)</span></span>

<span data-ttu-id="c1fe4-104">O elemento **delete** identifica um único item a ser excluído no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="c1fe4-104">The **Delete** element identifies a single item to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="c1fe4-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="c1fe4-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)  
- [<span data-ttu-id="c1fe4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c1fe4-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="c1fe4-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c1fe4-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="c1fe4-108">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="c1fe4-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="c1fe4-109">Excluir (issync)</span><span class="sxs-lookup"><span data-stu-id="c1fe4-109">Delete (ItemSync)</span></span>](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

<span data-ttu-id="c1fe4-110">**SyncFolderItemsDeleteType**</span><span class="sxs-lookup"><span data-stu-id="c1fe4-110">**SyncFolderItemsDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c1fe4-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c1fe4-111">Attributes and elements</span></span>

<span data-ttu-id="c1fe4-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c1fe4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1fe4-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="c1fe4-113">Attributes</span></span>

<span data-ttu-id="c1fe4-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1fe4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1fe4-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c1fe4-115">Child elements</span></span>

|<span data-ttu-id="c1fe4-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1fe4-116">**Element**</span></span>|<span data-ttu-id="c1fe4-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1fe4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1fe4-118">ItemId</span><span class="sxs-lookup"><span data-stu-id="c1fe4-118">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c1fe4-119">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1fe4-119">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1fe4-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c1fe4-120">Parent elements</span></span>

|<span data-ttu-id="c1fe4-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1fe4-121">**Element**</span></span>|<span data-ttu-id="c1fe4-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1fe4-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1fe4-123">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="c1fe4-123">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="c1fe4-124">Contém uma matriz de sequência de tipos de alteração que representam o tipo de diferença entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1fe4-124">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1fe4-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="c1fe4-125">Remarks</span></span>

<span data-ttu-id="c1fe4-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c1fe4-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1fe4-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c1fe4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1fe4-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="c1fe4-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1fe4-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c1fe4-129">Schema name</span></span>  <br/> |<span data-ttu-id="c1fe4-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c1fe4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1fe4-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c1fe4-131">Validation file</span></span>  <br/> |<span data-ttu-id="c1fe4-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c1fe4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1fe4-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c1fe4-133">Can be empty</span></span>  <br/> |<span data-ttu-id="c1fe4-134">False</span><span class="sxs-lookup"><span data-stu-id="c1fe4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1fe4-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1fe4-135">See also</span></span>

- [<span data-ttu-id="c1fe4-136">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c1fe4-136">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="c1fe4-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1fe4-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

