---
title: Constante
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: O elemento constante identifica um valor de constante em uma restrição.
ms.openlocfilehash: 73912bc1981c5d54040f7c4a563ad805916fe721
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751431"
---
# <a name="constant"></a><span data-ttu-id="cd539-103">Constante</span><span class="sxs-lookup"><span data-stu-id="cd539-103">Constant</span></span>

<span data-ttu-id="cd539-104">O elemento **constante** identifica um valor de constante em uma restrição.</span><span class="sxs-lookup"><span data-stu-id="cd539-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="cd539-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="cd539-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd539-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cd539-106">Attributes and elements</span></span>

<span data-ttu-id="cd539-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cd539-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd539-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cd539-108">Attributes</span></span>

|<span data-ttu-id="cd539-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="cd539-109">**Attribute**</span></span>|<span data-ttu-id="cd539-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd539-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cd539-111">**Valor**</span><span class="sxs-lookup"><span data-stu-id="cd539-111">**Value**</span></span> <br/> |<span data-ttu-id="cd539-112">Especifica o valor para comparar os a restrição.</span><span class="sxs-lookup"><span data-stu-id="cd539-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cd539-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cd539-113">Child elements</span></span>

<span data-ttu-id="cd539-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd539-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd539-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cd539-115">Parent elements</span></span>

|<span data-ttu-id="cd539-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd539-116">**Element**</span></span>|<span data-ttu-id="cd539-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd539-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd539-118">Contém</span><span class="sxs-lookup"><span data-stu-id="cd539-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="cd539-119">Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.</span><span class="sxs-lookup"><span data-stu-id="cd539-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="cd539-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="cd539-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="cd539-121">Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="cd539-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd539-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="cd539-122">Remarks</span></span>

<span data-ttu-id="cd539-123">O valor de cadeia de caracteres no atributo de **valor** deve ser conversível para o tipo que você está tentando comparar com.</span><span class="sxs-lookup"><span data-stu-id="cd539-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="cd539-124">Por exemplo, se você está comparando uma propriedade de data/hora em relação a um valor de constante, o valor de cadeia de caracteres deve representam uma data/hora.</span><span class="sxs-lookup"><span data-stu-id="cd539-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="cd539-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cd539-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd539-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cd539-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd539-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd539-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd539-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cd539-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cd539-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cd539-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd539-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cd539-130">Validation File</span></span>  <br/> |<span data-ttu-id="cd539-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd539-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd539-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cd539-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd539-133">False</span><span class="sxs-lookup"><span data-stu-id="cd539-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd539-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="cd539-134">See also</span></span>



- [<span data-ttu-id="cd539-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cd539-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

