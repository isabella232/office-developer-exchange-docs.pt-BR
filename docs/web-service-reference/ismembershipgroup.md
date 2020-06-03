---
title: Membro ismembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: O elemento ismembership Group especifica um valor Boolean que indica se a entidade é um grupo de distribuição ou uma caixa de correio.
ms.openlocfilehash: ed79961c6d13ab226c0b489103ef3d2c4a08668d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459283"
---
# <a name="ismembershipgroup"></a><span data-ttu-id="19cab-103">Membro ismembership</span><span class="sxs-lookup"><span data-stu-id="19cab-103">IsMembershipGroup</span></span>

<span data-ttu-id="19cab-104">O elemento **ismembership** Group especifica um valor Boolean que indica se a entidade é um grupo de distribuição ou uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="19cab-104">The **IsMembershipGroup** element specifies a Boolean value that indicates whether the entity is a distribution group or a mailbox.</span></span> 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 <span data-ttu-id="19cab-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="19cab-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19cab-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="19cab-106">Attributes and elements</span></span>

<span data-ttu-id="19cab-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="19cab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19cab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="19cab-108">Attributes</span></span>

<span data-ttu-id="19cab-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19cab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19cab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="19cab-110">Child elements</span></span>

<span data-ttu-id="19cab-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19cab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19cab-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="19cab-112">Parent elements</span></span>

|<span data-ttu-id="19cab-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19cab-113">**Element**</span></span>|<span data-ttu-id="19cab-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19cab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19cab-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="19cab-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="19cab-116">Especifica uma caixa de correio retornada de uma solicitação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="19cab-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19cab-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="19cab-117">Text value</span></span>

<span data-ttu-id="19cab-118">Um valor de texto **true** para o elemento **ismembership** Group indica que a entidade é um grupo de distribuição ou uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="19cab-118">A text value of **true** for the **IsMembershipGroup** element indicates that the entity is a distribution group or a mailbox.</span></span> <span data-ttu-id="19cab-119">Um valor false indica que a entidade não é um grupo de distribuição ou uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="19cab-119">A value of false indicates that the entity is not a distribution group or a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="19cab-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="19cab-120">Remarks</span></span>

<span data-ttu-id="19cab-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="19cab-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="19cab-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="19cab-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19cab-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="19cab-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19cab-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="19cab-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19cab-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="19cab-125">Schema Name</span></span>  <br/> |<span data-ttu-id="19cab-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="19cab-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="19cab-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="19cab-127">Validation File</span></span>  <br/> |<span data-ttu-id="19cab-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="19cab-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="19cab-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="19cab-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="19cab-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="19cab-130">See also</span></span>



- [<span data-ttu-id="19cab-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="19cab-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

