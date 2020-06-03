---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: O elemento MinimumSize representa o tamanho mínimo que uma mensagem deve ter para que a condição ou exceção seja aplicada.
ms.openlocfilehash: b43a8b5916747c4e3e4ca9b66cf8b9d73f5f8942
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464200"
---
# <a name="minimumsize"></a><span data-ttu-id="1995c-103">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="1995c-103">MinimumSize</span></span>

<span data-ttu-id="1995c-104">O elemento **MinimumSize** representa o tamanho mínimo que uma mensagem deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="1995c-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="1995c-105">**int**</span><span class="sxs-lookup"><span data-stu-id="1995c-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1995c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1995c-106">Attributes and elements</span></span>

<span data-ttu-id="1995c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1995c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1995c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1995c-108">Attributes</span></span>

<span data-ttu-id="1995c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1995c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1995c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1995c-110">Child elements</span></span>

<span data-ttu-id="1995c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1995c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1995c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1995c-112">Parent elements</span></span>

|<span data-ttu-id="1995c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1995c-113">**Element**</span></span>|<span data-ttu-id="1995c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1995c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1995c-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="1995c-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="1995c-116">Especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="1995c-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1995c-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1995c-117">Text value</span></span>

<span data-ttu-id="1995c-118">O valor de texto é um inteiro que identifica o tamanho mínimo da mensagem em bytes.</span><span class="sxs-lookup"><span data-stu-id="1995c-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1995c-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="1995c-119">Remarks</span></span>

<span data-ttu-id="1995c-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1995c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1995c-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1995c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1995c-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="1995c-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1995c-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1995c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1995c-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1995c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1995c-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1995c-125">Validation File</span></span>  <br/> |<span data-ttu-id="1995c-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1995c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1995c-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1995c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1995c-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="1995c-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1995c-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="1995c-129">See also</span></span>



[<span data-ttu-id="1995c-130">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="1995c-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="1995c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1995c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

