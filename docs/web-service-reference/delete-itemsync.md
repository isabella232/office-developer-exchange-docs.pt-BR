---
title: Excluir (ItemSync)
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
description: O elemento de excluir identifica um único item a ser excluído no repositório de cliente local.
ms.openlocfilehash: 18b7ae2f97db2de64896680c3aa76f2590c03177
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751733"
---
# <a name="delete-itemsync"></a><span data-ttu-id="159f6-103">Excluir (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="159f6-103">Delete (ItemSync)</span></span>

<span data-ttu-id="159f6-104">O elemento de **Excluir** identifica um único item a ser excluído no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="159f6-104">The **Delete** element identifies a single item to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="159f6-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="159f6-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)  
- [<span data-ttu-id="159f6-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="159f6-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="159f6-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="159f6-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="159f6-108">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="159f6-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="159f6-109">Excluir (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="159f6-109">Delete (ItemSync)</span></span>](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

<span data-ttu-id="159f6-110">**SyncFolderItemsDeleteType**</span><span class="sxs-lookup"><span data-stu-id="159f6-110">**SyncFolderItemsDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="159f6-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="159f6-111">Attributes and elements</span></span>

<span data-ttu-id="159f6-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="159f6-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="159f6-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="159f6-113">Attributes</span></span>

<span data-ttu-id="159f6-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="159f6-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="159f6-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="159f6-115">Child elements</span></span>

|<span data-ttu-id="159f6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="159f6-116">**Element**</span></span>|<span data-ttu-id="159f6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="159f6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="159f6-118">ItemId</span><span class="sxs-lookup"><span data-stu-id="159f6-118">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="159f6-119">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="159f6-119">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="159f6-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="159f6-120">Parent elements</span></span>

|<span data-ttu-id="159f6-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="159f6-121">**Element**</span></span>|<span data-ttu-id="159f6-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="159f6-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="159f6-123">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="159f6-123">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="159f6-124">Contém uma matriz de sequência de tipos de alteração que representam o tipo das diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="159f6-124">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="159f6-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="159f6-125">Remarks</span></span>

<span data-ttu-id="159f6-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="159f6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="159f6-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="159f6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="159f6-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="159f6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="159f6-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="159f6-129">Schema name</span></span>  <br/> |<span data-ttu-id="159f6-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="159f6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="159f6-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="159f6-131">Validation file</span></span>  <br/> |<span data-ttu-id="159f6-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="159f6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="159f6-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="159f6-133">Can be empty</span></span>  <br/> |<span data-ttu-id="159f6-134">False</span><span class="sxs-lookup"><span data-stu-id="159f6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="159f6-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="159f6-135">See also</span></span>

- [<span data-ttu-id="159f6-136">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="159f6-136">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="159f6-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="159f6-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

