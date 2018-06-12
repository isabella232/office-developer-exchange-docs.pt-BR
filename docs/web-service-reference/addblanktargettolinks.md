---
title: AddBlankTargetToLinks
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30180298-2501-4369-9b8f-2f7663f02336
description: O elemento AddBlankTargetToLinks Especifica que o atributo de destino em links HTML estão definidos para abrir uma nova janela.
ms.openlocfilehash: 8a47e44d89bcc84bc0e8b61d45f18ff3182f7870
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751042"
---
# <a name="addblanktargettolinks"></a><span data-ttu-id="e1f02-103">AddBlankTargetToLinks</span><span class="sxs-lookup"><span data-stu-id="e1f02-103">AddBlankTargetToLinks</span></span>

<span data-ttu-id="e1f02-104">O elemento **AddBlankTargetToLinks** Especifica que o atributo de destino em links HTML estão definidos para abrir uma nova janela.</span><span class="sxs-lookup"><span data-stu-id="e1f02-104">The **AddBlankTargetToLinks** element specifies that the target attribute in HTML links are set to open a new window.</span></span> 
  
```XML
<AddBlankTargetToLinks> true | false </AddBlankTargetToLinks>
```

<span data-ttu-id="e1f02-105">**xs:Boolean**</span><span class="sxs-lookup"><span data-stu-id="e1f02-105">**xs:Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e1f02-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e1f02-106">Attributes and elements</span></span>

<span data-ttu-id="e1f02-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1f02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1f02-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1f02-108">Attributes</span></span>

<span data-ttu-id="e1f02-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1f02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1f02-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1f02-110">Child elements</span></span>

<span data-ttu-id="e1f02-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1f02-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1f02-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1f02-112">Parent elements</span></span>

|<span data-ttu-id="e1f02-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1f02-113">**Element**</span></span>|<span data-ttu-id="e1f02-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1f02-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1f02-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e1f02-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="e1f02-116">Identifica as propriedades do item e o conteúdo a ser incluído em **GetItem**, **FindItem**, **GetConversationItems** ou resposta **SyncFolderItems** .</span><span class="sxs-lookup"><span data-stu-id="e1f02-116">Identifies the item properties and content to include in a **GetItem**, **FindItem**, **GetConversationItems** or **SyncFolderItems** response.</span></span><br/><br/>  <span data-ttu-id="e1f02-117">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="e1f02-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/>  `/GetConversationItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1f02-118">Text value</span><span class="sxs-lookup"><span data-stu-id="e1f02-118">Text value</span></span>

<span data-ttu-id="e1f02-119">Um valor de texto de **true** para o elemento **AddBlankTargetToLinks** indica que todos os links HTML serão definidos para abrir uma nova janela.</span><span class="sxs-lookup"><span data-stu-id="e1f02-119">A text value of **true** for the **AddBlankTargetToLinks** element indicates that all HTML links will be set to open a new window.</span></span> <span data-ttu-id="e1f02-120">Um valor **false** indica que os links HTML será aberta na janela atual.</span><span class="sxs-lookup"><span data-stu-id="e1f02-120">A value of **false** indicates that HTML links will open in the current window.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e1f02-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e1f02-121">Remarks</span></span>

<span data-ttu-id="e1f02-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e1f02-122">This element is optional.</span></span>
  
<span data-ttu-id="e1f02-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e1f02-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e1f02-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1f02-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1f02-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e1f02-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1f02-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1f02-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1f02-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1f02-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e1f02-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="e1f02-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e1f02-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1f02-129">Validation File</span></span>  <br/> |<span data-ttu-id="e1f02-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1f02-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1f02-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e1f02-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e1f02-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1f02-132">See also</span></span>

- [<span data-ttu-id="e1f02-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e1f02-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

