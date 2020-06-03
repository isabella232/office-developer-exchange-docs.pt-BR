---
title: StopProcessingRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StopProcessingRules
api_type:
- schema
ms.assetid: 5b89a2cb-ab26-444d-b3dd-2b3858872d63
description: O elemento StopProcessingRules indica se as regras subsequentes serão avaliadas.
ms.openlocfilehash: 9f068fd6290a39bbab6e3c1e29066c4fefefc64b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467897"
---
# <a name="stopprocessingrules"></a><span data-ttu-id="f161d-103">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="f161d-103">StopProcessingRules</span></span>

<span data-ttu-id="f161d-104">O elemento **StopProcessingRules** indica se as regras subsequentes serão avaliadas.</span><span class="sxs-lookup"><span data-stu-id="f161d-104">The **StopProcessingRules** element indicates whether subsequent rules are to be evaluated.</span></span> 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
```

 <span data-ttu-id="f161d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f161d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f161d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f161d-106">Attributes and elements</span></span>

<span data-ttu-id="f161d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f161d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f161d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f161d-108">Attributes</span></span>

<span data-ttu-id="f161d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f161d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f161d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f161d-110">Child elements</span></span>

<span data-ttu-id="f161d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f161d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f161d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f161d-112">Parent elements</span></span>

|<span data-ttu-id="f161d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f161d-113">**Element**</span></span>|<span data-ttu-id="f161d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f161d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f161d-115">Actions</span><span class="sxs-lookup"><span data-stu-id="f161d-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="f161d-116">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="f161d-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f161d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f161d-117">Text value</span></span>

<span data-ttu-id="f161d-118">Um valor **true** indica que as regras subsequentes não devem ser processadas.</span><span class="sxs-lookup"><span data-stu-id="f161d-118">A text value of **true** indicates that subsequent rules should not be processed.</span></span> <span data-ttu-id="f161d-119">Um valor **false** indica que as regras subsequentes devem continuar a ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="f161d-119">A value of **false** indicates that subsequent rules should continue to be evaluated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f161d-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="f161d-120">Remarks</span></span>

<span data-ttu-id="f161d-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f161d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f161d-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f161d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f161d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f161d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f161d-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f161d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f161d-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f161d-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f161d-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f161d-126">Validation File</span></span>  <br/> |<span data-ttu-id="f161d-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f161d-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f161d-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f161d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f161d-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f161d-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f161d-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="f161d-130">See also</span></span>



- [<span data-ttu-id="f161d-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f161d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

