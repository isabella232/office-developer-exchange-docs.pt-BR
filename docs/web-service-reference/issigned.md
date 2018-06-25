---
title: IsSigned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsSigned
api_type:
- schema
ms.assetid: a4f90fe5-2834-4621-9aa3-b561f74d4674
description: O elemento IsSigned indica se as mensagens de entrada devem ser assinadas em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 33ff204260465490c701c6573ff4140967ac625a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824105"
---
# <a name="issigned"></a><span data-ttu-id="27c3d-103">IsSigned</span><span class="sxs-lookup"><span data-stu-id="27c3d-103">IsSigned</span></span>

<span data-ttu-id="27c3d-104">O elemento **IsSigned** indica se as mensagens de entrada devem ser assinadas em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="27c3d-104">The **IsSigned** element indicates whether incoming messages must be signed in order for the condition or exception to apply.</span></span> 
  
```XML
<IsSigned>true | false</IsSigned>
```

 <span data-ttu-id="27c3d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="27c3d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27c3d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="27c3d-106">Attributes and elements</span></span>

<span data-ttu-id="27c3d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="27c3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27c3d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="27c3d-108">Attributes</span></span>

<span data-ttu-id="27c3d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="27c3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27c3d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="27c3d-110">Child elements</span></span>

<span data-ttu-id="27c3d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="27c3d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27c3d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="27c3d-112">Parent elements</span></span>

|<span data-ttu-id="27c3d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="27c3d-113">**Element**</span></span>|<span data-ttu-id="27c3d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="27c3d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27c3d-115">Condições</span><span class="sxs-lookup"><span data-stu-id="27c3d-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="27c3d-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="27c3d-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="27c3d-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="27c3d-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="27c3d-118">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="27c3d-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27c3d-119">Text value</span><span class="sxs-lookup"><span data-stu-id="27c3d-119">Text value</span></span>

<span data-ttu-id="27c3d-120">Um valor de texto de **true** indica que a mensagem deve ser assinada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="27c3d-120">A text value of **true** indicates that the message must be signed in order for the condition or exception to apply.</span></span> <span data-ttu-id="27c3d-121">Um valor de texto de **false** indica que a mensagem não precisa estar conectado para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="27c3d-121">A text value of **false** indicates that the message does not have to be signed for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="27c3d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="27c3d-122">Remarks</span></span>

<span data-ttu-id="27c3d-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="27c3d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27c3d-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="27c3d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27c3d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="27c3d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27c3d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="27c3d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="27c3d-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="27c3d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27c3d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="27c3d-128">Validation File</span></span>  <br/> |<span data-ttu-id="27c3d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27c3d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27c3d-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="27c3d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="27c3d-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="27c3d-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27c3d-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="27c3d-132">See also</span></span>



- [<span data-ttu-id="27c3d-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="27c3d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

