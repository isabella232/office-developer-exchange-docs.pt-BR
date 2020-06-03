---
title: Condição (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: O elemento Condition especifica a condição usada para identificar o final de uma pesquisa para um FindItem ou uma operação FindConversation.
ms.openlocfilehash: 00c5b5e615ed9b253c79dae9dc2b89c797853089
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463934"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="6a2c5-103">Condição (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="6a2c5-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="6a2c5-104">O elemento **Condition** especifica a condição usada para identificar o final de uma pesquisa para um **FindItem** ou uma operação **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="6a2c5-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="6a2c5-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="6a2c5-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a2c5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6a2c5-106">Attributes and elements</span></span>

<span data-ttu-id="6a2c5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6a2c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a2c5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6a2c5-108">Attributes</span></span>

<span data-ttu-id="6a2c5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a2c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a2c5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6a2c5-110">Child elements</span></span>

|<span data-ttu-id="6a2c5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a2c5-111">**Element**</span></span>|<span data-ttu-id="6a2c5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a2c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a2c5-113">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="6a2c5-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="6a2c5-114">Elemento abstract que representa o elemento substituído dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="6a2c5-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a2c5-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6a2c5-115">Parent elements</span></span>

|<span data-ttu-id="6a2c5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a2c5-116">**Element**</span></span>|<span data-ttu-id="6a2c5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a2c5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a2c5-118">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="6a2c5-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="6a2c5-119">Identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, o número máximo de entradas a serem retornadas e as direções de pesquisa para um **FindItem** ou uma operação **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="6a2c5-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a2c5-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="6a2c5-120">Remarks</span></span>

<span data-ttu-id="6a2c5-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6a2c5-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6a2c5-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a2c5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a2c5-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6a2c5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a2c5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a2c5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a2c5-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6a2c5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6a2c5-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="6a2c5-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6a2c5-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6a2c5-127">Validation File</span></span>  <br/> |<span data-ttu-id="6a2c5-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6a2c5-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a2c5-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6a2c5-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6a2c5-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="6a2c5-130">See also</span></span>



- [<span data-ttu-id="6a2c5-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6a2c5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

