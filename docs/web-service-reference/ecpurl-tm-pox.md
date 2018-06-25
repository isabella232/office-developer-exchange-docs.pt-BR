---
title: EcpUrl-tm POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: O elemento EcpUrl-tm Especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl POX () para gerar uma URL que pode ser usada para acessar uma lista de todas as caixas de correio de site dos quais um usuário habilitado para email é membro atualmente.
ms.openlocfilehash: 786459cab98f8c169f768b6ef850792e8111761a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751955"
---
# <a name="ecpurl-tm-pox"></a><span data-ttu-id="256b8-103">EcpUrl-tm POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-103">EcpUrl-tm (POX)</span></span>

<span data-ttu-id="256b8-104">O elemento **EcpUrl-tm** Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de todas as caixas de correio de site dos quais um usuário habilitado para email é membro atualmente.</span><span class="sxs-lookup"><span data-stu-id="256b8-104">The **EcpUrl-tm** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span> 
  
[<span data-ttu-id="256b8-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="256b8-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="256b8-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="256b8-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="256b8-109">EcpUrl-tm POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-109">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="256b8-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="256b8-110">Attributes and elements</span></span>

<span data-ttu-id="256b8-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="256b8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="256b8-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="256b8-112">Attributes</span></span>

<span data-ttu-id="256b8-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="256b8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="256b8-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="256b8-114">Child elements</span></span>

<span data-ttu-id="256b8-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="256b8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="256b8-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="256b8-116">Parent elements</span></span>

|<span data-ttu-id="256b8-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="256b8-117">**Element**</span></span>|<span data-ttu-id="256b8-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="256b8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="256b8-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="256b8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="256b8-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="256b8-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="256b8-121">Text value</span><span class="sxs-lookup"><span data-stu-id="256b8-121">Text value</span></span>

<span data-ttu-id="256b8-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de caixas de correio de site para o usuário.</span><span class="sxs-lookup"><span data-stu-id="256b8-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of site mailboxes for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="256b8-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="256b8-123">Remarks</span></span>

<span data-ttu-id="256b8-124">O **EcpUrl-tm** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="256b8-124">The **EcpUrl-tm** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="256b8-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="256b8-125">See also</span></span>



[<span data-ttu-id="256b8-126">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="256b8-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

