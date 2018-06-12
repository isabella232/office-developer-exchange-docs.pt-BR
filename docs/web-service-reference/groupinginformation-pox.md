---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: O elemento GroupingInformation contém um valor que é usado para a caixa de correio do usuário para manter a afinidade quando a assinatura de notificações em várias caixas de correio de grupo.
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823781"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="6d00f-103">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="6d00f-104">O elemento **GroupingInformation** contém um valor que é usado para agrupar a caixa de correio do usuário para [manter a afinidade](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) quando a assinatura de notificações em várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="6d00f-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="6d00f-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6d00f-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6d00f-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6d00f-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6d00f-109">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6d00f-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6d00f-110">Attributes and elements</span></span>

<span data-ttu-id="6d00f-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6d00f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d00f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6d00f-112">Attributes</span></span>

<span data-ttu-id="6d00f-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d00f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d00f-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6d00f-114">Child elements</span></span>

<span data-ttu-id="6d00f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d00f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d00f-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6d00f-116">Parent elements</span></span>

|<span data-ttu-id="6d00f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d00f-117">**Element**</span></span>|<span data-ttu-id="6d00f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d00f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d00f-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="6d00f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6d00f-120">Contém as especificações para conectar um cliente para o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="6d00f-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d00f-121">Text value</span><span class="sxs-lookup"><span data-stu-id="6d00f-121">Text value</span></span>

<span data-ttu-id="6d00f-122">O valor de texto é comparado com o valor do elemento **GroupingInformation** para outras caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="6d00f-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="6d00f-123">Caixas de correio que têm o mesmo valor e usar o mesmo ponto de extremidade de serviços Web do Exchange (EWS) podem ser agrupadas para manter a afinidade.</span><span class="sxs-lookup"><span data-stu-id="6d00f-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="6d00f-124">Para obter mais detalhes, consulte [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6d00f-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6d00f-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="6d00f-125">Remarks</span></span>

<span data-ttu-id="6d00f-126">O elemento **GroupingInformation** só é aplicável aos elementos de **protocolo** que têm um elemento filho de [Tipo POX ()](type-pox.md) com um valor de "EXPR".</span><span class="sxs-lookup"><span data-stu-id="6d00f-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6d00f-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="6d00f-127">See also</span></span>

- [<span data-ttu-id="6d00f-128">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="6d00f-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="6d00f-129">Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange</span><span class="sxs-lookup"><span data-stu-id="6d00f-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

