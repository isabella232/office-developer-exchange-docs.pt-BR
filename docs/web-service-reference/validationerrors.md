---
title: ValidationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ValidationErrors
api_type:
- schema
ms.assetid: 009526aa-22e7-4f5c-be88-079175aa9122
description: O elemento ValidationErrors representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.
ms.openlocfilehash: c95c8057ad2d16a314d33e3738553b495355fd76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838009"
---
# <a name="validationerrors"></a><span data-ttu-id="ed86f-103">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="ed86f-103">ValidationErrors</span></span>

<span data-ttu-id="ed86f-104">O elemento **ValidationErrors** representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="ed86f-104">The **ValidationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
```XML
<VaidationErrors>
   <Error/>
</ValidationErrors>
```

 <span data-ttu-id="ed86f-105">**ArrayOfRuleValidationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="ed86f-105">**ArrayOfRuleValidationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed86f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ed86f-106">Attributes and elements</span></span>

<span data-ttu-id="ed86f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ed86f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed86f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ed86f-108">Attributes</span></span>

<span data-ttu-id="ed86f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed86f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed86f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ed86f-110">Child elements</span></span>

|<span data-ttu-id="ed86f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed86f-111">**Element**</span></span>|<span data-ttu-id="ed86f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed86f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed86f-113">Erro</span><span class="sxs-lookup"><span data-stu-id="ed86f-113">Error</span></span>](error.md) <br/> |<span data-ttu-id="ed86f-114">Representa um erro de validação única em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action</span><span class="sxs-lookup"><span data-stu-id="ed86f-114">Represents a single validation error on a particular rule property value, predicate property value, or action property value</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed86f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ed86f-115">Parent elements</span></span>

|<span data-ttu-id="ed86f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed86f-116">**Element**</span></span>|<span data-ttu-id="ed86f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed86f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed86f-118">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="ed86f-118">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="ed86f-119">Representa um erro de operação de regra.</span><span class="sxs-lookup"><span data-stu-id="ed86f-119">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed86f-120">Text value</span><span class="sxs-lookup"><span data-stu-id="ed86f-120">Text value</span></span>

<span data-ttu-id="ed86f-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed86f-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed86f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed86f-122">Remarks</span></span>

<span data-ttu-id="ed86f-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed86f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed86f-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ed86f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed86f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed86f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed86f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ed86f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ed86f-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ed86f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ed86f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ed86f-128">Validation File</span></span>  <br/> |<span data-ttu-id="ed86f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ed86f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed86f-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ed86f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed86f-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ed86f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed86f-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="ed86f-132">See also</span></span>



- [<span data-ttu-id="ed86f-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ed86f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

