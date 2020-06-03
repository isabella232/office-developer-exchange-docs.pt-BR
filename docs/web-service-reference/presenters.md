---
title: Apresentadores
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: O elemento apresentadores especifica os apresentadores de uma reunião online.
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529907"
---
# <a name="presenters"></a><span data-ttu-id="b5dfe-103">Apresentadores</span><span class="sxs-lookup"><span data-stu-id="b5dfe-103">Presenters</span></span>

<span data-ttu-id="b5dfe-104">O elemento **apresentadores** especifica os apresentadores de uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="b5dfe-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="b5dfe-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5dfe-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b5dfe-106">Attributes and elements</span></span>

<span data-ttu-id="b5dfe-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5dfe-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b5dfe-108">Attributes</span></span>

<span data-ttu-id="b5dfe-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5dfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5dfe-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b5dfe-110">Child elements</span></span>

<span data-ttu-id="b5dfe-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5dfe-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b5dfe-112">Parent elements</span></span>

[<span data-ttu-id="b5dfe-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="b5dfe-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="b5dfe-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b5dfe-114">Text value</span></span>

<span data-ttu-id="b5dfe-115">O valor de texto do elemento **apresentadores** é o tipo de usuários que podem ser um apresentador para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="b5dfe-116">Os valores de texto para o elemento **apresentadores** são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="b5dfe-117">**Valores de texto do elemento apresentadores**</span><span class="sxs-lookup"><span data-stu-id="b5dfe-117">**Presenters element text values**</span></span>

|<span data-ttu-id="b5dfe-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b5dfe-118">**Value**</span></span>|<span data-ttu-id="b5dfe-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b5dfe-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b5dfe-120">Desabilitado</span><span class="sxs-lookup"><span data-stu-id="b5dfe-120">Disabled</span></span>  <br/> |<span data-ttu-id="b5dfe-121">Os apresentadores estão desabilitados.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="b5dfe-122">Interno</span><span class="sxs-lookup"><span data-stu-id="b5dfe-122">Internal</span></span>  <br/> |<span data-ttu-id="b5dfe-123">Somente os participantes internos podem ser apresentadores.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="b5dfe-124">Todos</span><span class="sxs-lookup"><span data-stu-id="b5dfe-124">Everyone</span></span>  <br/> |<span data-ttu-id="b5dfe-125">Qualquer participante pode ser um apresentador.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b5dfe-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="b5dfe-126">Remarks</span></span>

<span data-ttu-id="b5dfe-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b5dfe-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5dfe-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5dfe-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b5dfe-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5dfe-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="b5dfe-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5dfe-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b5dfe-131">Schema name</span></span>  <br/> |<span data-ttu-id="b5dfe-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b5dfe-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5dfe-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b5dfe-133">Validation file</span></span>  <br/> |<span data-ttu-id="b5dfe-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b5dfe-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5dfe-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b5dfe-135">Can be empty</span></span>  <br/> ||
   

