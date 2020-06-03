---
title: HasStartTimeChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04a6968d-7fb5-47ee-b66e-dc99c35dbb63
description: O elemento HasStartTimeChanged especifica se a hora de início de uma reunião foi alterada.
ms.openlocfilehash: 1355917005d956d05064bfc095055fb72aa16c57
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462742"
---
# <a name="hasstarttimechanged"></a><span data-ttu-id="cd723-103">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="cd723-103">HasStartTimeChanged</span></span>

<span data-ttu-id="cd723-104">O elemento **HasStartTimeChanged** especifica se a hora de início de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="cd723-104">The **HasStartTimeChanged** element specifies whether the start time for a meeting has changed.</span></span> 
  
```XML
<HasStartTimeChanged> true | false </HasStartTimeChanged>
```

 <span data-ttu-id="cd723-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cd723-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd723-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cd723-106">Attributes and elements</span></span>

<span data-ttu-id="cd723-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cd723-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd723-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cd723-108">Attributes</span></span>

<span data-ttu-id="cd723-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd723-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd723-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cd723-110">Child elements</span></span>

<span data-ttu-id="cd723-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd723-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd723-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cd723-112">Parent elements</span></span>

|<span data-ttu-id="cd723-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd723-113">**Element**</span></span>|<span data-ttu-id="cd723-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd723-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd723-115">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="cd723-115">ChangeHighlights</span></span>](changehighlights.md) <br/> |<span data-ttu-id="cd723-116">Especifica o que mudou entre duas versões de uma mensagem de solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="cd723-116">Specifies what has changed between two versions of a meeting request message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd723-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cd723-117">Text value</span></span>

<span data-ttu-id="cd723-118">Um valor de texto **true** para o elemento **HasStartTimeChanged** indica que a hora de início de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="cd723-118">A text value of **true** for the **HasStartTimeChanged** element indicates that the start time for a meeting has changed.</span></span> <span data-ttu-id="cd723-119">Um valor **false** indica que a hora de início não foi alterada.</span><span class="sxs-lookup"><span data-stu-id="cd723-119">A value of **false** indicates that the start time has not changed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cd723-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="cd723-120">Remarks</span></span>

<span data-ttu-id="cd723-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cd723-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cd723-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd723-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd723-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cd723-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd723-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd723-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd723-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cd723-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cd723-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="cd723-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="cd723-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cd723-127">Validation File</span></span>  <br/> |<span data-ttu-id="cd723-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cd723-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd723-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cd723-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cd723-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="cd723-130">See also</span></span>



- [<span data-ttu-id="cd723-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cd723-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

