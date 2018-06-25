---
title: FromConnectedAccounts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromConnectedAccounts
api_type:
- schema
ms.assetid: d4d7ddd7-078d-4f1a-a26b-22dce0c49f3a
description: O elemento FromConnectedAccounts representa os nomes de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 426e81bbbe96fb5fb4b36506438dc4af4f560eef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752372"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="2b9b1-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="2b9b1-103">FromConnectedAccounts</span></span>

<span data-ttu-id="2b9b1-104">O elemento **FromConnectedAccounts** representa os nomes de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="2b9b1-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="2b9b1-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b9b1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2b9b1-106">Attributes and elements</span></span>

<span data-ttu-id="2b9b1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b9b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2b9b1-108">Attributes</span></span>

<span data-ttu-id="2b9b1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b9b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2b9b1-110">Child elements</span></span>

|<span data-ttu-id="2b9b1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b9b1-111">**Element**</span></span>|<span data-ttu-id="2b9b1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b9b1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b9b1-113">String</span><span class="sxs-lookup"><span data-stu-id="2b9b1-113">String</span></span>](string.md) <br/> |<span data-ttu-id="2b9b1-114">Representa um nome de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b9b1-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2b9b1-115">Parent elements</span></span>

|<span data-ttu-id="2b9b1-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b9b1-116">**Element**</span></span>|<span data-ttu-id="2b9b1-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b9b1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b9b1-118">Condições</span><span class="sxs-lookup"><span data-stu-id="2b9b1-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="2b9b1-119">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="2b9b1-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="2b9b1-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="2b9b1-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b9b1-122">Text value</span><span class="sxs-lookup"><span data-stu-id="2b9b1-122">Text value</span></span>

<span data-ttu-id="2b9b1-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b9b1-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="2b9b1-124">Remarks</span></span>

<span data-ttu-id="2b9b1-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b9b1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b9b1-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2b9b1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b9b1-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b9b1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2b9b1-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2b9b1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2b9b1-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2b9b1-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2b9b1-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2b9b1-130">Validation File</span></span>  <br/> |<span data-ttu-id="2b9b1-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2b9b1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2b9b1-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2b9b1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b9b1-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="2b9b1-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b9b1-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="2b9b1-134">See also</span></span>



- [<span data-ttu-id="2b9b1-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2b9b1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

