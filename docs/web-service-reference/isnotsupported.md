---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: O elemento IsNotSupported indica se a regra não pode ser modificada usando-se as APIs de código gerenciado.
ms.openlocfilehash: 2468d47dbfdcaf1a28ed1a4afb1e7ea60147d1dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824057"
---
# <a name="isnotsupported"></a><span data-ttu-id="efd38-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="efd38-103">IsNotSupported</span></span>

<span data-ttu-id="efd38-104">O elemento **IsNotSupported** indica se a regra não pode ser modificada usando-se as APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="efd38-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="efd38-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="efd38-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="efd38-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="efd38-106">Attributes and elements</span></span>

<span data-ttu-id="efd38-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="efd38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="efd38-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="efd38-108">Attributes</span></span>

<span data-ttu-id="efd38-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efd38-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="efd38-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="efd38-110">Child elements</span></span>

<span data-ttu-id="efd38-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efd38-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="efd38-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="efd38-112">Parent elements</span></span>

|<span data-ttu-id="efd38-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="efd38-113">**Element**</span></span>|<span data-ttu-id="efd38-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="efd38-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="efd38-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="efd38-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="efd38-116">Representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="efd38-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="efd38-117">Text value</span><span class="sxs-lookup"><span data-stu-id="efd38-117">Text value</span></span>

<span data-ttu-id="efd38-118">Um valor de texto de **true** indica que a regra não pode ser modificada usando-se as APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="efd38-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="efd38-119">Um valor **false** indica que a regra pode ser modificada usando o APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="efd38-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="efd38-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="efd38-120">Remarks</span></span>

<span data-ttu-id="efd38-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="efd38-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="efd38-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="efd38-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="efd38-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="efd38-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="efd38-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="efd38-124">Schema Name</span></span>  <br/> |<span data-ttu-id="efd38-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="efd38-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="efd38-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="efd38-126">Validation File</span></span>  <br/> |<span data-ttu-id="efd38-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="efd38-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="efd38-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="efd38-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="efd38-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="efd38-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="efd38-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="efd38-130">See also</span></span>



- [<span data-ttu-id="efd38-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="efd38-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

