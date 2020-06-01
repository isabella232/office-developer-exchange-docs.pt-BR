---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: O elemento AddBlankTargetToLinks especifica que o atributo de destino nos links HTML está definido para abrir uma nova janela.
ms.openlocfilehash: 1d4d36c1f4b98ebee96baea683c40527d2a9ec27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465040"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="48af0-103">AddBlankTargetToLinks</span><span class="sxs-lookup"><span data-stu-id="48af0-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="48af0-104">O elemento **AddBlankTargetToLinks** especifica que o atributo de destino nos links HTML está definido para abrir uma nova janela.</span><span class="sxs-lookup"><span data-stu-id="48af0-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="48af0-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="48af0-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="48af0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="48af0-106">Attributes and elements</span></span>

<span data-ttu-id="48af0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="48af0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48af0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="48af0-108">Attributes</span></span>

<span data-ttu-id="48af0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48af0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48af0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="48af0-110">Child elements</span></span>

<span data-ttu-id="48af0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="48af0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48af0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="48af0-112">Parent elements</span></span>

|<span data-ttu-id="48af0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="48af0-113">**Element**</span></span>|<span data-ttu-id="48af0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48af0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48af0-115">Shape</span><span class="sxs-lookup"><span data-stu-id="48af0-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="48af0-116">Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta **GetItem**, **FindItem**, **GetConversationItems** ou **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="48af0-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="48af0-117">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="48af0-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="48af0-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="48af0-118">Text value</span></span>

<span data-ttu-id="48af0-119">Um valor de texto **true** para o elemento **AddBlankTargetToLinks** indica que todos os links HTML serão definidos para abrir uma nova janela.</span><span class="sxs-lookup"><span data-stu-id="48af0-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="48af0-120">Um valor **false** indica que os links HTML serão abertos na janela atual.</span><span class="sxs-lookup"><span data-stu-id="48af0-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="48af0-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="48af0-121">Remarks</span></span>

<span data-ttu-id="48af0-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="48af0-122">This element is optional.</span></span>
  
<span data-ttu-id="48af0-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="48af0-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="48af0-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="48af0-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48af0-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="48af0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48af0-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="48af0-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="48af0-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="48af0-127">Schema Name</span></span>  <br/> |<span data-ttu-id="48af0-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="48af0-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="48af0-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="48af0-129">Validation File</span></span>  <br/> |<span data-ttu-id="48af0-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="48af0-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="48af0-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="48af0-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="48af0-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="48af0-132">See also</span></span>

- [<span data-ttu-id="48af0-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="48af0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

