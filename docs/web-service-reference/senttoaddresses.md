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
description: O elemento SentToAddresses indica os endereços de email para os quais as mensagens de entrada precisam ter sido enviadas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 9a901a93b666144092bf9cc8ebbf03222ac7bf6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457414"
---
# <a name="senttoaddresses"></a><span data-ttu-id="0de4e-103">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="0de4e-103">SentToAddresses</span></span>

<span data-ttu-id="0de4e-104">O elemento **SentToAddresses** indica os endereços de email para os quais as mensagens de entrada precisam ter sido enviadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="0de4e-104">The **SentToAddresses** element indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToAddresses>
   <Address/>
</SentToAddresses>
```

 <span data-ttu-id="0de4e-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="0de4e-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0de4e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0de4e-106">Attributes and elements</span></span>

<span data-ttu-id="0de4e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0de4e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0de4e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0de4e-108">Attributes</span></span>

<span data-ttu-id="0de4e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0de4e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0de4e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0de4e-110">Child elements</span></span>

|<span data-ttu-id="0de4e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0de4e-111">**Element**</span></span>|<span data-ttu-id="0de4e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0de4e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0de4e-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="0de4e-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="0de4e-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="0de4e-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0de4e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0de4e-115">Parent elements</span></span>

|<span data-ttu-id="0de4e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0de4e-116">**Element**</span></span>|<span data-ttu-id="0de4e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0de4e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0de4e-118">Condições</span><span class="sxs-lookup"><span data-stu-id="0de4e-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0de4e-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="0de4e-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0de4e-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="0de4e-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0de4e-121">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="0de4e-121">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0de4e-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0de4e-122">Text value</span></span>

<span data-ttu-id="0de4e-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0de4e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0de4e-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="0de4e-124">Remarks</span></span>

<span data-ttu-id="0de4e-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0de4e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0de4e-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0de4e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0de4e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0de4e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0de4e-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0de4e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0de4e-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0de4e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0de4e-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0de4e-130">Validation File</span></span>  <br/> |<span data-ttu-id="0de4e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0de4e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0de4e-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0de4e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0de4e-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0de4e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0de4e-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0de4e-134">See also</span></span>



- [<span data-ttu-id="0de4e-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0de4e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

