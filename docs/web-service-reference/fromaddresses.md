---
title: FromAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromAddresses
api_type:
- schema
ms.assetid: b219f315-c20a-4633-af3e-94bd3e4526b6
description: O elemento FromAddresses indica os endereços de email dos quais as mensagens de entrada devem ser enviadas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 4fbb44d02f5010c4395cf691cb6160da4dbb6930
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459536"
---
# <a name="fromaddresses"></a><span data-ttu-id="be85d-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="be85d-103">FromAddresses</span></span>

<span data-ttu-id="be85d-104">O elemento **FromAddresses** indica os endereços de email dos quais as mensagens de entrada devem ser enviadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="be85d-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="be85d-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="be85d-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be85d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="be85d-106">Attributes and elements</span></span>

<span data-ttu-id="be85d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="be85d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be85d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="be85d-108">Attributes</span></span>

<span data-ttu-id="be85d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be85d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be85d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="be85d-110">Child elements</span></span>

|<span data-ttu-id="be85d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="be85d-111">**Element**</span></span>|<span data-ttu-id="be85d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be85d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be85d-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="be85d-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="be85d-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="be85d-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be85d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="be85d-115">Parent elements</span></span>

|<span data-ttu-id="be85d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="be85d-116">**Element**</span></span>|<span data-ttu-id="be85d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be85d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be85d-118">Condições</span><span class="sxs-lookup"><span data-stu-id="be85d-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="be85d-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="be85d-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="be85d-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="be85d-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="be85d-121">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="be85d-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be85d-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="be85d-122">Text value</span></span>

<span data-ttu-id="be85d-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be85d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be85d-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="be85d-124">Remarks</span></span>

<span data-ttu-id="be85d-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be85d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be85d-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="be85d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be85d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="be85d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="be85d-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="be85d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="be85d-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="be85d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="be85d-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="be85d-130">Validation File</span></span>  <br/> |<span data-ttu-id="be85d-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="be85d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="be85d-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="be85d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="be85d-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="be85d-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be85d-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="be85d-134">See also</span></span>



- [<span data-ttu-id="be85d-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be85d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

