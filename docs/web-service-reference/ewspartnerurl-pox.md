---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: O elemento EwsPartnerUrl especifica a URL da melhor instância de ponto de extremidade para os serviços Web do Exchange (EWS) para um usuário habilitado para email.
ms.openlocfilehash: a67eb17bb3db67a922c53ba5e37900ee0a9b956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526106"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="c1303-103">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="c1303-104">O elemento **EwsPartnerUrl** especifica a URL da melhor instância de ponto de extremidade para os serviços Web do Exchange (EWS) para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="c1303-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="c1303-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="c1303-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="c1303-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="c1303-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="c1303-109">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c1303-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c1303-110">Attributes and elements</span></span>

<span data-ttu-id="c1303-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c1303-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1303-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="c1303-112">Attributes</span></span>

<span data-ttu-id="c1303-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1303-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1303-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c1303-114">Child elements</span></span>

<span data-ttu-id="c1303-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c1303-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c1303-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c1303-116">Parent elements</span></span>

|<span data-ttu-id="c1303-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c1303-117">**Element**</span></span>|<span data-ttu-id="c1303-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1303-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1303-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c1303-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="c1303-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c1303-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1303-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c1303-121">Text value</span></span>

<span data-ttu-id="c1303-122">O valor de texto representa a URL do ponto de extremidade do EWS para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c1303-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c1303-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="c1303-123">Remarks</span></span>

<span data-ttu-id="c1303-124">O elemento **EwsPartnerUrl** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="c1303-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="c1303-125">É equivalente ao elemento [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="c1303-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c1303-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1303-126">See also</span></span>



[<span data-ttu-id="c1303-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="c1303-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

