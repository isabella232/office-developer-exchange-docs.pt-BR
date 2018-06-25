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
description: O elemento de SyncFolderHierarchy define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837682"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="b0c7c-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b0c7c-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="b0c7c-104">O elemento de **SyncFolderHierarchy** define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="b0c7c-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="b0c7c-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0c7c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b0c7c-106">Attributes and elements</span></span>

<span data-ttu-id="b0c7c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0c7c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b0c7c-108">Attributes</span></span>

<span data-ttu-id="b0c7c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0c7c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b0c7c-110">Child elements</span></span>

|<span data-ttu-id="b0c7c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0c7c-111">**Element**</span></span>|<span data-ttu-id="b0c7c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0c7c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0c7c-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="b0c7c-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="b0c7c-114">Identifica as propriedades de pasta para incluir em uma resposta [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c7c-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="b0c7c-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="b0c7c-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="b0c7c-116">Representa a pasta que contém os itens a serem sincronizados.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="b0c7c-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="b0c7c-118">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="b0c7c-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0c7c-119">Contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="b0c7c-120">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0c7c-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b0c7c-121">Parent elements</span></span>

<span data-ttu-id="b0c7c-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0c7c-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0c7c-123">Remarks</span></span>

<span data-ttu-id="b0c7c-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b0c7c-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0c7c-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b0c7c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0c7c-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0c7c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0c7c-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b0c7c-127">Schema name</span></span>  <br/> |<span data-ttu-id="b0c7c-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b0c7c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0c7c-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b0c7c-129">Validation file</span></span>  <br/> |<span data-ttu-id="b0c7c-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b0c7c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0c7c-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b0c7c-131">Can be empty</span></span>  <br/> |<span data-ttu-id="b0c7c-132">False</span><span class="sxs-lookup"><span data-stu-id="b0c7c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0c7c-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="b0c7c-133">See also</span></span>



[<span data-ttu-id="b0c7c-134">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b0c7c-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="b0c7c-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b0c7c-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

