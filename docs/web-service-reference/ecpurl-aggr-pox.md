---
title: EcpUrl-aggr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: O elemento EcpUrl-aggr especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar as configurações de agregação de email para um usuário habilitado para email.
ms.openlocfilehash: 26e855900154fb965eae9ba90a373b88e85c2ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457281"
---
# <a name="ecpurl-aggr-pox"></a><span data-ttu-id="4fb10-103">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-103">EcpUrl-aggr (POX)</span></span>

<span data-ttu-id="4fb10-104">O elemento **EcpUrl-aggr** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de agregação de email para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="4fb10-104">The **EcpUrl-aggr** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="4fb10-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="4fb10-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="4fb10-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="4fb10-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="4fb10-109">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-109">EcpUrl-aggr (POX)</span></span>](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4fb10-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4fb10-110">Attributes and elements</span></span>

<span data-ttu-id="4fb10-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4fb10-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fb10-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="4fb10-112">Attributes</span></span>

<span data-ttu-id="4fb10-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4fb10-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fb10-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4fb10-114">Child elements</span></span>

<span data-ttu-id="4fb10-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4fb10-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fb10-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4fb10-116">Parent elements</span></span>

|<span data-ttu-id="4fb10-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fb10-117">**Element**</span></span>|<span data-ttu-id="4fb10-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fb10-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fb10-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4fb10-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4fb10-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4fb10-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fb10-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4fb10-121">Text value</span></span>

<span data-ttu-id="4fb10-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de agregação de email para o usuário.</span><span class="sxs-lookup"><span data-stu-id="4fb10-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4fb10-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="4fb10-123">Remarks</span></span>

<span data-ttu-id="4fb10-124">O elemento **EcpUrl-aggr** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="4fb10-124">The **EcpUrl-aggr** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4fb10-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="4fb10-125">See also</span></span>



[<span data-ttu-id="4fb10-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="4fb10-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

