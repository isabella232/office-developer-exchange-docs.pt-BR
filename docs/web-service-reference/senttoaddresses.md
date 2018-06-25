---
title: SentToAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToAddresses
api_type:
- schema
ms.assetid: 086130d2-93b1-4de1-9553-10ec10322a0c
description: O elemento SentToAddresses indica os endereços de email que precisam foram enviadas em ordem para a condição ou exceção para aplicar a mensagens de entrada.
ms.openlocfilehash: c5a4770ff22e08713e5cf40b9a81191d50a2f437
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825358"
---
# <a name="senttoaddresses"></a><span data-ttu-id="624ed-103">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="624ed-103">SentToAddresses</span></span>

<span data-ttu-id="624ed-104">O elemento **SentToAddresses** indica os endereços de email que precisam foram enviadas em ordem para a condição ou exceção para aplicar a mensagens de entrada.</span><span class="sxs-lookup"><span data-stu-id="624ed-104">The **SentToAddresses** element indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToAddresses>
   <Address/>
</SentToAddresses>
```

 <span data-ttu-id="624ed-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="624ed-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="624ed-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="624ed-106">Attributes and elements</span></span>

<span data-ttu-id="624ed-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="624ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="624ed-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="624ed-108">Attributes</span></span>

<span data-ttu-id="624ed-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="624ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="624ed-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="624ed-110">Child elements</span></span>

|<span data-ttu-id="624ed-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="624ed-111">**Element**</span></span>|<span data-ttu-id="624ed-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="624ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="624ed-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="624ed-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="624ed-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="624ed-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="624ed-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="624ed-115">Parent elements</span></span>

|<span data-ttu-id="624ed-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="624ed-116">**Element**</span></span>|<span data-ttu-id="624ed-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="624ed-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="624ed-118">Condições</span><span class="sxs-lookup"><span data-stu-id="624ed-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="624ed-119">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="624ed-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="624ed-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="624ed-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="624ed-121">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="624ed-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="624ed-122">Text value</span><span class="sxs-lookup"><span data-stu-id="624ed-122">Text value</span></span>

<span data-ttu-id="624ed-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="624ed-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="624ed-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="624ed-124">Remarks</span></span>

<span data-ttu-id="624ed-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="624ed-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="624ed-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="624ed-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="624ed-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="624ed-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="624ed-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="624ed-128">Schema Name</span></span>  <br/> |<span data-ttu-id="624ed-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="624ed-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="624ed-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="624ed-130">Validation File</span></span>  <br/> |<span data-ttu-id="624ed-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="624ed-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="624ed-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="624ed-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="624ed-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="624ed-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="624ed-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="624ed-134">See also</span></span>



- [<span data-ttu-id="624ed-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="624ed-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

