---
title: HasEndTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0eb444d-8e2e-478b-b785-2b9787ffb226
description: O elemento HasEndTimeChanged especifica se a hora de término de uma reunião foi alterada.
ms.openlocfilehash: 15ad52c7b7581cce5ca96ba5ff4e8a1c130a02cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461783"
---
# <a name="hasendtimechanged"></a><span data-ttu-id="e06ae-103">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="e06ae-103">HasEndTimeChanged</span></span>

<span data-ttu-id="e06ae-104">O elemento **HasEndTimeChanged** especifica se a hora de término de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="e06ae-104">The **HasEndTimeChanged** element specifies whether the end time for a meeting has changed.</span></span> 
  
```XML
<HasEndTimeChanged>true | false</HasEndTimeChanged>
```

 <span data-ttu-id="e06ae-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e06ae-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e06ae-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e06ae-106">Attributes and elements</span></span>

<span data-ttu-id="e06ae-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e06ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e06ae-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e06ae-108">Attributes</span></span>

<span data-ttu-id="e06ae-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e06ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e06ae-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e06ae-110">Child elements</span></span>

<span data-ttu-id="e06ae-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e06ae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e06ae-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e06ae-112">Parent elements</span></span>

|<span data-ttu-id="e06ae-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e06ae-113">**Element**</span></span>|<span data-ttu-id="e06ae-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e06ae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e06ae-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="e06ae-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="e06ae-116">Especifica o que mudou entre duas versões de uma mensagem de solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="e06ae-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e06ae-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e06ae-117">Text value</span></span>

<span data-ttu-id="e06ae-118">Um valor de texto **true** para o elemento **HasEndTimeChanged** indica que a hora de término de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="e06ae-118">A text value of **true** for the **HasEndTimeChanged** element indicates that the end time of a meeting has changed.</span></span> <span data-ttu-id="e06ae-119">Um valor **false** indica que a hora de término de uma reunião não foi alterada.</span><span class="sxs-lookup"><span data-stu-id="e06ae-119">A value of **false** indicates that the end time of a meeting has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e06ae-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="e06ae-120">Remarks</span></span>

<span data-ttu-id="e06ae-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e06ae-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e06ae-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e06ae-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e06ae-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e06ae-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e06ae-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e06ae-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e06ae-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e06ae-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e06ae-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="e06ae-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e06ae-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e06ae-127">Validation File</span></span>  <br/> |<span data-ttu-id="e06ae-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e06ae-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e06ae-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e06ae-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e06ae-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e06ae-130">See also</span></span>



- [<span data-ttu-id="e06ae-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e06ae-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

