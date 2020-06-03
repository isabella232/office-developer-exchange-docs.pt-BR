---
title: Transição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transition
api_type:
- schema
ms.assetid: 23ce171a-a9c9-47ed-a366-822777048eea
description: O elemento Transition representa uma transição de fuso horário.
ms.openlocfilehash: 05495eb4a493feedc88532cc4bc8b949493481f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467491"
---
# <a name="transition"></a><span data-ttu-id="8e191-103">Transição</span><span class="sxs-lookup"><span data-stu-id="8e191-103">Transition</span></span>

<span data-ttu-id="8e191-104">O elemento **Transition** representa uma transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8e191-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="8e191-105">**Transitiontype**</span><span class="sxs-lookup"><span data-stu-id="8e191-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e191-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8e191-106">Attributes and elements</span></span>

<span data-ttu-id="8e191-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8e191-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e191-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8e191-108">Attributes</span></span>

<span data-ttu-id="8e191-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e191-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e191-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8e191-110">Child elements</span></span>

|<span data-ttu-id="8e191-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8e191-111">**Element**</span></span>|<span data-ttu-id="8e191-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8e191-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e191-113">To</span><span class="sxs-lookup"><span data-stu-id="8e191-113">To</span></span>](to.md) <br/> |<span data-ttu-id="8e191-114">Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8e191-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8e191-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8e191-115">Parent elements</span></span>

|<span data-ttu-id="8e191-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8e191-116">**Element**</span></span>|<span data-ttu-id="8e191-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8e191-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e191-118">Transições</span><span class="sxs-lookup"><span data-stu-id="8e191-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="8e191-119">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8e191-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e191-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8e191-120">Remarks</span></span>

<span data-ttu-id="8e191-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8e191-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e191-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8e191-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e191-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e191-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e191-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8e191-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8e191-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8e191-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e191-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8e191-126">Validation File</span></span>  <br/> |<span data-ttu-id="8e191-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8e191-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e191-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8e191-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e191-129">False</span><span class="sxs-lookup"><span data-stu-id="8e191-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e191-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="8e191-130">See also</span></span>



- [<span data-ttu-id="8e191-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8e191-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

