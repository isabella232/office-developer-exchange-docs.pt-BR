---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: O elemento BlockExternalImages Especifica se as imagens externas estarem bloqueadas em corpos de texto HTML.
ms.openlocfilehash: 41ab2ec7ec1c24ccbbef037ef1e27431c1fe6811
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751272"
---
# <a name="blockexternalimages"></a><span data-ttu-id="52b29-103">BlockExternalImages</span><span class="sxs-lookup"><span data-stu-id="52b29-103">BlockExternalImages</span></span>

<span data-ttu-id="52b29-104">O elemento **BlockExternalImages** Especifica se as imagens externas estarem bloqueadas em corpos de texto HTML.</span><span class="sxs-lookup"><span data-stu-id="52b29-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="52b29-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="52b29-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52b29-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="52b29-106">Attributes and elements</span></span>

<span data-ttu-id="52b29-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="52b29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52b29-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="52b29-108">Attributes</span></span>

<span data-ttu-id="52b29-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="52b29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52b29-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="52b29-110">Child elements</span></span>

<span data-ttu-id="52b29-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="52b29-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52b29-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="52b29-112">Parent elements</span></span>

|<span data-ttu-id="52b29-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="52b29-113">**Element**</span></span>|<span data-ttu-id="52b29-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52b29-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52b29-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="52b29-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="52b29-116">Identifica as propriedades de pasta para incluir na resposta GetFolder, FindFolder ou SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="52b29-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="52b29-117">ItemShape</span><span class="sxs-lookup"><span data-stu-id="52b29-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="52b29-118">Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="52b29-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52b29-119">Text value</span><span class="sxs-lookup"><span data-stu-id="52b29-119">Text value</span></span>

<span data-ttu-id="52b29-120">Um valor de **true** para o elemento **BlockExternalImages** text indica que imagens externas estarem bloqueadas em corpos HTML.</span><span class="sxs-lookup"><span data-stu-id="52b29-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="52b29-121">Um valor **false** indica que externos imagens são permitidas.</span><span class="sxs-lookup"><span data-stu-id="52b29-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="52b29-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="52b29-122">Remarks</span></span>

<span data-ttu-id="52b29-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="52b29-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="52b29-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="52b29-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52b29-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="52b29-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52b29-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="52b29-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52b29-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="52b29-127">Schema Name</span></span>  <br/> |<span data-ttu-id="52b29-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="52b29-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="52b29-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="52b29-129">Validation File</span></span>  <br/> |<span data-ttu-id="52b29-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52b29-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="52b29-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="52b29-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="52b29-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="52b29-132">See also</span></span>



- [<span data-ttu-id="52b29-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52b29-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

