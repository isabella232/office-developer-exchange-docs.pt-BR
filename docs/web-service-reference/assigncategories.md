---
title: AssignCategories
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssignCategories
api_type:
- schema
ms.assetid: f5c73fed-7b00-446d-8296-71a0c86e7fc6
description: O elemento AssignCategories representa as categorias que estão marcadas em mensagens de email.
ms.openlocfilehash: 96c77306d649677c1be745e8cadc2886e4a84c8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751209"
---
# <a name="assigncategories"></a><span data-ttu-id="9d3fe-103">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="9d3fe-103">AssignCategories</span></span>

<span data-ttu-id="9d3fe-104">O elemento **AssignCategories** representa as categorias que estão marcadas em mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-104">The **AssignCategories** element represents the categories that are stamped on e-mail messages.</span></span> 
  
- [<span data-ttu-id="9d3fe-105">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="9d3fe-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
- [<span data-ttu-id="9d3fe-106">Ações</span><span class="sxs-lookup"><span data-stu-id="9d3fe-106">Actions</span></span>](actions.md)
  
```XML
<AssignCategories>
   <String/>
</AssignCategories>
```

 <span data-ttu-id="9d3fe-107">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="9d3fe-107">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d3fe-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9d3fe-108">Attributes and elements</span></span>

<span data-ttu-id="9d3fe-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d3fe-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d3fe-110">Attributes</span></span>

<span data-ttu-id="9d3fe-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d3fe-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d3fe-112">Child elements</span></span>

|<span data-ttu-id="9d3fe-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d3fe-113">**Element**</span></span>|<span data-ttu-id="9d3fe-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d3fe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d3fe-115">String</span><span class="sxs-lookup"><span data-stu-id="9d3fe-115">String</span></span>](string.md) <br/> |<span data-ttu-id="9d3fe-116">Contém uma cadeia de caracteres que identifica uma única categoria.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-116">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d3fe-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d3fe-117">Parent elements</span></span>

|<span data-ttu-id="9d3fe-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d3fe-118">**Element**</span></span>|<span data-ttu-id="9d3fe-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d3fe-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d3fe-120">Ações</span><span class="sxs-lookup"><span data-stu-id="9d3fe-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="9d3fe-121">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d3fe-122">Text value</span><span class="sxs-lookup"><span data-stu-id="9d3fe-122">Text value</span></span>

<span data-ttu-id="9d3fe-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d3fe-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d3fe-124">Remarks</span></span>

<span data-ttu-id="9d3fe-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d3fe-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d3fe-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9d3fe-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d3fe-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d3fe-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d3fe-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d3fe-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9d3fe-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9d3fe-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d3fe-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d3fe-130">Validation File</span></span>  <br/> |<span data-ttu-id="9d3fe-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d3fe-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d3fe-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d3fe-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d3fe-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9d3fe-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d3fe-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="9d3fe-134">See also</span></span>

- [<span data-ttu-id="9d3fe-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d3fe-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

