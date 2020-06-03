---
title: SyncFolderHierarchyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponse
api_type:
- schema
ms.assetid: 7e6061d2-bbce-4864-a7bb-a6457628cb7c
description: O elemento SyncFolderHierarchyResponse define uma resposta a uma solicitação SyncFolderHierarchy.
ms.openlocfilehash: bf17ee9080405d308328197f7cbeb92e9b1e02d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456420"
---
# <a name="syncfolderhierarchyresponse"></a><span data-ttu-id="a3e60-103">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="a3e60-103">SyncFolderHierarchyResponse</span></span>

<span data-ttu-id="a3e60-104">O elemento **SyncFolderHierarchyResponse** define uma resposta a uma solicitação SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="a3e60-104">The **SyncFolderHierarchyResponse** element defines a response to a SyncFolderHierarchy request.</span></span> 
  
```xml
<SyncFolderHierarchyResponse>
   <ResponseMessages/>
</SyncFolderHierarchyResponse>
```

 <span data-ttu-id="a3e60-105">**SyncFolderHierarchyResponseType**</span><span class="sxs-lookup"><span data-stu-id="a3e60-105">**SyncFolderHierarchyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3e60-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a3e60-106">Attributes and elements</span></span>

<span data-ttu-id="a3e60-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a3e60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3e60-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a3e60-108">Attributes</span></span>

<span data-ttu-id="a3e60-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3e60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3e60-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a3e60-110">Child elements</span></span>

|<span data-ttu-id="a3e60-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3e60-111">**Element**</span></span>|<span data-ttu-id="a3e60-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3e60-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3e60-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a3e60-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a3e60-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3e60-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3e60-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a3e60-115">Parent elements</span></span>

<span data-ttu-id="a3e60-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3e60-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3e60-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3e60-117">Remarks</span></span>

<span data-ttu-id="a3e60-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a3e60-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3e60-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a3e60-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3e60-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3e60-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3e60-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a3e60-121">Schema name</span></span>  <br/> |<span data-ttu-id="a3e60-122">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a3e60-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="a3e60-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a3e60-123">Validation file</span></span>  <br/> |<span data-ttu-id="a3e60-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a3e60-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3e60-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a3e60-125">Can be empty</span></span>  <br/> |<span data-ttu-id="a3e60-126">False</span><span class="sxs-lookup"><span data-stu-id="a3e60-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3e60-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="a3e60-127">See also</span></span>



[<span data-ttu-id="a3e60-128">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a3e60-128">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="a3e60-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a3e60-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

