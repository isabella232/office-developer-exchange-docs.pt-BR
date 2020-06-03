---
title: ContainsHeaderStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsHeaderStrings
api_type:
- schema
ms.assetid: 5f68427b-990a-4a27-bfb3-fce3115b02d7
description: O elemento ContainsHeaderStrings indica as cadeias de caracteres que devem aparecer nos cabeçalhos das mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 23e3d0e7cff9c78edbac10a6275514af93cab325
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458989"
---
# <a name="containsheaderstrings"></a><span data-ttu-id="e685d-103">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="e685d-103">ContainsHeaderStrings</span></span>

<span data-ttu-id="e685d-104">O elemento **ContainsHeaderStrings** indica as cadeias de caracteres que devem aparecer nos cabeçalhos das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="e685d-104">The **ContainsHeaderStrings** element indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsHeaderStrings>
    <String/>
</ContainsHeaderStrings>
```

 <span data-ttu-id="e685d-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e685d-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e685d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e685d-106">Attributes and elements</span></span>

<span data-ttu-id="e685d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e685d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e685d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e685d-108">Attributes</span></span>

<span data-ttu-id="e685d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e685d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e685d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e685d-110">Child elements</span></span>

|<span data-ttu-id="e685d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e685d-111">**Element**</span></span>|<span data-ttu-id="e685d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e685d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e685d-113">String</span><span class="sxs-lookup"><span data-stu-id="e685d-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e685d-114">Representa uma cadeia de caracteres que deve aparecer em cabeçalhos de mensagem para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="e685d-114">Represents a string that must appear in message headers in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e685d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e685d-115">Parent elements</span></span>

|<span data-ttu-id="e685d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e685d-116">**Element**</span></span>|<span data-ttu-id="e685d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e685d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e685d-118">Condições</span><span class="sxs-lookup"><span data-stu-id="e685d-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e685d-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="e685d-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e685d-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="e685d-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e685d-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="e685d-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e685d-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e685d-122">Text value</span></span>

<span data-ttu-id="e685d-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e685d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e685d-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="e685d-124">Remarks</span></span>

<span data-ttu-id="e685d-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e685d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e685d-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e685d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e685d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="e685d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e685d-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e685d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e685d-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e685d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e685d-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e685d-130">Validation File</span></span>  <br/> |<span data-ttu-id="e685d-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e685d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e685d-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e685d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e685d-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e685d-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e685d-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="e685d-134">See also</span></span>



- [<span data-ttu-id="e685d-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e685d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

