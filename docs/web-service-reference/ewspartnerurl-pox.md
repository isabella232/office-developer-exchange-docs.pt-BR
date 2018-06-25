---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: O elemento EwsPartnerUrl Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.
ms.openlocfilehash: 97c33e1fed4adc8a9e8542d85e67c942118f6096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752124"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="d9140-103">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="d9140-104">O elemento **EwsPartnerUrl** Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="d9140-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="d9140-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d9140-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d9140-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d9140-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d9140-109">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d9140-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d9140-110">Attributes and elements</span></span>

<span data-ttu-id="d9140-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9140-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9140-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9140-112">Attributes</span></span>

<span data-ttu-id="d9140-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9140-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9140-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9140-114">Child elements</span></span>

<span data-ttu-id="d9140-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9140-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9140-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9140-116">Parent elements</span></span>

|<span data-ttu-id="d9140-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9140-117">**Element**</span></span>|<span data-ttu-id="d9140-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9140-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9140-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="d9140-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d9140-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d9140-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9140-121">Text value</span><span class="sxs-lookup"><span data-stu-id="d9140-121">Text value</span></span>

<span data-ttu-id="d9140-122">O valor de texto representa a URL do ponto de extremidade EWS para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d9140-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9140-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9140-123">Remarks</span></span>

<span data-ttu-id="d9140-124">O **EwsPartnerUrl** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="d9140-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="d9140-125">É equivalente ao elemento [EwsUrl POX ()](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="d9140-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d9140-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9140-126">See also</span></span>



[<span data-ttu-id="d9140-127">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="d9140-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

