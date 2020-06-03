---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: O elemento SyncFolderItems define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465146"
---
# <a name="syncfolderitems"></a><span data-ttu-id="1df48-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1df48-103">SyncFolderItems</span></span>

<span data-ttu-id="1df48-104">O elemento **SyncFolderItems** define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1df48-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="1df48-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="1df48-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1df48-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1df48-106">Attributes and elements</span></span>

<span data-ttu-id="1df48-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1df48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1df48-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1df48-108">Attributes</span></span>

<span data-ttu-id="1df48-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1df48-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1df48-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1df48-110">Child elements</span></span>

|<span data-ttu-id="1df48-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1df48-111">**Element**</span></span>|<span data-ttu-id="1df48-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1df48-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1df48-113">Shape</span><span class="sxs-lookup"><span data-stu-id="1df48-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="1df48-114">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="1df48-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="1df48-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1df48-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1df48-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="1df48-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="1df48-117">Representa a pasta que contém os itens a serem sincronizados.</span><span class="sxs-lookup"><span data-stu-id="1df48-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="1df48-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1df48-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1df48-119">SyncState</span><span class="sxs-lookup"><span data-stu-id="1df48-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1df48-120">Contém uma forma codificada em base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="1df48-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="1df48-121">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1df48-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="1df48-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1df48-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1df48-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="1df48-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="1df48-124">Identifica os itens a serem ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="1df48-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="1df48-125">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1df48-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1df48-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="1df48-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="1df48-127">Descreve o número máximo de alterações que podem ser retornadas em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1df48-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="1df48-128">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1df48-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1df48-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="1df48-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="1df48-130">Especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1df48-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="1df48-131">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="1df48-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1df48-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1df48-132">Parent elements</span></span>

<span data-ttu-id="1df48-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1df48-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1df48-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="1df48-134">Remarks</span></span>

<span data-ttu-id="1df48-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1df48-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1df48-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1df48-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1df48-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="1df48-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1df48-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1df48-138">Schema name</span></span>  <br/> |<span data-ttu-id="1df48-139">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1df48-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="1df48-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1df48-140">Validation file</span></span>  <br/> |<span data-ttu-id="1df48-141">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1df48-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1df48-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1df48-142">Can be empty</span></span>  <br/> |<span data-ttu-id="1df48-143">False</span><span class="sxs-lookup"><span data-stu-id="1df48-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1df48-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="1df48-144">See also</span></span>



[<span data-ttu-id="1df48-145">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="1df48-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="1df48-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1df48-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

