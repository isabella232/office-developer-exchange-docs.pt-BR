---
title: EcpUrl-RET (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5f090fd2-b0c4-4ca0-a959-1433d73a2069
description: O elemento EcpUrl-RET especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar as configurações da marca de retenção para um usuário habilitado para email.
ms.openlocfilehash: 1f6878dc58bb01fca6a56fdd645efd3363a3d442
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458688"
---
# <a name="ecpurl-ret-pox"></a><span data-ttu-id="d606a-103">EcpUrl-RET (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-103">EcpUrl-ret (POX)</span></span>

<span data-ttu-id="d606a-104">O elemento **EcpUrl-RET** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações da marca de retenção para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="d606a-104">The **EcpUrl-ret** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="d606a-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d606a-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d606a-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d606a-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d606a-109">EcpUrl-RET (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-109">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md)
  
```XML
<EcpUrl-ret/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d606a-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d606a-110">Attributes and elements</span></span>

<span data-ttu-id="d606a-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d606a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d606a-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="d606a-112">Attributes</span></span>

<span data-ttu-id="d606a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d606a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d606a-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d606a-114">Child elements</span></span>

<span data-ttu-id="d606a-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d606a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d606a-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d606a-116">Parent elements</span></span>

|<span data-ttu-id="d606a-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d606a-117">**Element**</span></span>|<span data-ttu-id="d606a-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d606a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d606a-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="d606a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d606a-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d606a-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d606a-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d606a-121">Text value</span></span>

<span data-ttu-id="d606a-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações da marca de retenção do usuário.</span><span class="sxs-lookup"><span data-stu-id="d606a-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d606a-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="d606a-123">Remarks</span></span>

<span data-ttu-id="d606a-124">O elemento **EcpUrl-RET** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="d606a-124">The **EcpUrl-ret** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d606a-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="d606a-125">See also</span></span>



[<span data-ttu-id="d606a-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="d606a-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

