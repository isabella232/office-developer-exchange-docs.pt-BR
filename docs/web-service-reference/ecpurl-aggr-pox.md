---
title: EcpUrl-agregação (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: O elemento de agregação de EcpUrl Especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl POX () para gerar uma URL que pode ser usada para acessar as configurações de agregação de lista segura de email para um usuário habilitado para email.
ms.openlocfilehash: fb9bd92611998acc52fab0ea3e3c1ecb3e507faa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751942"
---
# <a name="ecpurl-aggr-pox"></a><span data-ttu-id="c8de0-103">EcpUrl-agregação (POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-103">EcpUrl-aggr (POX)</span></span>

<span data-ttu-id="c8de0-104">O elemento de **agregação de EcpUrl** Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de agregação de lista segura de email para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="c8de0-104">The **EcpUrl-aggr** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="c8de0-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="c8de0-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="c8de0-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="c8de0-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="c8de0-109">EcpUrl-agregação (POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-109">EcpUrl-aggr (POX)</span></span>](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c8de0-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c8de0-110">Attributes and elements</span></span>

<span data-ttu-id="c8de0-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c8de0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8de0-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="c8de0-112">Attributes</span></span>

<span data-ttu-id="c8de0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8de0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8de0-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c8de0-114">Child elements</span></span>

<span data-ttu-id="c8de0-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8de0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8de0-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c8de0-116">Parent elements</span></span>

|<span data-ttu-id="c8de0-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8de0-117">**Element**</span></span>|<span data-ttu-id="c8de0-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8de0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8de0-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="c8de0-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="c8de0-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c8de0-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8de0-121">Text value</span><span class="sxs-lookup"><span data-stu-id="c8de0-121">Text value</span></span>

<span data-ttu-id="c8de0-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de agregação de lista segura de email para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c8de0-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c8de0-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c8de0-123">Remarks</span></span>

<span data-ttu-id="c8de0-124">A **agregação de EcpUrl** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="c8de0-124">The **EcpUrl-aggr** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c8de0-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8de0-125">See also</span></span>



[<span data-ttu-id="c8de0-126">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="c8de0-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

