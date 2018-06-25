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
description: O elemento FromAddresses indica os endereços de email do qual as mensagens de entrada devem ser enviadas na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 40ecb1f3e16ad961b8e4c38d5aa9d15f4f74469a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752374"
---
# <a name="fromaddresses"></a><span data-ttu-id="8a8ab-103">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="8a8ab-103">FromAddresses</span></span>

<span data-ttu-id="8a8ab-104">O elemento **FromAddresses** indica os endereços de email do qual as mensagens de entrada devem ser enviadas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-104">The **FromAddresses** element indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span> 
  
```XML
<FromAddresses>
   <Address/>
</FromAddresses>
```

 <span data-ttu-id="8a8ab-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="8a8ab-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a8ab-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8a8ab-106">Attributes and elements</span></span>

<span data-ttu-id="8a8ab-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a8ab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8a8ab-108">Attributes</span></span>

<span data-ttu-id="8a8ab-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a8ab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8a8ab-110">Child elements</span></span>

|<span data-ttu-id="8a8ab-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8a8ab-111">**Element**</span></span>|<span data-ttu-id="8a8ab-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a8ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a8ab-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="8a8ab-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="8a8ab-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a8ab-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8a8ab-115">Parent elements</span></span>

|<span data-ttu-id="8a8ab-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8a8ab-116">**Element**</span></span>|<span data-ttu-id="8a8ab-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a8ab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a8ab-118">Condições</span><span class="sxs-lookup"><span data-stu-id="8a8ab-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="8a8ab-119">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="8a8ab-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="8a8ab-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="8a8ab-121">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8a8ab-122">Text value</span><span class="sxs-lookup"><span data-stu-id="8a8ab-122">Text value</span></span>

<span data-ttu-id="8a8ab-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a8ab-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="8a8ab-124">Remarks</span></span>

<span data-ttu-id="8a8ab-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8ab-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a8ab-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8a8ab-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a8ab-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a8ab-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a8ab-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8a8ab-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8a8ab-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8a8ab-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8a8ab-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8a8ab-130">Validation File</span></span>  <br/> |<span data-ttu-id="8a8ab-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8a8ab-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a8ab-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8a8ab-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a8ab-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="8a8ab-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a8ab-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="8a8ab-134">See also</span></span>



- [<span data-ttu-id="8a8ab-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8ab-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

