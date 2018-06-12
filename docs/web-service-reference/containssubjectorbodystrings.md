---
title: ContainsSubjectOrBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectOrBodyStrings
api_type:
- schema
ms.assetid: 22aebf31-d9f4-4e03-bbff-c675409518d1
description: O elemento ContainsSubjectOrBodyStrings indica as cadeias de caracteres que devem aparecer no corpo ou o assunto de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: f577e7d26bb7d82ea1017f720e1d3a30892e2ef1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751485"
---
# <a name="containssubjectorbodystrings"></a><span data-ttu-id="6a821-103">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="6a821-103">ContainsSubjectOrBodyStrings</span></span>

<span data-ttu-id="6a821-104">O elemento **ContainsSubjectOrBodyStrings** indica as cadeias de caracteres que devem aparecer no corpo ou o assunto de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6a821-104">The **ContainsSubjectOrBodyStrings** element indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 <span data-ttu-id="6a821-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="6a821-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a821-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6a821-106">Attributes and elements</span></span>

<span data-ttu-id="6a821-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6a821-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a821-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6a821-108">Attributes</span></span>

<span data-ttu-id="6a821-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6a821-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a821-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6a821-110">Child elements</span></span>

|<span data-ttu-id="6a821-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a821-111">**Element**</span></span>|<span data-ttu-id="6a821-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a821-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a821-113">String</span><span class="sxs-lookup"><span data-stu-id="6a821-113">String</span></span>](string.md) <br/> |<span data-ttu-id="6a821-114">Representa uma cadeia de caracteres que deve aparecer no corpo ou o assunto de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6a821-114">Represents a string that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a821-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6a821-115">Parent elements</span></span>

|<span data-ttu-id="6a821-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a821-116">**Element**</span></span>|<span data-ttu-id="6a821-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a821-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a821-118">Condições</span><span class="sxs-lookup"><span data-stu-id="6a821-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6a821-119">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="6a821-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6a821-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="6a821-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6a821-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="6a821-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a821-122">Text value</span><span class="sxs-lookup"><span data-stu-id="6a821-122">Text value</span></span>

<span data-ttu-id="6a821-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6a821-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6a821-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="6a821-124">Remarks</span></span>

<span data-ttu-id="6a821-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a821-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a821-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6a821-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a821-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a821-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6a821-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6a821-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6a821-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6a821-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6a821-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6a821-130">Validation File</span></span>  <br/> |<span data-ttu-id="6a821-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6a821-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a821-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6a821-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a821-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6a821-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a821-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="6a821-134">See also</span></span>



- [<span data-ttu-id="6a821-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6a821-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

