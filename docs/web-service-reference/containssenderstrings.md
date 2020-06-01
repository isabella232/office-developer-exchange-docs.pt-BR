---
title: ContainsSenderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSenderStrings
api_type:
- schema
ms.assetid: 3e16163f-cffe-4c4e-9a2a-00245d25ba96
description: O elemento ContainsSenderStrings indica as cadeias de caracteres que devem aparecer na propriedade from de mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: e7b78f1311d288db7969a0024bde84433e18d37f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458975"
---
# <a name="containssenderstrings"></a><span data-ttu-id="b9317-103">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b9317-103">ContainsSenderStrings</span></span>

<span data-ttu-id="b9317-104">O elemento **ContainsSenderStrings** indica as cadeias de caracteres que devem aparecer na propriedade **from** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="b9317-104">The **ContainsSenderStrings** element indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSenderStrings>
    <String/>
</ContainsSenderStrings>
```

 <span data-ttu-id="b9317-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b9317-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9317-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b9317-106">Attributes and elements</span></span>

<span data-ttu-id="b9317-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b9317-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9317-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b9317-108">Attributes</span></span>

<span data-ttu-id="b9317-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9317-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9317-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b9317-110">Child elements</span></span>

|<span data-ttu-id="b9317-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9317-111">**Element**</span></span>|<span data-ttu-id="b9317-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9317-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9317-113">String</span><span class="sxs-lookup"><span data-stu-id="b9317-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b9317-114">Representa uma cadeia de caracteres que deve aparecer na propriedade **from** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="b9317-114">Represents a string that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9317-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b9317-115">Parent elements</span></span>

|<span data-ttu-id="b9317-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9317-116">**Element**</span></span>|<span data-ttu-id="b9317-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9317-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9317-118">Condições</span><span class="sxs-lookup"><span data-stu-id="b9317-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b9317-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="b9317-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b9317-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="b9317-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b9317-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="b9317-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9317-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b9317-122">Text value</span></span>

<span data-ttu-id="b9317-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9317-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9317-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="b9317-124">Remarks</span></span>

<span data-ttu-id="b9317-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9317-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9317-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b9317-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9317-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9317-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9317-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b9317-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b9317-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b9317-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b9317-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b9317-130">Validation File</span></span>  <br/> |<span data-ttu-id="b9317-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9317-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9317-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b9317-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9317-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b9317-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9317-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b9317-134">See also</span></span>



- [<span data-ttu-id="b9317-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b9317-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

