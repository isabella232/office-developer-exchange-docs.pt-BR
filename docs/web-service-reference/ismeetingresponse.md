---
title: IsMeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingResponse
api_type:
- schema
ms.assetid: 85090943-81c6-4fbe-a2db-007dced6a4cf
description: O elemento IsMeetngResponsequest indica se as mensagens de entrada devem ser uma resposta de reunião para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 40714b7e926768f55207d870b79f21f07163bb37
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465930"
---
# <a name="ismeetingresponse"></a><span data-ttu-id="80dd9-103">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="80dd9-103">IsMeetingResponse</span></span>

<span data-ttu-id="80dd9-104">O elemento **IsMeetngResponsequest** indica se as mensagens de entrada devem ser uma resposta de reunião para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="80dd9-104">The **IsMeetngResponsequest** element indicates whether incoming messages must be a meeting response in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
```

 <span data-ttu-id="80dd9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="80dd9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80dd9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="80dd9-106">Attributes and elements</span></span>

<span data-ttu-id="80dd9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="80dd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80dd9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="80dd9-108">Attributes</span></span>

<span data-ttu-id="80dd9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80dd9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80dd9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="80dd9-110">Child elements</span></span>

<span data-ttu-id="80dd9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="80dd9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80dd9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="80dd9-112">Parent elements</span></span>

|<span data-ttu-id="80dd9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="80dd9-113">**Element**</span></span>|<span data-ttu-id="80dd9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="80dd9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80dd9-115">Condições</span><span class="sxs-lookup"><span data-stu-id="80dd9-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="80dd9-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="80dd9-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="80dd9-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="80dd9-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="80dd9-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="80dd9-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80dd9-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="80dd9-119">Text value</span></span>

<span data-ttu-id="80dd9-120">Um valor de texto **true** indica que a mensagem deve ser uma resposta de reunião para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="80dd9-120">A text value of **true** indicates that the message must be a meeting response in order for the condition or exception to apply.</span></span> <span data-ttu-id="80dd9-121">Um valor **false** indica que a mensagem não deve ser uma resposta de reunião para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="80dd9-121">A text value of **false** indicates that the message must not be a meeting response in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="80dd9-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="80dd9-122">Remarks</span></span>

<span data-ttu-id="80dd9-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="80dd9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80dd9-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="80dd9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80dd9-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="80dd9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="80dd9-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="80dd9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="80dd9-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="80dd9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="80dd9-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="80dd9-128">Validation File</span></span>  <br/> |<span data-ttu-id="80dd9-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="80dd9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="80dd9-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="80dd9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="80dd9-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="80dd9-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80dd9-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="80dd9-132">See also</span></span>



- [<span data-ttu-id="80dd9-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="80dd9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

