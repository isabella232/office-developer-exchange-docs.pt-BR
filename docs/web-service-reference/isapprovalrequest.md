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
description: O elemento IsApprovalRequest indica se as mensagens de entrada devem ser solicitações de aprovação em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 45b0836efff3ec9fe644cbaeb7ea7192346422bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823984"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="32939-103">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="32939-103">IsApprovalRequest</span></span>

<span data-ttu-id="32939-104">O elemento **IsApprovalRequest** indica se as mensagens de entrada devem ser solicitações de aprovação em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="32939-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="32939-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="32939-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32939-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="32939-106">Attributes and elements</span></span>

<span data-ttu-id="32939-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="32939-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32939-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="32939-108">Attributes</span></span>

<span data-ttu-id="32939-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32939-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32939-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="32939-110">Child elements</span></span>

<span data-ttu-id="32939-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32939-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32939-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="32939-112">Parent elements</span></span>

|<span data-ttu-id="32939-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="32939-113">**Element**</span></span>|<span data-ttu-id="32939-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="32939-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32939-115">Condições</span><span class="sxs-lookup"><span data-stu-id="32939-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="32939-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="32939-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="32939-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="32939-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="32939-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="32939-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32939-119">Text value</span><span class="sxs-lookup"><span data-stu-id="32939-119">Text value</span></span>

<span data-ttu-id="32939-120">Um valor de texto de **true** indica que a mensagem deve ser uma solicitação de aprovação em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="32939-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="32939-121">Um valor **false** indica que a mensagem não deve ser uma solicitação de aprovação em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="32939-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="32939-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="32939-122">Remarks</span></span>

<span data-ttu-id="32939-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="32939-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32939-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="32939-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32939-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="32939-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32939-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="32939-126">Schema Name</span></span>  <br/> |<span data-ttu-id="32939-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="32939-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32939-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="32939-128">Validation File</span></span>  <br/> |<span data-ttu-id="32939-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32939-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32939-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="32939-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="32939-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="32939-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32939-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="32939-132">See also</span></span>



- [<span data-ttu-id="32939-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="32939-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

