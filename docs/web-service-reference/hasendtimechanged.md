---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: O elemento HasEndTimeChanged Especifica se a hora de término para uma reunião foi alterada.
ms.openlocfilehash: 046bb302d6f7052c6f1757ce393583b305311e2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823805"
---
# <a name="hasendtimechanged"></a><span data-ttu-id="a8caf-103">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="a8caf-103">HasEndTimeChanged</span></span>

<span data-ttu-id="a8caf-104">O elemento **HasEndTimeChanged** Especifica se a hora de término para uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="a8caf-104">The **HasEndTimeChanged** element specifies whether the end time for a meeting has changed.</span></span> 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
```

 <span data-ttu-id="a8caf-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a8caf-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8caf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a8caf-106">Attributes and elements</span></span>

<span data-ttu-id="a8caf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a8caf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8caf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a8caf-108">Attributes</span></span>

<span data-ttu-id="a8caf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8caf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8caf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a8caf-110">Child elements</span></span>

<span data-ttu-id="a8caf-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8caf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8caf-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a8caf-112">Parent elements</span></span>

|<span data-ttu-id="a8caf-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a8caf-113">**Element**</span></span>|<span data-ttu-id="a8caf-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a8caf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8caf-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="a8caf-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="a8caf-116">Especifica o que mudou entre duas versões de uma reunião mensagem de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8caf-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8caf-117">Text value</span><span class="sxs-lookup"><span data-stu-id="a8caf-117">Text value</span></span>

<span data-ttu-id="a8caf-118">Um valor de texto de **true** para o elemento **HasEndTimeChanged** indica que a hora de término de uma reunião foi alterado.</span><span class="sxs-lookup"><span data-stu-id="a8caf-118">A text value of **true** for the **HasEndTimeChanged** element indicates that the end time of a meeting has changed.</span></span> <span data-ttu-id="a8caf-119">Um valor **false** indica que a hora de término de uma reunião não tiver sido alterado.</span><span class="sxs-lookup"><span data-stu-id="a8caf-119">A value of **false** indicates that the end time of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a8caf-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a8caf-120">Remarks</span></span>

<span data-ttu-id="a8caf-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a8caf-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a8caf-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8caf-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8caf-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a8caf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8caf-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8caf-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8caf-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a8caf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a8caf-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="a8caf-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a8caf-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a8caf-127">Validation File</span></span>  <br/> |<span data-ttu-id="a8caf-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8caf-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8caf-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a8caf-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a8caf-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="a8caf-130">See also</span></span>



- [<span data-ttu-id="a8caf-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a8caf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

