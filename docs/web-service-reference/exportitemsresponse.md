---
title: ExportItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponse
api_type:
- schema
ms.assetid: ef44354b-fbdb-4f7c-b6bd-b27f56a1d018
description: O elemento ExportItemsResponse representa a resposta a uma única solicitação ExportItems.
ms.openlocfilehash: 08033532d9cc381be8c544d790e9fe43840efb7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752149"
---
# <a name="exportitemsresponse"></a><span data-ttu-id="a8b1f-103">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="a8b1f-103">ExportItemsResponse</span></span>

<span data-ttu-id="a8b1f-104">O elemento **ExportItemsResponse** representa a resposta a uma única solicitação **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="a8b1f-104">The **ExportItemsResponse** element represents response to a single **ExportItems** request.</span></span> 
  
[<span data-ttu-id="a8b1f-105">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="a8b1f-105">ExportItemsResponse</span></span>](exportitemsresponse.md)
  
```XML
<ExportItemsResponse>
   <ResponseMessages/>
</ExportItemsResponse>
```

 <span data-ttu-id="a8b1f-106">**ExportItemsResponseType**</span><span class="sxs-lookup"><span data-stu-id="a8b1f-106">**ExportItemsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8b1f-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a8b1f-107">Attributes and elements</span></span>

<span data-ttu-id="a8b1f-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a8b1f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8b1f-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="a8b1f-109">Attributes</span></span>

<span data-ttu-id="a8b1f-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8b1f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8b1f-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a8b1f-111">Child elements</span></span>

|<span data-ttu-id="a8b1f-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a8b1f-112">**Element**</span></span>|<span data-ttu-id="a8b1f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a8b1f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8b1f-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a8b1f-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a8b1f-115">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8b1f-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8b1f-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a8b1f-116">Parent elements</span></span>

<span data-ttu-id="a8b1f-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8b1f-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a8b1f-118">Text value</span><span class="sxs-lookup"><span data-stu-id="a8b1f-118">Text value</span></span>

<span data-ttu-id="a8b1f-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8b1f-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8b1f-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="a8b1f-120">Remarks</span></span>

<span data-ttu-id="a8b1f-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8b1f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8b1f-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a8b1f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8b1f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8b1f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8b1f-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a8b1f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a8b1f-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="a8b1f-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="a8b1f-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a8b1f-126">Validation File</span></span>  <br/> |<span data-ttu-id="a8b1f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a8b1f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8b1f-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a8b1f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8b1f-129">False</span><span class="sxs-lookup"><span data-stu-id="a8b1f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8b1f-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="a8b1f-130">See also</span></span>



[<span data-ttu-id="a8b1f-131">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="a8b1f-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="a8b1f-132">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="a8b1f-132">UploadItems operation</span></span>](uploaditems-operation.md)

