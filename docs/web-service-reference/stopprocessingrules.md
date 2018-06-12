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
description: O elemento StopProcessingRules indica se as regras subsequentes devem ser avaliadas.
ms.openlocfilehash: 48799975f8c928bf291fcdcdb83f2ff8768af8b9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825593"
---
# <a name="stopprocessingrules"></a><span data-ttu-id="c9fb4-103">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="c9fb4-103">StopProcessingRules</span></span>

<span data-ttu-id="c9fb4-104">O elemento **StopProcessingRules** indica se as regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-104">The **StopProcessingRules** element indicates whether subsequent rules are to be evaluated.</span></span> 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
```

 <span data-ttu-id="c9fb4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c9fb4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9fb4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c9fb4-106">Attributes and elements</span></span>

<span data-ttu-id="c9fb4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9fb4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9fb4-108">Attributes</span></span>

<span data-ttu-id="c9fb4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9fb4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9fb4-110">Child elements</span></span>

<span data-ttu-id="c9fb4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9fb4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9fb4-112">Parent elements</span></span>

|<span data-ttu-id="c9fb4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9fb4-113">**Element**</span></span>|<span data-ttu-id="c9fb4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9fb4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9fb4-115">Ações</span><span class="sxs-lookup"><span data-stu-id="c9fb4-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="c9fb4-116">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9fb4-117">Text value</span><span class="sxs-lookup"><span data-stu-id="c9fb4-117">Text value</span></span>

<span data-ttu-id="c9fb4-118">Um valor de texto de **true** indica que as regras subsequentes não devem ser processadas.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-118">A text value of **true** indicates that subsequent rules should not be processed.</span></span> <span data-ttu-id="c9fb4-119">Um valor **false** indica que as regras subsequentes devem continuar a ser avaliada.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-119">A value of **false** indicates that subsequent rules should continue to be evaluated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c9fb4-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="c9fb4-120">Remarks</span></span>

<span data-ttu-id="c9fb4-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9fb4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9fb4-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c9fb4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9fb4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9fb4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9fb4-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9fb4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c9fb4-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c9fb4-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c9fb4-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9fb4-126">Validation File</span></span>  <br/> |<span data-ttu-id="c9fb4-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c9fb4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9fb4-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c9fb4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9fb4-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c9fb4-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9fb4-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="c9fb4-130">See also</span></span>



- [<span data-ttu-id="c9fb4-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c9fb4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

