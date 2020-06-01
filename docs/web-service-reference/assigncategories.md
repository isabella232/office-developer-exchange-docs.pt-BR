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
description: O elemento AssignCategories representa as categorias que estão carimbadas nas mensagens de email.
ms.openlocfilehash: e2dad0e2ef46421ae92a0d2826d161e5e2af3b93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464739"
---
# <a name="assigncategories"></a><span data-ttu-id="a9b7d-103">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="a9b7d-103">AssignCategories</span></span>

<span data-ttu-id="a9b7d-104">O elemento **AssignCategories** representa as categorias que estão carimbadas nas mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="a9b7d-104">The **AssignCategories** element represents the categories that are stamped on e-mail messages.</span></span> 
  
- [<span data-ttu-id="a9b7d-105">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="a9b7d-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
- [<span data-ttu-id="a9b7d-106">Actions</span><span class="sxs-lookup"><span data-stu-id="a9b7d-106">Actions</span></span>](actions.md)
  
```XML
<AssignCategories>
   <String/>
</AssignCategories>
```

 <span data-ttu-id="a9b7d-107">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="a9b7d-107">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9b7d-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a9b7d-108">Attributes and elements</span></span>

<span data-ttu-id="a9b7d-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a9b7d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9b7d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a9b7d-110">Attributes</span></span>

<span data-ttu-id="a9b7d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9b7d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9b7d-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a9b7d-112">Child elements</span></span>

|<span data-ttu-id="a9b7d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a9b7d-113">**Element**</span></span>|<span data-ttu-id="a9b7d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9b7d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9b7d-115">String</span><span class="sxs-lookup"><span data-stu-id="a9b7d-115">String</span></span>](string.md) <br/> |<span data-ttu-id="a9b7d-116">Contém uma cadeia de caracteres que identifica uma única categoria.</span><span class="sxs-lookup"><span data-stu-id="a9b7d-116">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a9b7d-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a9b7d-117">Parent elements</span></span>

|<span data-ttu-id="a9b7d-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a9b7d-118">**Element**</span></span>|<span data-ttu-id="a9b7d-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9b7d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9b7d-120">Actions</span><span class="sxs-lookup"><span data-stu-id="a9b7d-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="a9b7d-121">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="a9b7d-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9b7d-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a9b7d-122">Text value</span></span>

<span data-ttu-id="a9b7d-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9b7d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a9b7d-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="a9b7d-124">Remarks</span></span>

<span data-ttu-id="a9b7d-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9b7d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9b7d-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a9b7d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9b7d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="a9b7d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a9b7d-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a9b7d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a9b7d-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a9b7d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a9b7d-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a9b7d-130">Validation File</span></span>  <br/> |<span data-ttu-id="a9b7d-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a9b7d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a9b7d-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a9b7d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9b7d-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a9b7d-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9b7d-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a9b7d-134">See also</span></span>

- [<span data-ttu-id="a9b7d-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a9b7d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

