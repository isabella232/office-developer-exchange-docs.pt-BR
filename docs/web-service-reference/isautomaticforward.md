---
title: IsAutomaticForward
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticForward
api_type:
- schema
ms.assetid: 6876b849-a648-482e-8934-93eb5a0c465f
description: O elemento IsAutomaticForward indica se as mensagens de entrada devem ser encaminhamentos automáticos para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 800d38bab30245d88b3c09609e6235e6de8fed25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455573"
---
# <a name="isautomaticforward"></a><span data-ttu-id="01900-103">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="01900-103">IsAutomaticForward</span></span>

<span data-ttu-id="01900-104">O elemento **IsAutomaticForward** indica se as mensagens de entrada devem ser encaminhamentos automáticos para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="01900-104">The **IsAutomaticForward** element indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticForward/> true | false</IsAutomaticForward>
```

 <span data-ttu-id="01900-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="01900-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01900-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="01900-106">Attributes and elements</span></span>

<span data-ttu-id="01900-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01900-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01900-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01900-108">Attributes</span></span>

<span data-ttu-id="01900-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01900-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01900-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01900-110">Child elements</span></span>

<span data-ttu-id="01900-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01900-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01900-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01900-112">Parent elements</span></span>

|<span data-ttu-id="01900-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01900-113">**Element**</span></span>|<span data-ttu-id="01900-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01900-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01900-115">Condições</span><span class="sxs-lookup"><span data-stu-id="01900-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="01900-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="01900-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="01900-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="01900-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="01900-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="01900-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01900-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="01900-119">Text value</span></span>

<span data-ttu-id="01900-120">Um valor de texto **true** indica que a mensagem deve ser um avanço automático para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="01900-120">A text value of **true** indicates that the message must be an automatic forward in order for the condition or exception to apply.</span></span> <span data-ttu-id="01900-121">Um valor **false** indica que a mensagem não deve ser um avanço automático para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="01900-121">A value of **false** indicates that the message must not be an automatic forward in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01900-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="01900-122">Remarks</span></span>

<span data-ttu-id="01900-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01900-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01900-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="01900-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01900-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="01900-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01900-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01900-126">Schema Name</span></span>  <br/> |<span data-ttu-id="01900-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="01900-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01900-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01900-128">Validation File</span></span>  <br/> |<span data-ttu-id="01900-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01900-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01900-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="01900-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="01900-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="01900-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01900-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="01900-132">See also</span></span>



- [<span data-ttu-id="01900-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01900-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

