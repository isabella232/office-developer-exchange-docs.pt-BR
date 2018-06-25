---
title: Estado de sincronização
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: O elemento de estado de sincronização contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização.
ms.openlocfilehash: 3c600dde09fd813dcfb1f6e74671ebe9004701a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837691"
---
# <a name="syncstate"></a><span data-ttu-id="0498b-104">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="0498b-104">SyncState</span></span>

<span data-ttu-id="0498b-105">O elemento de **estado de sincronização** contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="0498b-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="0498b-106">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0498b-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="0498b-107">**String**</span><span class="sxs-lookup"><span data-stu-id="0498b-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0498b-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0498b-108">Attributes and elements</span></span>

<span data-ttu-id="0498b-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0498b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0498b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0498b-110">Attributes</span></span>

<span data-ttu-id="0498b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0498b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0498b-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0498b-112">Child elements</span></span>

<span data-ttu-id="0498b-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0498b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0498b-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0498b-114">Parent elements</span></span>

|<span data-ttu-id="0498b-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0498b-115">**Element**</span></span>|<span data-ttu-id="0498b-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0498b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0498b-117">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="0498b-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="0498b-118">Define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.</span><span class="sxs-lookup"><span data-stu-id="0498b-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="0498b-119">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0498b-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="0498b-120">Contém o status e o resultado de uma solicitação de SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="0498b-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="0498b-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0498b-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="0498b-122">Define uma solicitação para sincronizar os itens em uma pasta de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0498b-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="0498b-123">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0498b-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="0498b-124">Contém o status e o resultado de uma solicitação de SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="0498b-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0498b-125">Text value</span><span class="sxs-lookup"><span data-stu-id="0498b-125">Text value</span></span>

<span data-ttu-id="0498b-126">Quando esse elemento é usado, é necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="0498b-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0498b-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="0498b-127">Remarks</span></span>

<span data-ttu-id="0498b-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0498b-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0498b-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0498b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0498b-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="0498b-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0498b-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0498b-131">Schema name</span></span>  <br/> |<span data-ttu-id="0498b-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0498b-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0498b-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0498b-133">Validation file</span></span>  <br/> |<span data-ttu-id="0498b-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0498b-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0498b-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0498b-135">Can be empty</span></span>  <br/> |<span data-ttu-id="0498b-136">False</span><span class="sxs-lookup"><span data-stu-id="0498b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0498b-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="0498b-137">See also</span></span>



[<span data-ttu-id="0498b-138">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0498b-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="0498b-139">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="0498b-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="0498b-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0498b-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

