---
title: IsAutomaticForward
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticForward
api_type:
- schema
ms.assetid: 6876b849-a648-482e-8934-93eb5a0c465f
description: O elemento IsAutomaticForward indica se as mensagens de entrada devem ser encaminhamentos automáticos na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: c2d44d6dce30cbf55e0c7673aaf41b114a3e2cd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823989"
---
# <a name="isautomaticforward"></a><span data-ttu-id="a451b-103">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="a451b-103">IsAutomaticForward</span></span>

<span data-ttu-id="a451b-104">O elemento **IsAutomaticForward** indica se as mensagens de entrada devem ser encaminhamentos automáticos na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="a451b-104">The **IsAutomaticForward** element indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticForward/> true | false</IsAutomaticForward>
```

 <span data-ttu-id="a451b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a451b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a451b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a451b-106">Attributes and elements</span></span>

<span data-ttu-id="a451b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a451b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a451b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a451b-108">Attributes</span></span>

<span data-ttu-id="a451b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a451b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a451b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a451b-110">Child elements</span></span>

<span data-ttu-id="a451b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a451b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a451b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a451b-112">Parent elements</span></span>

|<span data-ttu-id="a451b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a451b-113">**Element**</span></span>|<span data-ttu-id="a451b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a451b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a451b-115">Condições</span><span class="sxs-lookup"><span data-stu-id="a451b-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="a451b-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="a451b-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="a451b-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="a451b-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="a451b-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="a451b-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a451b-119">Text value</span><span class="sxs-lookup"><span data-stu-id="a451b-119">Text value</span></span>

<span data-ttu-id="a451b-120">Um valor de texto de **true** indica que a mensagem deve ser um encaminhamento automático na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="a451b-120">A text value of **true** indicates that the message must be an automatic forward in order for the condition or exception to apply.</span></span> <span data-ttu-id="a451b-121">Um valor **false** indica que a mensagem não deve ser um encaminhamento automático na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="a451b-121">A value of **false** indicates that the message must not be an automatic forward in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a451b-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="a451b-122">Remarks</span></span>

<span data-ttu-id="a451b-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a451b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a451b-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a451b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a451b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a451b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a451b-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a451b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a451b-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a451b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a451b-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a451b-128">Validation File</span></span>  <br/> |<span data-ttu-id="a451b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a451b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a451b-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a451b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a451b-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a451b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a451b-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="a451b-132">See also</span></span>



- [<span data-ttu-id="a451b-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a451b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

