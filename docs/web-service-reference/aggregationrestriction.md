---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: O elemento AggregationRestriction Especifica um valor que é aplicado a um conjunto de propriedades de pessoa resultante de uma solicitação de FindPeople e filtra o resultado de acordo com a restrição especificada.
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751077"
---
# <a name="aggregationrestriction"></a><span data-ttu-id="c2c89-103">AggregationRestriction</span><span class="sxs-lookup"><span data-stu-id="c2c89-103">AggregationRestriction</span></span>

<span data-ttu-id="c2c89-104">O elemento **AggregationRestriction** Especifica um valor que é aplicado a um conjunto de propriedades de pessoa resultante de uma solicitação de FindPeople e filtra o resultado de acordo com a restrição especificada.</span><span class="sxs-lookup"><span data-stu-id="c2c89-104">The **AggregationRestriction** element specifies a value that is applied to a set of Persona properties resulting from a FindPeople request and filters the result according to the specified restriction.</span></span> 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 <span data-ttu-id="c2c89-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="c2c89-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2c89-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c2c89-106">Attributes and elements</span></span>

<span data-ttu-id="c2c89-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2c89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2c89-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2c89-108">Attributes</span></span>

<span data-ttu-id="c2c89-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2c89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2c89-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2c89-110">Child elements</span></span>

[<span data-ttu-id="c2c89-111">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="c2c89-111">SearchExpression</span></span>](searchexpression.md)
  
### <a name="parent-elements"></a><span data-ttu-id="c2c89-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2c89-112">Parent elements</span></span>

[<span data-ttu-id="c2c89-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="c2c89-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="c2c89-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c2c89-114">Remarks</span></span>

<span data-ttu-id="c2c89-115">O elemento **AggregationRestriction** pode conter qualquer elemento filho que usa o grupo de substituição de **SearchExpression** .</span><span class="sxs-lookup"><span data-stu-id="c2c89-115">The **AggregationRestriction** element can contain any child element that uses the **SearchExpression** substitution group.</span></span> <span data-ttu-id="c2c89-116">Os elementos que fazem parte do grupo de substituição **SearchExpression** são: [contém](contains.md), [exclusões](excludes.md), [Exists](exists.md), [não](not.md), [ou](or.md) [e](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan ](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md)e [IsLessThanOrEqualTo](islessthanorequalto.md).</span><span class="sxs-lookup"><span data-stu-id="c2c89-116">The elements that are a part of the **SearchExpression** substitution group are: [Contains](contains.md), [Excludes](excludes.md), [Exists](exists.md), [Not](not.md), [Or](or.md), [And](and.md), [IsEqualTo](isequalto.md), [IsNotEqualTo](isnotequalto.md), [IsGreaterThan](isgreaterthan.md), [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md), [IsLessThan](islessthan.md), and [IsLessThanOrEqualTo](islessthanorequalto.md).</span></span>
  
<span data-ttu-id="c2c89-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c2c89-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c2c89-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2c89-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2c89-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c2c89-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2c89-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2c89-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2c89-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2c89-121">Schema name</span></span>  <br/> |<span data-ttu-id="c2c89-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c2c89-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2c89-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2c89-123">Validation file</span></span>  <br/> |<span data-ttu-id="c2c89-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2c89-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2c89-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c2c89-125">Can be empty</span></span>  <br/> |<span data-ttu-id="c2c89-126">false</span><span class="sxs-lookup"><span data-stu-id="c2c89-126">false</span></span>  <br/> |
   

