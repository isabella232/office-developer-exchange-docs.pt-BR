---
title: ContainsBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsBodyStrings
api_type:
- schema
ms.assetid: 70639472-64bb-456a-8b40-dce727542443
description: O elemento ContainsBodyStrings indica as cadeias de caracteres que devem aparecer no corpo das mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 008261ab94b1bed33cc72cacf7abe7aa58927d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463801"
---
# <a name="containsbodystrings"></a><span data-ttu-id="0449b-103">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="0449b-103">ContainsBodyStrings</span></span>

<span data-ttu-id="0449b-104">O elemento **ContainsBodyStrings** indica as cadeias de caracteres que devem aparecer no corpo das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="0449b-104">The **ContainsBodyStrings** element indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsBodyStrings>
    <String/>
</ContainsBodyStrings>
```

 <span data-ttu-id="0449b-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="0449b-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0449b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0449b-106">Attributes and elements</span></span>

<span data-ttu-id="0449b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0449b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0449b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0449b-108">Attributes</span></span>

<span data-ttu-id="0449b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0449b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0449b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0449b-110">Child elements</span></span>

|<span data-ttu-id="0449b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0449b-111">**Element**</span></span>|<span data-ttu-id="0449b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0449b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0449b-113">String</span><span class="sxs-lookup"><span data-stu-id="0449b-113">String</span></span>](string.md) <br/> |<span data-ttu-id="0449b-114">Representa uma cadeia de caracteres que deve aparecer no corpo de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="0449b-114">Represents a string that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0449b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0449b-115">Parent elements</span></span>

|<span data-ttu-id="0449b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0449b-116">**Element**</span></span>|<span data-ttu-id="0449b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0449b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0449b-118">Condições</span><span class="sxs-lookup"><span data-stu-id="0449b-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0449b-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="0449b-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0449b-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="0449b-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0449b-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="0449b-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0449b-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0449b-122">Text value</span></span>

<span data-ttu-id="0449b-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0449b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0449b-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="0449b-124">Remarks</span></span>

<span data-ttu-id="0449b-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0449b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0449b-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0449b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0449b-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0449b-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0449b-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0449b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0449b-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0449b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0449b-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0449b-130">Validation File</span></span>  <br/> |<span data-ttu-id="0449b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0449b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0449b-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0449b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0449b-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0449b-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0449b-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0449b-134">See also</span></span>



- [<span data-ttu-id="0449b-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0449b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

