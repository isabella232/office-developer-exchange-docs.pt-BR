---
title: Iscaixa postal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsVoicemail
api_type:
- schema
ms.assetid: 96d81d6e-4b75-43ad-b151-2dd4fd57db94
description: O elemento iscaixa postal indica se as mensagens de entrada devem ser mensagens de caixa postal para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 8c60513a54cbf2398fde4b71ab1fbcf8a5efb608
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458135"
---
# <a name="isvoicemail"></a><span data-ttu-id="77269-103">Iscaixa postal</span><span class="sxs-lookup"><span data-stu-id="77269-103">IsVoicemail</span></span>

<span data-ttu-id="77269-104">O elemento **Iscaixa postal** indica se as mensagens de entrada devem ser mensagens de caixa postal para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="77269-104">The **IsVoicemail** element indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span> 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
```

 <span data-ttu-id="77269-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="77269-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77269-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="77269-106">Attributes and elements</span></span>

<span data-ttu-id="77269-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="77269-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77269-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="77269-108">Attributes</span></span>

<span data-ttu-id="77269-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77269-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77269-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="77269-110">Child elements</span></span>

<span data-ttu-id="77269-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77269-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="77269-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="77269-112">Parent elements</span></span>

|<span data-ttu-id="77269-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77269-113">**Element**</span></span>|<span data-ttu-id="77269-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77269-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77269-115">Condições</span><span class="sxs-lookup"><span data-stu-id="77269-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="77269-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="77269-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="77269-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="77269-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="77269-118">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="77269-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77269-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="77269-119">Text value</span></span>

<span data-ttu-id="77269-120">Um valor de texto **true** indica que a mensagem deve ser uma mensagem de caixa postal para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="77269-120">A text value of **true** indicates that the message must be a voice mail message in order for the condition or exception to apply.</span></span> <span data-ttu-id="77269-121">Um valor **false** indica que a mensagem não deve ser uma mensagem de caixa postal para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="77269-121">A value of **false** indicates that the message must not be a voice mail message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="77269-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="77269-122">Remarks</span></span>

<span data-ttu-id="77269-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77269-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77269-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="77269-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77269-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="77269-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77269-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="77269-126">Schema Name</span></span>  <br/> |<span data-ttu-id="77269-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="77269-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77269-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="77269-128">Validation File</span></span>  <br/> |<span data-ttu-id="77269-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77269-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77269-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="77269-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="77269-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="77269-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77269-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="77269-132">See also</span></span>



- [<span data-ttu-id="77269-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77269-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

