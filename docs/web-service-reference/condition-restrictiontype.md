---
title: Condição (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: O elemento de condição Especifica a condição que é usada para identificar o final de uma pesquisa para um FindItem ou uma operação FindConversation.
ms.openlocfilehash: 513fc21be52a90698f1c292d6d20d7cdaab07371
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751414"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="aa765-103">Condição (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="aa765-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="aa765-104">O elemento de **condição** Especifica a condição que é usada para identificar o final de uma pesquisa para um **FindItem** ou uma operação **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="aa765-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="aa765-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="aa765-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa765-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aa765-106">Attributes and elements</span></span>

<span data-ttu-id="aa765-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aa765-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa765-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aa765-108">Attributes</span></span>

<span data-ttu-id="aa765-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aa765-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa765-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aa765-110">Child elements</span></span>

|<span data-ttu-id="aa765-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aa765-111">**Element**</span></span>|<span data-ttu-id="aa765-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa765-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa765-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="aa765-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="aa765-114">Elemento abstrato que representa o elemento substituído dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="aa765-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa765-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aa765-115">Parent elements</span></span>

|<span data-ttu-id="aa765-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aa765-116">**Element**</span></span>|<span data-ttu-id="aa765-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa765-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa765-118">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="aa765-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="aa765-119">Identifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para uma operação de **FindConversation** ou um **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="aa765-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa765-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="aa765-120">Remarks</span></span>

<span data-ttu-id="aa765-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aa765-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aa765-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa765-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa765-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aa765-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa765-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa765-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aa765-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aa765-125">Schema Name</span></span>  <br/> |<span data-ttu-id="aa765-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="aa765-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="aa765-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aa765-127">Validation File</span></span>  <br/> |<span data-ttu-id="aa765-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aa765-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="aa765-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="aa765-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aa765-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="aa765-130">See also</span></span>



- [<span data-ttu-id="aa765-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aa765-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

