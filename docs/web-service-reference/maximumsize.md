---
title: MaximumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: O elemento MaximumSize representa o tamanho máximo que uma mensagem deve ter para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 250e0c6aed37b934f5cf6eaed9d93b9f56159d93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461748"
---
# <a name="maximumsize"></a><span data-ttu-id="6bb38-103">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="6bb38-103">MaximumSize</span></span>

<span data-ttu-id="6bb38-104">O elemento **MaximumSize** representa o tamanho máximo que uma mensagem deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="6bb38-104">The **MaximumSize** element represents the maximum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<Maximum/>
```

 <span data-ttu-id="6bb38-105">**int**</span><span class="sxs-lookup"><span data-stu-id="6bb38-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bb38-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6bb38-106">Attributes and elements</span></span>

<span data-ttu-id="6bb38-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6bb38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bb38-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6bb38-108">Attributes</span></span>

<span data-ttu-id="6bb38-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bb38-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bb38-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6bb38-110">Child elements</span></span>

<span data-ttu-id="6bb38-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6bb38-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bb38-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6bb38-112">Parent elements</span></span>

|<span data-ttu-id="6bb38-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6bb38-113">**Element**</span></span>|<span data-ttu-id="6bb38-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6bb38-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bb38-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="6bb38-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="6bb38-116">Especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="6bb38-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bb38-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6bb38-117">Text value</span></span>

<span data-ttu-id="6bb38-118">O valor de texto é um inteiro que identifica o tamanho máximo da mensagem em bytes.</span><span class="sxs-lookup"><span data-stu-id="6bb38-118">The text value is an integer that identifies the maximum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6bb38-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="6bb38-119">Remarks</span></span>

<span data-ttu-id="6bb38-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bb38-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bb38-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6bb38-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bb38-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="6bb38-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6bb38-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6bb38-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6bb38-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6bb38-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6bb38-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6bb38-125">Validation File</span></span>  <br/> |<span data-ttu-id="6bb38-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6bb38-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6bb38-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6bb38-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6bb38-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6bb38-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bb38-129">Também consulte</span><span class="sxs-lookup"><span data-stu-id="6bb38-129">See also</span></span>



[<span data-ttu-id="6bb38-130">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="6bb38-130">MinimumSize</span></span>](minimumsize.md)


- [<span data-ttu-id="6bb38-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6bb38-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

