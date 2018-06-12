---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: O elemento IsMembershipGroup Especifica um valor Boolean que indica se a entidade é um grupo de distribuição ou uma caixa de correio.
ms.openlocfilehash: 03ab0dc75d2c798b7f2afeef85aa45f0349be70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824050"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="2274f-103">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="2274f-103">IsMembershipGroup</span></span>

<span data-ttu-id="2274f-104">O elemento **IsMembershipGroup** Especifica um valor Boolean que indica se a entidade é um grupo de distribuição ou uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2274f-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="2274f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2274f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2274f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2274f-106">Attributes and elements</span></span>

<span data-ttu-id="2274f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2274f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2274f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2274f-108">Attributes</span></span>

<span data-ttu-id="2274f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2274f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2274f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2274f-110">Child elements</span></span>

<span data-ttu-id="2274f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2274f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2274f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2274f-112">Parent elements</span></span>

|<span data-ttu-id="2274f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2274f-113">**Element**</span></span>|<span data-ttu-id="2274f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2274f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2274f-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="2274f-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="2274f-116">Especifica uma caixa de correio retornados de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="2274f-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2274f-117">Text value</span><span class="sxs-lookup"><span data-stu-id="2274f-117">Text value</span></span>

<span data-ttu-id="2274f-118">Um valor de texto de **true** para o elemento **IsMembershipGroup** indica que a entidade é um grupo de distribuição ou uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2274f-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="2274f-119">Um valor false indica que a entidade não é um grupo de distribuição ou uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2274f-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2274f-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2274f-120">Remarks</span></span>

<span data-ttu-id="2274f-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2274f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2274f-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2274f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2274f-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2274f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2274f-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2274f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2274f-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2274f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2274f-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2274f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2274f-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2274f-127">Validation File</span></span>  <br/> |<span data-ttu-id="2274f-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2274f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2274f-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2274f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2274f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="2274f-130">See also</span></span>



- [<span data-ttu-id="2274f-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2274f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

