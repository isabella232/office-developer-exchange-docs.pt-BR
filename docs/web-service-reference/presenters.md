---
title: Apresentadores
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: O elemento de apresentadores Especifica os apresentadores de uma reunião online.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824875"
---
# <a name="presenters"></a><span data-ttu-id="ae715-103">Apresentadores</span><span class="sxs-lookup"><span data-stu-id="ae715-103">Presenters</span></span>

<span data-ttu-id="ae715-104">O elemento de **apresentadores** Especifica os apresentadores de uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae715-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="ae715-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="ae715-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae715-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ae715-106">Attributes and elements</span></span>

<span data-ttu-id="ae715-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ae715-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae715-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ae715-108">Attributes</span></span>

<span data-ttu-id="ae715-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ae715-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae715-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ae715-110">Child elements</span></span>

<span data-ttu-id="ae715-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ae715-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae715-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ae715-112">Parent elements</span></span>

[<span data-ttu-id="ae715-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="ae715-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="ae715-114">Text value</span><span class="sxs-lookup"><span data-stu-id="ae715-114">Text value</span></span>

<span data-ttu-id="ae715-115">O valor de texto do elemento de **apresentadores** é o tipo de usuários que pode ser um apresentador de uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae715-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="ae715-116">Os valores de texto para o elemento de **apresentadores** são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ae715-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="ae715-117">**Valores de texto do elemento de apresentadores**</span><span class="sxs-lookup"><span data-stu-id="ae715-117">**Presenters element text values**</span></span>

|<span data-ttu-id="ae715-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ae715-118">**Value**</span></span>|<span data-ttu-id="ae715-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae715-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ae715-120">Desabilitado</span><span class="sxs-lookup"><span data-stu-id="ae715-120">Disabled</span></span>  <br/> |<span data-ttu-id="ae715-121">Os apresentadores estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="ae715-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="ae715-122">Interno</span><span class="sxs-lookup"><span data-stu-id="ae715-122">Internal</span></span>  <br/> |<span data-ttu-id="ae715-123">Somente os participantes internos podem ser apresentadores.</span><span class="sxs-lookup"><span data-stu-id="ae715-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="ae715-124">Todos</span><span class="sxs-lookup"><span data-stu-id="ae715-124">Everyone</span></span>  <br/> |<span data-ttu-id="ae715-125">Qualquer participante pode ser um apresentador.</span><span class="sxs-lookup"><span data-stu-id="ae715-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ae715-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="ae715-126">Remarks</span></span>

<span data-ttu-id="ae715-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ae715-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ae715-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae715-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae715-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ae715-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae715-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae715-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae715-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ae715-131">Schema name</span></span>  <br/> |<span data-ttu-id="ae715-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ae715-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae715-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ae715-133">Validation file</span></span>  <br/> |<span data-ttu-id="ae715-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae715-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae715-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ae715-135">Can be empty</span></span>  <br/> ||
   

