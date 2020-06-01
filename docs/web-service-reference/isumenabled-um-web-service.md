---
title: IsUMEnabled (serviço Web da UM)
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
ms.openlocfilehash: ea5bde677c62664acad8afd5c8142e96d82b7a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458226"
---
# <a name="isumenabled-um-web-service"></a><span data-ttu-id="a91ca-103">IsUMEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="a91ca-103">IsUMEnabled (UM web service)</span></span>

<span data-ttu-id="a91ca-104">O elemento **IsUMEnabled** indica se uma caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="a91ca-104">The **IsUMEnabled** element indicates whether a mailbox is enabled for Unified Messaging.</span></span> 
  
```xml
<IsUMEnabled/>
```

 <span data-ttu-id="a91ca-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a91ca-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a91ca-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a91ca-106">Attributes and elements</span></span>

<span data-ttu-id="a91ca-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a91ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a91ca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a91ca-108">Attributes</span></span>

<span data-ttu-id="a91ca-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a91ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a91ca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a91ca-110">Child elements</span></span>

<span data-ttu-id="a91ca-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a91ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a91ca-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a91ca-112">Parent elements</span></span>

<span data-ttu-id="a91ca-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a91ca-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a91ca-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a91ca-114">Text value</span></span>

<span data-ttu-id="a91ca-115">Um valor de texto que representa um valor booliano é necessário se esse elemento for incluído.</span><span class="sxs-lookup"><span data-stu-id="a91ca-115">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="a91ca-116">Um valor **true** indica que a caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="a91ca-116">A value of **true** indicates that the mailbox is enabled for Unified Messaging.</span></span> <span data-ttu-id="a91ca-117">Um valor **false** significa que a caixa de correio não está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="a91ca-117">A value of **false** means that the mailbox is not enabled for Unified Messaging.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a91ca-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="a91ca-118">Remarks</span></span>

<span data-ttu-id="a91ca-119">Para determinar se uma caixa de correio está habilitada para Unificação de mensagens, use a [operação IsUMEnabled (serviço da um da Web)](isumenabled-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="a91ca-119">To determine whether a mailbox is enabled for Unified Messaging, use the [IsUMEnabled operation (UM web service)](isumenabled-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a91ca-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a91ca-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a91ca-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="a91ca-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a91ca-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a91ca-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a91ca-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="a91ca-123">Messages</span></span>  <br/> |
|<span data-ttu-id="a91ca-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a91ca-124">Validation File</span></span>  <br/> |<span data-ttu-id="a91ca-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a91ca-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a91ca-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a91ca-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a91ca-127">False</span><span class="sxs-lookup"><span data-stu-id="a91ca-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a91ca-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="a91ca-128">See also</span></span>



[<span data-ttu-id="a91ca-129">Operação IsUMEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="a91ca-129">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)


[<span data-ttu-id="a91ca-130">Elementos XML do serviço Web de Unificação de mensagens para o Exchange</span><span class="sxs-lookup"><span data-stu-id="a91ca-130">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

