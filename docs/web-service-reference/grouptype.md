---
title: GroupType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c31552f-22b8-4bf0-8cac-046fd92ac0d4
description: O elemento GroupType Especifica a classe de grupo de um grupo (IM) de mensagens instantâneas.
ms.openlocfilehash: 330a1567ce85877ba73c6205898ea66b59585e16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823800"
---
# <a name="grouptype"></a><span data-ttu-id="3c130-103">GroupType</span><span class="sxs-lookup"><span data-stu-id="3c130-103">GroupType</span></span>

<span data-ttu-id="3c130-104">O elemento **GroupType** Especifica a classe de grupo de um grupo (IM) de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="3c130-104">The **GroupType** element specifies the group class of an instant messaging (IM) group.</span></span> 
  
```XML
<GroupType></GroupType>
```

 <span data-ttu-id="3c130-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="3c130-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c130-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3c130-106">Attributes and elements</span></span>

<span data-ttu-id="3c130-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3c130-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c130-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3c130-108">Attributes</span></span>

<span data-ttu-id="3c130-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c130-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c130-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3c130-110">Child elements</span></span>

<span data-ttu-id="3c130-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c130-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c130-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3c130-112">Parent elements</span></span>

|<span data-ttu-id="3c130-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3c130-113">**Element**</span></span>|<span data-ttu-id="3c130-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3c130-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c130-115">ImGroup</span><span class="sxs-lookup"><span data-stu-id="3c130-115">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="3c130-116">Representa um grupo de mensagens instantâneo.</span><span class="sxs-lookup"><span data-stu-id="3c130-116">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c130-117">Text value</span><span class="sxs-lookup"><span data-stu-id="3c130-117">Text value</span></span>

<span data-ttu-id="3c130-118">O valor de texto do elemento **GroupType** é um valor string que especifica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="3c130-118">The text value of the **GroupType** element is a string value that specifies type of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3c130-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3c130-119">Remarks</span></span>

<span data-ttu-id="3c130-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3c130-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3c130-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c130-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c130-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3c130-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c130-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c130-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c130-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3c130-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3c130-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="3c130-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="3c130-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3c130-126">Validation File</span></span>  <br/> |<span data-ttu-id="3c130-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c130-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c130-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3c130-128">Can Be Empty</span></span>  <br/> |<span data-ttu-id="3c130-129">False</span><span class="sxs-lookup"><span data-stu-id="3c130-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c130-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="3c130-130">See also</span></span>



- [<span data-ttu-id="3c130-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3c130-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

