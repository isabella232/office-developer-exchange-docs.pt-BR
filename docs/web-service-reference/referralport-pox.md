---
title: ReferralPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cd693f1e-fed4-4eb9-8297-178906f47050
description: O elemento ReferralPort especifica a porta usada para obter uma referência a um diretório.
ms.openlocfilehash: 6b3968d7b2f252439d2dfbc647bd8337668cf818
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456785"
---
# <a name="referralport-pox"></a><span data-ttu-id="a1163-103">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-103">ReferralPort (POX)</span></span>

<span data-ttu-id="a1163-104">O elemento **ReferralPort** especifica a porta usada para obter uma referência a um diretório.</span><span class="sxs-lookup"><span data-stu-id="a1163-104">The **ReferralPort** element specifies the port that is used to get a referral to a directory.</span></span> 
  
[<span data-ttu-id="a1163-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a1163-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a1163-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a1163-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a1163-109">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-109">ReferralPort (POX)</span></span>](referralport-pox.md)
  
```xml
<ReferralPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a1163-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a1163-110">Attributes and elements</span></span>

<span data-ttu-id="a1163-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a1163-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1163-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a1163-112">Attributes</span></span>

<span data-ttu-id="a1163-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1163-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1163-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a1163-114">Child elements</span></span>

<span data-ttu-id="a1163-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a1163-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1163-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a1163-116">Parent elements</span></span>

|<span data-ttu-id="a1163-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a1163-117">**Element**</span></span>|<span data-ttu-id="a1163-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a1163-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1163-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="a1163-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a1163-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a1163-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1163-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a1163-121">Text value</span></span>

<span data-ttu-id="a1163-122">O valor de texto representa a porta usada para acessar o servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1163-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1163-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a1163-123">Remarks</span></span>

<span data-ttu-id="a1163-124">O elemento **ReferralPort** é usado somente quando o elemento [tipo (POX)](type-pox.md) é igual a Exch ou expr.</span><span class="sxs-lookup"><span data-stu-id="a1163-124">The **ReferralPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a1163-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="a1163-125">See also</span></span>



[<span data-ttu-id="a1163-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="a1163-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

