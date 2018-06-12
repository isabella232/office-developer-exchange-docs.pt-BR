---
title: EcpUrl-resposta POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5f090fd2-b0c4-4ca0-a959-1433d73a2069
description: O elemento de resposta de EcpUrl Especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl POX () para gerar uma URL que pode ser usada para acessar as configurações de marca de retenção para um usuário habilitado para email.
ms.openlocfilehash: 366a7a79c0f3c19b2cfef21c01826e62b0e95793
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751959"
---
# <a name="ecpurl-ret-pox"></a><span data-ttu-id="330f2-103">EcpUrl-resposta POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-103">EcpUrl-ret (POX)</span></span>

<span data-ttu-id="330f2-104">O elemento de **resposta de EcpUrl** Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de marca de retenção para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="330f2-104">The **EcpUrl-ret** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="330f2-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="330f2-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="330f2-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="330f2-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="330f2-109">EcpUrl-resposta POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-109">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md)
  
```XML
<EcpUrl-ret/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="330f2-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="330f2-110">Attributes and elements</span></span>

<span data-ttu-id="330f2-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="330f2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="330f2-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="330f2-112">Attributes</span></span>

<span data-ttu-id="330f2-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="330f2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="330f2-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="330f2-114">Child elements</span></span>

<span data-ttu-id="330f2-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="330f2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="330f2-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="330f2-116">Parent elements</span></span>

|<span data-ttu-id="330f2-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="330f2-117">**Element**</span></span>|<span data-ttu-id="330f2-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="330f2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="330f2-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="330f2-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="330f2-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="330f2-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="330f2-121">Text value</span><span class="sxs-lookup"><span data-stu-id="330f2-121">Text value</span></span>

<span data-ttu-id="330f2-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de marca de retenção para o usuário.</span><span class="sxs-lookup"><span data-stu-id="330f2-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="330f2-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="330f2-123">Remarks</span></span>

<span data-ttu-id="330f2-124">A **resposta de EcpUrl** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="330f2-124">The **EcpUrl-ret** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="330f2-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="330f2-125">See also</span></span>



[<span data-ttu-id="330f2-126">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="330f2-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

