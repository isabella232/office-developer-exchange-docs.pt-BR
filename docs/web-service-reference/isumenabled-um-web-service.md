---
title: IsUMEnabled (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: O elemento IsUMEnabled indica se uma caixa de correio está habilitada para Unificação de mensagens.
ms.openlocfilehash: 5f4d59c5497158e5afbc8bb5db4900bd129df50b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824113"
---
# <a name="isumenabled-um-web-service"></a><span data-ttu-id="c13f0-103">IsUMEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c13f0-103">IsUMEnabled (UM web service)</span></span>

<span data-ttu-id="c13f0-104">O elemento **IsUMEnabled** indica se uma caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="c13f0-104">The **IsUMEnabled** element indicates whether a mailbox is enabled for Unified Messaging.</span></span> 
  
```xml
<IsUMEnabled/>
```

 <span data-ttu-id="c13f0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c13f0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c13f0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c13f0-106">Attributes and elements</span></span>

<span data-ttu-id="c13f0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c13f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c13f0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c13f0-108">Attributes</span></span>

<span data-ttu-id="c13f0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c13f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c13f0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c13f0-110">Child elements</span></span>

<span data-ttu-id="c13f0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c13f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c13f0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c13f0-112">Parent elements</span></span>

<span data-ttu-id="c13f0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c13f0-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c13f0-114">Text value</span><span class="sxs-lookup"><span data-stu-id="c13f0-114">Text value</span></span>

<span data-ttu-id="c13f0-115">Um valor de texto que representa um valor booleano é necessário se este elemento é incluído.</span><span class="sxs-lookup"><span data-stu-id="c13f0-115">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="c13f0-116">Um valor **true** indica que a caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="c13f0-116">A value of **true** indicates that the mailbox is enabled for Unified Messaging.</span></span> <span data-ttu-id="c13f0-117">Um valor **false** significa que a caixa de correio não está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="c13f0-117">A value of **false** means that the mailbox is not enabled for Unified Messaging.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c13f0-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="c13f0-118">Remarks</span></span>

<span data-ttu-id="c13f0-119">Para determinar se uma caixa de correio está habilitada para Unificação de mensagens, use a [operação IsUMEnabled (serviço web de Unificação de mensagens)](isumenabled-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="c13f0-119">To determine whether a mailbox is enabled for Unified Messaging, use the [IsUMEnabled operation (UM web service)](isumenabled-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c13f0-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c13f0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c13f0-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="c13f0-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c13f0-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c13f0-122">Schema Name</span></span>  <br/> |<span data-ttu-id="c13f0-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="c13f0-123">Messages</span></span>  <br/> |
|<span data-ttu-id="c13f0-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c13f0-124">Validation File</span></span>  <br/> |<span data-ttu-id="c13f0-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c13f0-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c13f0-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c13f0-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="c13f0-127">False</span><span class="sxs-lookup"><span data-stu-id="c13f0-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c13f0-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="c13f0-128">See also</span></span>



[<span data-ttu-id="c13f0-129">Operação de IsUMEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c13f0-129">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)


[<span data-ttu-id="c13f0-130">Unified Messaging web service os elementos XML para o Exchange</span><span class="sxs-lookup"><span data-stu-id="c13f0-130">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

