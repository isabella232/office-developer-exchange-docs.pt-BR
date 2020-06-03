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
description: O elemento FromConnectedAccounts representa os nomes de conta de email dos quais as mensagens de entrada precisam ter sido agregadas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 159ae064827c2f9c2b470580ad5457264e8dae93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464046"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="7d273-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="7d273-103">FromConnectedAccounts</span></span>

<span data-ttu-id="7d273-104">O elemento **FromConnectedAccounts** representa os nomes de conta de email dos quais as mensagens de entrada precisam ter sido agregadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="7d273-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="7d273-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="7d273-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d273-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7d273-106">Attributes and elements</span></span>

<span data-ttu-id="7d273-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7d273-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d273-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7d273-108">Attributes</span></span>

<span data-ttu-id="7d273-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d273-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d273-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7d273-110">Child elements</span></span>

|<span data-ttu-id="7d273-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7d273-111">**Element**</span></span>|<span data-ttu-id="7d273-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7d273-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d273-113">String</span><span class="sxs-lookup"><span data-stu-id="7d273-113">String</span></span>](string.md) <br/> |<span data-ttu-id="7d273-114">Representa um nome de conta de email a partir do qual as mensagens de entrada precisam ser agregadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="7d273-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d273-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7d273-115">Parent elements</span></span>

|<span data-ttu-id="7d273-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7d273-116">**Element**</span></span>|<span data-ttu-id="7d273-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7d273-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d273-118">Condições</span><span class="sxs-lookup"><span data-stu-id="7d273-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="7d273-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="7d273-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="7d273-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="7d273-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="7d273-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="7d273-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d273-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7d273-122">Text value</span></span>

<span data-ttu-id="7d273-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7d273-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d273-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="7d273-124">Remarks</span></span>

<span data-ttu-id="7d273-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d273-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d273-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7d273-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d273-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7d273-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d273-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7d273-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7d273-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7d273-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d273-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7d273-130">Validation File</span></span>  <br/> |<span data-ttu-id="7d273-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7d273-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d273-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7d273-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d273-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="7d273-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d273-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="7d273-134">See also</span></span>



- [<span data-ttu-id="7d273-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7d273-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

