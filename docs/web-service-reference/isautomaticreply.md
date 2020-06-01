---
title: IsAutomaticReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAutomaticReply
api_type:
- schema
ms.assetid: 280e9baf-199d-422c-8fdf-1d0751a3e77d
description: O elemento IsAutomaticReply indica se as mensagens de entrada devem ser respostas automáticas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 7521dbbb458cf7683b52b2fe4fddacd276b40256
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455559"
---
# <a name="isautomaticreply"></a><span data-ttu-id="0e58d-103">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="0e58d-103">IsAutomaticReply</span></span>

<span data-ttu-id="0e58d-104">O elemento **IsAutomaticReply** indica se as mensagens de entrada devem ser respostas automáticas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="0e58d-104">The **IsAutomaticReply** element indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span> 
  
```XML
<IsAutomaticReply> true | false</IsAutomaticReply>
```

 <span data-ttu-id="0e58d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0e58d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e58d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0e58d-106">Attributes and elements</span></span>

<span data-ttu-id="0e58d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0e58d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e58d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0e58d-108">Attributes</span></span>

<span data-ttu-id="0e58d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e58d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e58d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0e58d-110">Child elements</span></span>

<span data-ttu-id="0e58d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e58d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e58d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0e58d-112">Parent elements</span></span>

|<span data-ttu-id="0e58d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e58d-113">**Element**</span></span>|<span data-ttu-id="0e58d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e58d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e58d-115">Condições</span><span class="sxs-lookup"><span data-stu-id="0e58d-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0e58d-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="0e58d-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0e58d-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="0e58d-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0e58d-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="0e58d-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e58d-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0e58d-119">Text value</span></span>

<span data-ttu-id="0e58d-120">Um valor de texto **true** indica que a mensagem deve ser uma resposta automática para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="0e58d-120">A text value of **true** indicates that the message must be an automatic reply in order for the condition or exception to apply.</span></span> <span data-ttu-id="0e58d-121">Um valor **false** indica que a mensagem não precisa ser uma resposta automática para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="0e58d-121">A value of **false** indicates that the message does not have to be an automatic reply in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e58d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e58d-122">Remarks</span></span>

<span data-ttu-id="0e58d-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e58d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e58d-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0e58d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e58d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e58d-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0e58d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0e58d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0e58d-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0e58d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0e58d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0e58d-128">Validation File</span></span>  <br/> |<span data-ttu-id="0e58d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0e58d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e58d-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0e58d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e58d-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0e58d-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e58d-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0e58d-132">See also</span></span>



- [<span data-ttu-id="0e58d-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0e58d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

