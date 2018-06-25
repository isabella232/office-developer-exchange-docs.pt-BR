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
description: O elemento de transição representa uma transição de fuso horário.
ms.openlocfilehash: 5dcd2f0dae7c3df2dcf660d6fe1a41b216c67b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837799"
---
# <a name="transition"></a><span data-ttu-id="69501-103">Transição</span><span class="sxs-lookup"><span data-stu-id="69501-103">Transition</span></span>

<span data-ttu-id="69501-104">O elemento de **transição** representa uma transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="69501-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="69501-105">**TransitionType**</span><span class="sxs-lookup"><span data-stu-id="69501-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69501-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="69501-106">Attributes and elements</span></span>

<span data-ttu-id="69501-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="69501-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69501-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="69501-108">Attributes</span></span>

<span data-ttu-id="69501-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="69501-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69501-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="69501-110">Child elements</span></span>

|<span data-ttu-id="69501-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="69501-111">**Element**</span></span>|<span data-ttu-id="69501-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="69501-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69501-113">To</span><span class="sxs-lookup"><span data-stu-id="69501-113">To</span></span>](to.md) <br/> |<span data-ttu-id="69501-114">Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário.</span><span class="sxs-lookup"><span data-stu-id="69501-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69501-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="69501-115">Parent elements</span></span>

|<span data-ttu-id="69501-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="69501-116">**Element**</span></span>|<span data-ttu-id="69501-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="69501-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69501-118">Transições</span><span class="sxs-lookup"><span data-stu-id="69501-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="69501-119">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="69501-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69501-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="69501-120">Remarks</span></span>

<span data-ttu-id="69501-121">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="69501-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69501-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="69501-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69501-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="69501-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69501-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="69501-124">Schema Name</span></span>  <br/> |<span data-ttu-id="69501-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="69501-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="69501-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="69501-126">Validation File</span></span>  <br/> |<span data-ttu-id="69501-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="69501-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69501-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="69501-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="69501-129">False</span><span class="sxs-lookup"><span data-stu-id="69501-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69501-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="69501-130">See also</span></span>



- [<span data-ttu-id="69501-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="69501-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

