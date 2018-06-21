---
title: Prioridade
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: O elemento de prioridade indica a ordem na qual uma regra será executada.
ms.openlocfilehash: 49e9bda063d8766ff49c8a2e9574c986bcfdbeb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19824888"
---
# <a name="priority"></a><span data-ttu-id="d86b7-103">Prioridade</span><span class="sxs-lookup"><span data-stu-id="d86b7-103">Priority</span></span>

<span data-ttu-id="d86b7-104">O elemento de **prioridade** indica a ordem na qual uma regra será executada.</span><span class="sxs-lookup"><span data-stu-id="d86b7-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="d86b7-105">**int**</span><span class="sxs-lookup"><span data-stu-id="d86b7-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d86b7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d86b7-106">Attributes and elements</span></span>

<span data-ttu-id="d86b7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d86b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d86b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d86b7-108">Attributes</span></span>

<span data-ttu-id="d86b7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d86b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d86b7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d86b7-110">Child elements</span></span>

<span data-ttu-id="d86b7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d86b7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d86b7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d86b7-112">Parent elements</span></span>

|<span data-ttu-id="d86b7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d86b7-113">**Element**</span></span>|<span data-ttu-id="d86b7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d86b7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d86b7-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="d86b7-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="d86b7-116">Representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d86b7-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d86b7-117">Text value</span><span class="sxs-lookup"><span data-stu-id="d86b7-117">Text value</span></span>

<span data-ttu-id="d86b7-118">O valor de texto para o elemento de **prioridade** é um inteiro que indica a ordem de execução no qual uma regra deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="d86b7-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d86b7-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="d86b7-119">Remarks</span></span>

<span data-ttu-id="d86b7-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d86b7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d86b7-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d86b7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d86b7-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d86b7-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d86b7-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d86b7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d86b7-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d86b7-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d86b7-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d86b7-125">Validation File</span></span>  <br/> |<span data-ttu-id="d86b7-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d86b7-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d86b7-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d86b7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d86b7-128">False</span><span class="sxs-lookup"><span data-stu-id="d86b7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d86b7-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="d86b7-129">See also</span></span>



- [<span data-ttu-id="d86b7-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d86b7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

