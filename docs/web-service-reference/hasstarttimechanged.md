---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: O elemento HasStartTimeChanged Especifica se a hora de início para uma reunião foi alterada.
ms.openlocfilehash: 2096084f4ec8848a63d10e0e80fdc7a37e473cd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823809"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="e5520-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="e5520-103">HasStartTimeChanged</span></span>

<span data-ttu-id="e5520-104">O elemento **HasStartTimeChanged** Especifica se a hora de início para uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="e5520-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="e5520-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e5520-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5520-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e5520-106">Attributes and elements</span></span>

<span data-ttu-id="e5520-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e5520-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5520-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e5520-108">Attributes</span></span>

<span data-ttu-id="e5520-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e5520-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5520-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e5520-110">Child elements</span></span>

<span data-ttu-id="e5520-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e5520-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5520-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e5520-112">Parent elements</span></span>

|<span data-ttu-id="e5520-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e5520-113">**Element**</span></span>|<span data-ttu-id="e5520-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e5520-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5520-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="e5520-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="e5520-116">Especifica o que mudou entre duas versões de uma reunião mensagem de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5520-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5520-117">Text value</span><span class="sxs-lookup"><span data-stu-id="e5520-117">Text value</span></span>

<span data-ttu-id="e5520-118">Um valor de texto de **true** para o elemento **HasStartTimeChanged** indica que a hora de início para uma reunião foi alterado.</span><span class="sxs-lookup"><span data-stu-id="e5520-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="e5520-119">Um valor **false** indica que a hora de início não tiver sido alterado.</span><span class="sxs-lookup"><span data-stu-id="e5520-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e5520-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e5520-120">Remarks</span></span>

<span data-ttu-id="e5520-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e5520-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e5520-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5520-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5520-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e5520-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5520-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e5520-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5520-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e5520-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e5520-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="e5520-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e5520-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e5520-127">Validation File</span></span>  <br/> |<span data-ttu-id="e5520-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5520-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5520-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e5520-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e5520-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="e5520-130">See also</span></span>



- [<span data-ttu-id="e5520-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e5520-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

