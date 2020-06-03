---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: O elemento AggregationRestriction especifica um valor que é aplicado a um conjunto de propriedades persona resultante de uma solicitação FindPeople e filtra o resultado de acordo com a restrição especificada.
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463521"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="df512-103">AggregationRestriction</span><span class="sxs-lookup"><span data-stu-id="df512-103">AggregationRestriction</span></span>

<span data-ttu-id="df512-104">O elemento **AggregationRestriction** especifica um valor que é aplicado a um conjunto de propriedades persona resultante de uma solicitação FindPeople e filtra o resultado de acordo com a restrição especificada.</span><span class="sxs-lookup"><span data-stu-id="df512-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="df512-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="df512-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df512-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="df512-106">Attributes and elements</span></span>

<span data-ttu-id="df512-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="df512-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df512-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="df512-108">Attributes</span></span>

<span data-ttu-id="df512-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df512-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df512-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="df512-110">Child elements</span></span>

[<span data-ttu-id="df512-111">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="df512-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="df512-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="df512-112">Parent elements</span></span>

[<span data-ttu-id="df512-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="df512-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="df512-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="df512-114">Remarks</span></span>

<span data-ttu-id="df512-115">O elemento **AggregationRestriction** pode conter qualquer elemento filho que usa o grupo de substituição de **pesquisa** .</span><span class="sxs-lookup"><span data-stu-id="df512-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="df512-116">Os elementos que fazem parte do grupo de substituição da **pesquisa** são: [Contains](contains.md), [Exclude](excludes.md), [Exists](exists.md), [not](not.md), [or](or.md), [e](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)e [IsLessThanOrEqualTo](islessthanorequalto.md).</span><span class="sxs-lookup"><span data-stu-id="df512-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="df512-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="df512-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="df512-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="df512-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df512-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="df512-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df512-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="df512-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="df512-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="df512-121">Schema name</span></span>  <br/> |<span data-ttu-id="df512-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="df512-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="df512-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="df512-123">Validation file</span></span>  <br/> |<span data-ttu-id="df512-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="df512-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="df512-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="df512-125">Can be empty</span></span>  <br/> |<span data-ttu-id="df512-126">falso</span><span class="sxs-lookup"><span data-stu-id="df512-126">false</span></span>  <br/> |
   

