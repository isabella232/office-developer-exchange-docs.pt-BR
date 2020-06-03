---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: O elemento BlockExternalImages especifica se as imagens externas são bloqueadas em corpos de texto HTML.
ms.openlocfilehash: 73342316024ebe476a0e35f14157befc80edcf83
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527401"
---
# <a name="blockexternalimages"></a><span data-ttu-id="4bdca-103">BlockExternalImages</span><span class="sxs-lookup"><span data-stu-id="4bdca-103">BlockExternalImages</span></span>

<span data-ttu-id="4bdca-104">O elemento **BlockExternalImages** especifica se as imagens externas são bloqueadas em corpos de texto HTML.</span><span class="sxs-lookup"><span data-stu-id="4bdca-104">The **BlockExternalImages** element specifies whether external images are blocked in HTML text bodies.</span></span> 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 <span data-ttu-id="4bdca-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4bdca-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bdca-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4bdca-106">Attributes and elements</span></span>

<span data-ttu-id="4bdca-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4bdca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bdca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4bdca-108">Attributes</span></span>

<span data-ttu-id="4bdca-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bdca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bdca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4bdca-110">Child elements</span></span>

<span data-ttu-id="4bdca-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4bdca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4bdca-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4bdca-112">Parent elements</span></span>

|<span data-ttu-id="4bdca-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4bdca-113">**Element**</span></span>|<span data-ttu-id="4bdca-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4bdca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bdca-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="4bdca-115">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="4bdca-116">Identifica as propriedades da pasta a serem incluídas na resposta GetFolder, FindFolder ou SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="4bdca-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span>  <br/> |
|[<span data-ttu-id="4bdca-117">Shape</span><span class="sxs-lookup"><span data-stu-id="4bdca-117">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="4bdca-118">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="4bdca-118">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4bdca-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4bdca-119">Text value</span></span>

<span data-ttu-id="4bdca-120">Um valor de texto **true** para o elemento **BlockExternalImages** indica que as imagens externas são bloqueadas em corpos de HTML.</span><span class="sxs-lookup"><span data-stu-id="4bdca-120">A text value of **true** for **BlockExternalImages** element indicates that external images are blocked in HTML bodies.</span></span> <span data-ttu-id="4bdca-121">Um valor **false** indica que as imagens externas são permitidas.</span><span class="sxs-lookup"><span data-stu-id="4bdca-121">A value of **false** indicates that external images are allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4bdca-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="4bdca-122">Remarks</span></span>

<span data-ttu-id="4bdca-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4bdca-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4bdca-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4bdca-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bdca-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4bdca-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bdca-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bdca-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4bdca-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4bdca-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4bdca-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4bdca-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4bdca-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4bdca-129">Validation File</span></span>  <br/> |<span data-ttu-id="4bdca-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4bdca-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4bdca-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4bdca-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4bdca-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="4bdca-132">See also</span></span>



- [<span data-ttu-id="4bdca-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4bdca-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

