---
title: MessageClassifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageClassifications
api_type:
- schema
ms.assetid: 041b3d48-8f43-47f3-869f-72b66bef372a
description: O elemento MessageClassifications representa as classificações de mensagem que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 63481aa8903c4e9637870130eb9154118471c3b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467967"
---
# <a name="messageclassifications"></a><span data-ttu-id="aefc7-103">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="aefc7-103">MessageClassifications</span></span>

<span data-ttu-id="aefc7-104">O elemento **MessageClassifications** representa as classificações de mensagem que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="aefc7-104">The **MessageClassifications** element represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<MessageClassifications>
    <String/>
</MessageClassifications>
```

 <span data-ttu-id="aefc7-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="aefc7-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aefc7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="aefc7-106">Attributes and elements</span></span>

<span data-ttu-id="aefc7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aefc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aefc7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aefc7-108">Attributes</span></span>

<span data-ttu-id="aefc7-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="aefc7-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aefc7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aefc7-110">Child elements</span></span>

|<span data-ttu-id="aefc7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aefc7-111">**Element**</span></span>|<span data-ttu-id="aefc7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aefc7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aefc7-113">String</span><span class="sxs-lookup"><span data-stu-id="aefc7-113">String</span></span>](string.md) <br/> |<span data-ttu-id="aefc7-114">Representa uma classificação de mensagem.</span><span class="sxs-lookup"><span data-stu-id="aefc7-114">Represents a message classification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aefc7-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aefc7-115">Parent elements</span></span>

|<span data-ttu-id="aefc7-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aefc7-116">**Element**</span></span>|<span data-ttu-id="aefc7-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aefc7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aefc7-118">Condições</span><span class="sxs-lookup"><span data-stu-id="aefc7-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="aefc7-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="aefc7-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="aefc7-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="aefc7-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="aefc7-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="aefc7-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aefc7-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="aefc7-122">Text value</span></span>

<span data-ttu-id="aefc7-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aefc7-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aefc7-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="aefc7-124">Remarks</span></span>

<span data-ttu-id="aefc7-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aefc7-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aefc7-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="aefc7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aefc7-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="aefc7-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aefc7-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aefc7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="aefc7-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="aefc7-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aefc7-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aefc7-130">Validation File</span></span>  <br/> |<span data-ttu-id="aefc7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aefc7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aefc7-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aefc7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="aefc7-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="aefc7-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aefc7-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="aefc7-134">See also</span></span>



- [<span data-ttu-id="aefc7-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aefc7-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

