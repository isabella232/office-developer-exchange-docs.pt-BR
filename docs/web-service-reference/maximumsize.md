---
title: MaximumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: O elemento MaximumSize representa o tamanho máximo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 37e3d377b105534fe34b54e262bd47bc450706da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824387"
---
# <a name="maximumsize"></a><span data-ttu-id="0dede-103">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="0dede-103">MaximumSize</span></span>

<span data-ttu-id="0dede-104">O elemento **MaximumSize** representa o tamanho máximo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="0dede-104">The **MaximumSize** element represents the maximum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<Maximum/>
```

 <span data-ttu-id="0dede-105">**int**</span><span class="sxs-lookup"><span data-stu-id="0dede-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dede-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0dede-106">Attributes and elements</span></span>

<span data-ttu-id="0dede-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0dede-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dede-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0dede-108">Attributes</span></span>

<span data-ttu-id="0dede-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0dede-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dede-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0dede-110">Child elements</span></span>

<span data-ttu-id="0dede-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0dede-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0dede-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0dede-112">Parent elements</span></span>

|<span data-ttu-id="0dede-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0dede-113">**Element**</span></span>|<span data-ttu-id="0dede-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0dede-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dede-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="0dede-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="0dede-116">Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="0dede-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0dede-117">Text value</span><span class="sxs-lookup"><span data-stu-id="0dede-117">Text value</span></span>

<span data-ttu-id="0dede-118">O valor de texto é um inteiro que identifica o tamanho máximo da mensagem em bytes.</span><span class="sxs-lookup"><span data-stu-id="0dede-118">The text value is an integer that identifies the maximum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0dede-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="0dede-119">Remarks</span></span>

<span data-ttu-id="0dede-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dede-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dede-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0dede-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dede-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="0dede-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0dede-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0dede-123">Schema Name</span></span>  <br/> |<span data-ttu-id="0dede-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0dede-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0dede-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0dede-125">Validation File</span></span>  <br/> |<span data-ttu-id="0dede-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0dede-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0dede-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0dede-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="0dede-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0dede-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dede-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="0dede-129">See also</span></span>



[<span data-ttu-id="0dede-130">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="0dede-130">MinimumSize</span></span>](minimumsize.md)


- [<span data-ttu-id="0dede-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0dede-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

