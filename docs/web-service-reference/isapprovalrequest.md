---
title: IsApprovalRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsApprovalRequest
api_type:
- schema
ms.assetid: 293ed01b-f6a4-4459-819c-933bbfaa2dd7
description: O elemento IsApprovalRequest indica se as mensagens de entrada devem ser solicitações de aprovação para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 08ea36820b2680bb2c7e5695eb2dd481154c05eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530006"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="5d421-103">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="5d421-103">IsApprovalRequest</span></span>

<span data-ttu-id="5d421-104">O elemento **IsApprovalRequest** indica se as mensagens de entrada devem ser solicitações de aprovação para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="5d421-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="5d421-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5d421-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d421-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5d421-106">Attributes and elements</span></span>

<span data-ttu-id="5d421-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d421-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d421-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d421-108">Attributes</span></span>

<span data-ttu-id="5d421-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d421-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d421-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d421-110">Child elements</span></span>

<span data-ttu-id="5d421-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d421-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d421-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d421-112">Parent elements</span></span>

|<span data-ttu-id="5d421-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d421-113">**Element**</span></span>|<span data-ttu-id="5d421-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d421-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d421-115">Condições</span><span class="sxs-lookup"><span data-stu-id="5d421-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="5d421-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="5d421-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="5d421-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="5d421-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="5d421-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="5d421-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d421-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5d421-119">Text value</span></span>

<span data-ttu-id="5d421-120">Um valor de texto **true** indica que a mensagem deve ser uma solicitação de aprovação para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="5d421-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="5d421-121">Um valor **false** indica que a mensagem não deve ser uma solicitação de aprovação para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="5d421-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5d421-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="5d421-122">Remarks</span></span>

<span data-ttu-id="5d421-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d421-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d421-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5d421-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d421-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d421-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d421-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5d421-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5d421-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5d421-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d421-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5d421-128">Validation File</span></span>  <br/> |<span data-ttu-id="5d421-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d421-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d421-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5d421-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d421-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5d421-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d421-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="5d421-132">See also</span></span>



- [<span data-ttu-id="5d421-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5d421-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

