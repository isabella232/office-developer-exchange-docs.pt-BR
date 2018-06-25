---
title: ContainsSubjectStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectStrings
api_type:
- schema
ms.assetid: c6ec1d8d-8dd8-4c9a-a3e1-50e24958eb0d
description: O elemento ContainsSubjectStrings indica as cadeias de caracteres que devem aparecer no assunto do mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: a266855effaeb34aa232305db970f97c309a2e4c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751496"
---
# <a name="containssubjectstrings"></a><span data-ttu-id="e1cae-103">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="e1cae-103">ContainsSubjectStrings</span></span>

<span data-ttu-id="e1cae-104">O elemento **ContainsSubjectStrings** indica as cadeias de caracteres que devem aparecer no assunto do mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e1cae-104">The **ContainsSubjectStrings** element indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectStrings>
    <String/>
</ContainsSubjectStrings>
```

 <span data-ttu-id="e1cae-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e1cae-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1cae-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e1cae-106">Attributes and elements</span></span>

<span data-ttu-id="e1cae-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1cae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1cae-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1cae-108">Attributes</span></span>

<span data-ttu-id="e1cae-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1cae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1cae-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1cae-110">Child elements</span></span>

|<span data-ttu-id="e1cae-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1cae-111">**Element**</span></span>|<span data-ttu-id="e1cae-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1cae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1cae-113">String</span><span class="sxs-lookup"><span data-stu-id="e1cae-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e1cae-114">Representa uma cadeia de caracteres que deve aparecer no assunto do mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e1cae-114">Represents a string that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1cae-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1cae-115">Parent elements</span></span>

|<span data-ttu-id="e1cae-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1cae-116">**Element**</span></span>|<span data-ttu-id="e1cae-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1cae-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1cae-118">Condições</span><span class="sxs-lookup"><span data-stu-id="e1cae-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e1cae-119">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="e1cae-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e1cae-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="e1cae-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e1cae-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="e1cae-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1cae-122">Text value</span><span class="sxs-lookup"><span data-stu-id="e1cae-122">Text value</span></span>

<span data-ttu-id="e1cae-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1cae-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1cae-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1cae-124">Remarks</span></span>

<span data-ttu-id="e1cae-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1cae-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1cae-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e1cae-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1cae-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1cae-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1cae-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1cae-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e1cae-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e1cae-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e1cae-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1cae-130">Validation File</span></span>  <br/> |<span data-ttu-id="e1cae-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e1cae-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1cae-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e1cae-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1cae-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e1cae-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1cae-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="e1cae-134">See also</span></span>



- [<span data-ttu-id="e1cae-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e1cae-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

