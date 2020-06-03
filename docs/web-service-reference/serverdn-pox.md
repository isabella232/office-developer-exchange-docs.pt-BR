---
title: ServerDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: O elemento ServerDN especifica o nome distinto do computador que está executando o Microsoft Exchange Server 2007.
ms.openlocfilehash: 16c6e7368e221b7e54c8d7d63532bb29464a7e54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461993"
---
# <a name="serverdn-pox"></a><span data-ttu-id="9f27f-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-103">ServerDN (POX)</span></span>

<span data-ttu-id="9f27f-104">O elemento **ServerDN** especifica o nome distinto do computador que está executando o Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="9f27f-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="9f27f-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9f27f-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9f27f-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9f27f-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9f27f-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9f27f-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9f27f-110">Attributes and elements</span></span>

<span data-ttu-id="9f27f-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f27f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f27f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f27f-112">Attributes</span></span>

<span data-ttu-id="9f27f-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f27f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f27f-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f27f-114">Child elements</span></span>

<span data-ttu-id="9f27f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9f27f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9f27f-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f27f-116">Parent elements</span></span>

|<span data-ttu-id="9f27f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f27f-117">**Element**</span></span>|<span data-ttu-id="9f27f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f27f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f27f-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="9f27f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9f27f-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9f27f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9f27f-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9f27f-121">Text value</span></span>

<span data-ttu-id="9f27f-122">O valor de texto representa o nome distinto do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f27f-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f27f-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="9f27f-123">Remarks</span></span>

<span data-ttu-id="9f27f-124">O valor **ServerDN** é usado somente quando o [tipo (POX)](type-pox.md) é igual a Exch.</span><span class="sxs-lookup"><span data-stu-id="9f27f-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9f27f-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="9f27f-125">See also</span></span>



[<span data-ttu-id="9f27f-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="9f27f-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

