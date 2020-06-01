---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: O elemento SyncFolderHierarchy define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.
ms.openlocfilehash: 68b607dbf603e955f74dfaccadd3ce6c4c9fb6ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466644"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="cad1e-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="cad1e-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="cad1e-104">O elemento **SyncFolderHierarchy** define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.</span><span class="sxs-lookup"><span data-stu-id="cad1e-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="cad1e-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="cad1e-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cad1e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cad1e-106">Attributes and elements</span></span>

<span data-ttu-id="cad1e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cad1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cad1e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cad1e-108">Attributes</span></span>

<span data-ttu-id="cad1e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cad1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cad1e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cad1e-110">Child elements</span></span>

|<span data-ttu-id="cad1e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cad1e-111">**Element**</span></span>|<span data-ttu-id="cad1e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cad1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cad1e-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="cad1e-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="cad1e-114">Identifica as propriedades da pasta a serem incluídas em uma resposta [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="cad1e-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="cad1e-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="cad1e-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="cad1e-116">Representa a pasta que contém os itens a serem sincronizados.</span><span class="sxs-lookup"><span data-stu-id="cad1e-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="cad1e-117">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="cad1e-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="cad1e-118">SyncState</span><span class="sxs-lookup"><span data-stu-id="cad1e-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cad1e-119">Contém uma forma codificada em base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="cad1e-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="cad1e-120">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cad1e-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cad1e-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cad1e-121">Parent elements</span></span>

<span data-ttu-id="cad1e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cad1e-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cad1e-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="cad1e-123">Remarks</span></span>

<span data-ttu-id="cad1e-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cad1e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cad1e-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cad1e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cad1e-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="cad1e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cad1e-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cad1e-127">Schema name</span></span>  <br/> |<span data-ttu-id="cad1e-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cad1e-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cad1e-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cad1e-129">Validation file</span></span>  <br/> |<span data-ttu-id="cad1e-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cad1e-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cad1e-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cad1e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="cad1e-132">False</span><span class="sxs-lookup"><span data-stu-id="cad1e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cad1e-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="cad1e-133">See also</span></span>



[<span data-ttu-id="cad1e-134">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="cad1e-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="cad1e-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cad1e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

