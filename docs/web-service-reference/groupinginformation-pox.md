---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: O elemento GroupingInformation contém um valor usado para agrupar a caixa de correio do usuário para manter a afinidade ao assinar notificações em várias caixas de correio.
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530075"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="8ed58-103">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="8ed58-104">O elemento **GroupingInformation** contém um valor usado para agrupar a caixa de correio do usuário para [manter a afinidade](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) ao assinar notificações em várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="8ed58-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="8ed58-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8ed58-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8ed58-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8ed58-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8ed58-109">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8ed58-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8ed58-110">Attributes and elements</span></span>

<span data-ttu-id="8ed58-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8ed58-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ed58-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8ed58-112">Attributes</span></span>

<span data-ttu-id="8ed58-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ed58-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ed58-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8ed58-114">Child elements</span></span>

<span data-ttu-id="8ed58-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ed58-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ed58-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8ed58-116">Parent elements</span></span>

|<span data-ttu-id="8ed58-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8ed58-117">**Element**</span></span>|<span data-ttu-id="8ed58-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ed58-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ed58-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8ed58-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8ed58-120">Contém as especificações para conectar um cliente ao servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ed58-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ed58-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8ed58-121">Text value</span></span>

<span data-ttu-id="8ed58-122">O valor de texto é comparado com o valor do elemento **GroupingInformation** para outras caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="8ed58-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="8ed58-123">As caixas de correio que têm o mesmo valor e usam o mesmo ponto de extremidade do EWS (serviços Web do Exchange) podem ser agrupadas para manter a afinidade.</span><span class="sxs-lookup"><span data-stu-id="8ed58-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="8ed58-124">Para obter mais detalhes, consulte [manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8ed58-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ed58-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="8ed58-125">Remarks</span></span>

<span data-ttu-id="8ed58-126">O elemento **GroupingInformation** só é aplicável a elementos de **protocolo** que têm um elemento filho [tipo (POX)](type-pox.md) com um valor de "expr".</span><span class="sxs-lookup"><span data-stu-id="8ed58-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8ed58-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="8ed58-127">See also</span></span>

- [<span data-ttu-id="8ed58-128">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="8ed58-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="8ed58-129">Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange</span><span class="sxs-lookup"><span data-stu-id="8ed58-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

