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
description: O elemento de SyncFolderItems define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837686"
---
# <a name="syncfolderitems"></a><span data-ttu-id="5222b-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5222b-103">SyncFolderItems</span></span>

<span data-ttu-id="5222b-104">O elemento de **SyncFolderItems** define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5222b-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="5222b-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="5222b-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5222b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5222b-106">Attributes and elements</span></span>

<span data-ttu-id="5222b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5222b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5222b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5222b-108">Attributes</span></span>

<span data-ttu-id="5222b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5222b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5222b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5222b-110">Child elements</span></span>

|<span data-ttu-id="5222b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5222b-111">**Element**</span></span>|<span data-ttu-id="5222b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5222b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5222b-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5222b-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="5222b-114">Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="5222b-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="5222b-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5222b-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5222b-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="5222b-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="5222b-117">Representa a pasta que contém os itens a serem sincronizados.</span><span class="sxs-lookup"><span data-stu-id="5222b-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="5222b-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5222b-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5222b-119">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="5222b-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5222b-120">Contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="5222b-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="5222b-121">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5222b-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="5222b-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="5222b-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="5222b-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="5222b-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="5222b-124">Identifica os itens a serem ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="5222b-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="5222b-125">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="5222b-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="5222b-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="5222b-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="5222b-127">Descreve o número máximo de alterações que pode ser retornado em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5222b-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="5222b-128">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5222b-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5222b-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="5222b-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="5222b-130">Especifica se apenas itens ou itens e informações de pasta associada são retornados em uma resposta de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5222b-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="5222b-131">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="5222b-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5222b-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5222b-132">Parent elements</span></span>

<span data-ttu-id="5222b-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5222b-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5222b-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="5222b-134">Remarks</span></span>

<span data-ttu-id="5222b-135">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5222b-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5222b-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5222b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5222b-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="5222b-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5222b-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5222b-138">Schema name</span></span>  <br/> |<span data-ttu-id="5222b-139">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5222b-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="5222b-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5222b-140">Validation file</span></span>  <br/> |<span data-ttu-id="5222b-141">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5222b-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5222b-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5222b-142">Can be empty</span></span>  <br/> |<span data-ttu-id="5222b-143">False</span><span class="sxs-lookup"><span data-stu-id="5222b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5222b-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="5222b-144">See also</span></span>



[<span data-ttu-id="5222b-145">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5222b-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="5222b-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5222b-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

