---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: O elemento MinimumSize representa o tamanho mínimo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 4f80bac3b9226019ec3d726cd2d6430e02cac423
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824480"
---
# <a name="minimumsize"></a><span data-ttu-id="e7a79-103">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="e7a79-103">MinimumSize</span></span>

<span data-ttu-id="e7a79-104">O elemento **MinimumSize** representa o tamanho mínimo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e7a79-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="e7a79-105">**int**</span><span class="sxs-lookup"><span data-stu-id="e7a79-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7a79-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e7a79-106">Attributes and elements</span></span>

<span data-ttu-id="e7a79-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e7a79-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7a79-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e7a79-108">Attributes</span></span>

<span data-ttu-id="e7a79-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7a79-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7a79-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e7a79-110">Child elements</span></span>

<span data-ttu-id="e7a79-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7a79-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7a79-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e7a79-112">Parent elements</span></span>

|<span data-ttu-id="e7a79-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7a79-113">**Element**</span></span>|<span data-ttu-id="e7a79-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7a79-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7a79-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="e7a79-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="e7a79-116">Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e7a79-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7a79-117">Text value</span><span class="sxs-lookup"><span data-stu-id="e7a79-117">Text value</span></span>

<span data-ttu-id="e7a79-118">O valor de texto é um inteiro que identifica o tamanho mínimo da mensagem em bytes.</span><span class="sxs-lookup"><span data-stu-id="e7a79-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7a79-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="e7a79-119">Remarks</span></span>

<span data-ttu-id="e7a79-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7a79-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7a79-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e7a79-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7a79-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7a79-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7a79-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e7a79-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e7a79-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e7a79-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7a79-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e7a79-125">Validation File</span></span>  <br/> |<span data-ttu-id="e7a79-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e7a79-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7a79-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e7a79-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7a79-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e7a79-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7a79-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="e7a79-129">See also</span></span>



[<span data-ttu-id="e7a79-130">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="e7a79-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="e7a79-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e7a79-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

